# 🎯 Strategic Bargaining, Auctions, and Mechanism Design with Humans and LLMs

> **Abstract**  
> This project explores how bargaining, auction, and matching outcomes evolve when participants are **humans vs. LLMs**.  
> It combines **game-theoretic theory**, **computational modeling**, and **behavioral experiments** to study efficiency, fairness, and robustness in strategic environments.  
> - **Two-player simultaneous-demand bargaining:** all surplus-exhausting allocations are Nash equilibria (efficient but unequal).  
> - **Three-player and higher:** coordination failures yield inefficient “over-ask” equilibria.  
> - **Common-value auctions:** LLM agents mix rational and behavioral bidding patterns (winner’s curse, shading).  
> - **Refugee burden-sharing:** proposes **RCCM**—a two-stage *Robust Condorcet + Credit Matching* mechanism improving fairness, efficiency, and legitimacy.

---

## 👥 Authors and Roles

| Name | Role | Responsibilities |
|------|------|------------------|
| **Peilin Wu** | 🎓 Economist | Formal modeling, NE/SPNE derivations, welfare and fairness analysis |
|  | 💻 Computational Scientist | Matrix construction, NashPy/QuantEcon computation, GTE visualization |
|  | 🧠 Behavioral Scientist | oTree experiments, human/LLM sessions, data analysis |
|  | 🏗️ Mechanism Designer | RCCM design (Condorcet → Credit Clearing → Stable Matching) and KPI evaluation |

---

## 🧩 Contribution to SDGs

This project contributes to the **United Nations Sustainable Development Goals**:

| SDG | Goal | Alignment |
|-----|------|------------|
| **4** | Quality Education | Reproducible, open-source computational social-science education |
| **9** | Industry, Innovation & Infrastructure | Responsible LLM integration in experimental economics |
| **10** | Reduced Inequalities | Quantifying fairness and welfare in allocation mechanisms |
| **16** | Peace, Justice & Strong Institutions | Designing transparent and legitimate decision mechanisms |

---

## 🙏 Acknowledgments

Grateful to **Prof. Luyao Zhang** and classmates for guidance and feedback.  
Appreciation to **open-source communities**: [NashPy](https://nashpy.readthedocs.io/), [QuantEcon](https://quantecon.org/), [Game Theory Explorer](https://gtegames.com/), and [oTree](https://www.otree.org/).  
Thanks also to **responsible AIGC tools** (GPT-5, Qwen3, DeepSeek, Hunyuan) for code organization, drafting, and visualization support.

---

## ⚖️ Disclaimer

> This repository supports the final research proposal submitted to **COMSCI/ECON 206: Computational Microeconomics**, instructed by **Prof. Luyao Zhang** at **Duke Kunshan University** in **Autumn 2025**.

---

## 🌱 Statement of Intellectual and Professional Growth

Through PS1 → PS2 → Final Proposal and field experiences, this project fostered:

- **Research design**: from formal modeling to empirically testable hypotheses.  
- **Technical mastery**: NE/SPNE computation, oTree deployment, and reproducible workflows.  
- **Interdisciplinary thinking**: bridging economics, computation, and behavioral data.  
- **Professional growth**: collaboration, transparent communication, ethical reflection, and responsible AI practice.

---

## 🗂️ Table of Contents

1. [Abstract](#-strategic-bargaining-auctions-and-mechanism-design-with-humans-and-llms)  
2. [Authors and Roles](#-authors-and-roles)  
3. [Contribution to SDGs](#-contribution-to-sdgs)  
4. [Acknowledgments](#-acknowledgments)  
5. [Disclaimer](#-disclaimer)  
6. [Statement of Growth](#-statement-of-intellectual-and-professional-growth)  
7. [Navigation Instructions](#-navigation-instructions)  
8. [Repository Map](#-repository-map)  
9. [Embedded Media](#-embedded-media)  
10. [Reproducibility Guide](#-reproducibility-guide)  
11. [Citations](#-citations)

---

## 🧭 Navigation Instructions

**Locate core components easily:**

| Category | Folder | Description |
|-----------|---------|-------------|
| Equilibria Computation | [`computational_scientist/colab/`](computational_scientist/colab/) | 2P matrices + NashPy runs |
| Enumeration (3P+) | [`computational_scientist/enumeration/`](computational_scientist/enumeration/) | Over-ask NE checks |
| Mechanism Design | [`mechanism_design/src/`](mechanism_design/src/) | RCCM: Condorcet → Credit Clearing → Stable Matching |
| KPI Experiments | [`mechanism_design/experiments/`](mechanism_design/experiments/) | Fairness, Efficiency, Legitimacy |
| Auctions | [`simulations/auctions/`](simulations/auctions/) | LLM bidding (T1/T2/CONTROL) |
| oTree App | [`behavioral_scientist/otree_app/`](behavioral_scientist/otree_app/) | Human experiment interface |
| Figures & Outputs | [`figures/`](figures/) | Plots, tables, and exports |
| Documentation | [`docs/report/`](docs/report/) | Final LaTeX report + poster + field trip |

---

## 📁 Repository Map

```plaintext
.
├── computational_scientist/
│   ├── colab/
│   └── enumeration/
├── mechanism_design/
│   ├── src/
│   └── experiments/
├── simulations/
│   └── auctions/
├── behavioral_scientist/
│   ├── otree_app/
│   └── sessions/
├── figures/
├── outputs/
├── poster/
├── media/
├── docs/
│   ├── report/
│   └── field_trip/
├── sample.bib
└── README.md
