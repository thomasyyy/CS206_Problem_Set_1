\section*{Behavioral Scientist --- oTree Experiment \& LLM Comparison}

This folder contains the \textbf{behavioral experiment implementation and results} for the bargaining game study. 
It includes both human session data (via oTree) and parallel large language model (LLM) sessions.

\subsection*{Folder Structure}
\begin{verbatim}
behavioral_scientist/
├── otree_app.zip                # Full oTree app (ready to deploy on oTree Hub or local server)
├── screenshots/                 # Screenshots of instructions, decision screens, and results pages
│   ├── Instructions.png
│   ├── Result_for_2.png
│   └── Results_for_3.png
├── llm/                         # LLM simulation assets
│   ├── prompts.txt              # Prompts used to simulate LLM players
│   ├── transcript.tex           # Example dialogues between LLM "players"
│   └── settings.json            # Parameters (model names, temperature, max tokens, etc.)
\end{verbatim}

\subsection*{Deployment Steps (oTree)}
\begin{enumerate}
    \item Install oTree runtime (Python 3.9+):
    \begin{verbatim}
    pip3 install -U otree zipserver
    \end{verbatim}
    \item Launch the app:
    \begin{verbatim}
    zipserver otree_app.zip
    \end{verbatim}
    This automatically unpacks the \texttt{.otreezip} and launches the admin panel.
    \item Start a session:
    \begin{itemize}
        \item Open the local admin panel (usually \texttt{http://localhost:8000}).
        \item Choose 2-player or 3-player configuration.
        \item Share participant links and observe results in real time.
    \end{itemize}
\end{enumerate}

\subsection*{Session Configurations}
\textbf{Two-player (2P) bargaining game:} each participant demands $d_i \in \{0,\dots,100\}$.
\[
u_i(d) = 
\begin{cases}
d_i & \text{if } \sum_j d_j \leq 100, \\
0   & \text{if } \sum_j d_j > 100.
\end{cases}
\]

\noindent
\textbf{Three-player (3P) bargaining game:} same payoff rule extended to $n=3$. Coordination failures are more frequent, leading to zero-payoff outcomes.

\subsection*{Data \& Screenshots}
\begin{itemize}
    \item Instructions page: \texttt{screenshots/Instructions.png}
    \item Two-player session results: \texttt{screenshots/Result\_for\_2.png}
    \item Three-player session results: \texttt{screenshots/Results\_for\_3.png}
\end{itemize}

\subsection*{LLM Sessions}
\begin{itemize}
    \item Models: ChatGPT-5, Qwen, Yi (Yi added in 3-player case).
    \item Action set: $\{0,25,50,75,100\}$.
    \item Example prompt (from \texttt{prompts.txt}):
\begin{verbatim}
You are Player 1 in a bargaining game. 
You and the other players each demand from 0–100. 
If the sum ≤ 100, you get your demand; otherwise all get 0. 
What do you choose?
\end{verbatim}
    \item Outputs and reasoning are logged in \texttt{transcript.tex}.
\end{itemize}

\subsection*{Ethics Note}
Human participants (two classmates) participated voluntarily. 
No personal or identifying data was collected. 
Risks are minimal; the main ethical concern is fair reporting. 
Results are anonymized, reproducible, and available in this repository.
