# Bargaining Game: An Interdisciplinary Study

## Abstract
This repository accompanies **Problem Set 1 (COMSCI/ECON 206: Computational Microeconomics, Autumn 2025)**.  
The project extends the classic two-player bargaining game to three players, combining theory, computation, and behavioral evidence.  
It formalizes equilibrium concepts, computes equilibria with tools such as **NashPy** and **Game Theory Explorer**, and deploys an **oTree experiment** tested with both human participants and large language models (LLMs).

---

## Task Summary
- **Economist (theory & welfare):** Formalize the bargaining game, characterize Nash and SPNE equilibria, and analyze efficiency and fairness.  
- **Computational Scientist (coding & tools):** Construct payoff matrices, compute equilibria via Google Colab & NashPy, and build an extensive form in GTE.  
- **Behavioral Scientist (experiment & AI comparison):** Deploy oTree, run human sessions, simulate with LLMs, and compare outcomes to theory.  

---

## Reproduction Steps
1. **Economist part**  
   - See `economist/README.md` for definitions, textbook references, and analytical solution notes.

2. **Computational Scientist part**  
   - Open `computational_scientist/notebook.ipynb` in **Google Colab**  
     or run locally after installing:
     ```bash
     pip install nashpy numpy matplotlib
     ```
   - For extensive form, open the `.gte` files in **Game Theory Explorer**.  
   - Screenshots of solver outputs and trees are in `computational_scientist/gte/`.

3. **Behavioral Scientist part**  
   - Unzip and run `behavioral_scientist/otree_app.zip`.  
   - Install requirements:
     ```bash
     pip3 install -U otree zipserver
     zipserver your_project.otreezip
     ```
   - Screenshots of game pages are in `behavioral_scientist/screenshots/`.  
   - LLM prompts and transcripts are in `behavioral_scientist/llm/`.  

4. **Paper**  
   - See `Problem_Set_1.pdf` (compiled LaTeX source) for the write-up including figures and analysis.  

---

## Data/Code Availability
- 📂 GitHub repository: [CS206_Problem_Set_1](https://github.com/thomasyyy/CS206_Problem_Set_1)  
- 📑 Google Colab notebook: [link](https://colab.research.google.com/drive/1vxD5r5U3DXyJXzuUMp2tLGh2g5DKo3WB)  

---

## Software Citations
- Osborne, M. J., & Rubinstein, A. (1994). *A Course in Game Theory*. MIT Press.  
- Shoham, Y., & Leyton-Brown, K. (2008). *Multiagent Systems*. Cambridge University Press.  
- Knight, V. (2021). *NashPy: A Python library for the computation of equilibria of 2-player strategic games*, Version 0.0.28.  
- Savani, R., & von Stengel, B. (2015). *Game Theory Explorer – Software for the Applied Game Theorist*. Computational Management Science, 12, 5–33.  
- Sargent, T. J., & Stachurski, J. (2021). *Quantitative Economics (Python)*, Version 0.5.1.  
