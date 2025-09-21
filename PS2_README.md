# COMSCI/ECON 206 – Problem Set 2 : Play to Innovate
**Peilin Wu · Autumn 2025**

> One PDF + Organized Repo as required by the syllabus.

---

## 📑 Deliverables (per rubric)

This repository contains all revised materials required for Problem Set 2:

- **Problem Set 1 (Updated)**  
  File: `Problem_Set_1_updated.pdf`

- **Acknowledgments**  
  Included at the beginning of `Problem_Set_1_updated.pdf`

- **Point-by-Point Responses (Appendix)**  
  See Appendix A in `Problem_Set_1_updated.pdf`

- **Problem Set 2: Mechanism Design (Winner’s Curse with LLMs)**  
  File: `Problem_Set_2_PeilinWu.pdf`  
  Contains: auction design, hypotheses, AI experiment setup, results, and analysis

➡️ All of the above deliverables are committed together in this repository and referenced here in the root `README.md`.

---

## 📦 Repository Structure
- `economist/` – game forms, equilibrium notes, GTE exports  
- `computational_scientist/` – NashPy demos, Colab notebook, solver outputs  
- `behavioral_scientist/` – oTree app + screenshots + session CSVs  
- `mechanism_design/` – LLM prompts, transcripts, aggregated results, analysis scripts  
- `references/` – `refs.bib` (Chicago Author–Date), Nobel links, software citations  
- `scripts/` – one-click reproduction  

---

## 🧪 Reproducibility
```bash
# create env (conda) or use requirements.txt
conda env create -f computational_scientist/env.yml
conda activate ps2

# run all demos + regenerate tables/plots
bash scripts/run_all.sh
