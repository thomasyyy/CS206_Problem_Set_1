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
def payoff(demands):
    total = sum(demands)
    if total <= 100:
        return demands
    else:
        return [0 for _ in demands]

