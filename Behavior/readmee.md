# Behavioral Scientist — Bargaining Game Experiments

This folder contains the oTree implementation, screenshots, and LLM session data for the bargaining game study.  
We compare **human subjects** and **large language models (LLMs)** in both 2-player and 3-player bargaining games.

---

## Deployment Steps

1. Download `otree_app.zip` from this folder.  
2. Open terminal and navigate to the file location.  
3. Install requirements:
   ```bash
   pip3 install -U otree zipserver
4. Run the app:
   ```bash
   zipserver otree_app.zip
5. Open http://localhost:8000 in your browser → Admin panel → Create session.

### Session Config
Two-player version

Players: 2

Each chooses demand $d_i \in [0,100]$

Payoff rule:
- Players: `n` (we analyze `n = 2` and `n ≥ 3`)
- Payoffs:
  - If `S ≤ 100`: `every one gets what they ask for`
  - If `S > 100`: `every one gets 0 payoff`

**Intuition.** Everyone demands a share from a fixed pie of size 100. If the group stays within budget, each gets exactly what they asked for; otherwise, everyone gets 0.

### Ethics Note

The experiment was conducted in a classroom setting with classmates.

Participation was voluntary and anonymous.

No monetary incentives were used; payoffs were points only.

LLM sessions (ChatGPT-5, Qwen, Yi) complied with providers’ terms of service.

Data shared in this repo contains no personal information.
