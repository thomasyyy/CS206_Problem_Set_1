# Point-by-Point Response to Reviewer Feedback

---

## Reviewer: Prof. Luyao Zhang  
**Manuscript:** *Problem Set 1 — Deployment of a Strategic Game: An Interdisciplinary Study*

I thank the reviewer for constructive feedback. Below I respond point-by-point. For each comment, I provide: the original excerpt, my response, methodological rationale, concrete edits, and evidence of compliance.

---

### 1. oTree adaptation not fully explained

**Original comment:**  
> “It’s unclear how you modified the original oTree app: Did you adjust instructions, payoff calculations, UI logic, number of rounds, session config, or player roles?”

**Response:** I agree. Section *oTree deployment and adaptations* now documents the base demo, session configurations, payoff implementation, instruction changes, timing, and data capture.

**Rationale:** Transparent reporting of experimental software aligns with reproducibility norms in behavioral/experimental economics and HCI.

**Concrete edits made:**
- Stated that I adapted the official oTree bargaining/public-goods demo.  
- Added two sessions `Bargaining2P` / `Bargaining3P` with `num_rounds=10`.  
- Generalized `Constants.players_per_group` from 2 → 3 for 3P treatment.  
- Implemented budget rule in `models.py::set_payoffs()`.  
- Customized instructions with numeric examples and comprehension checks.  
- Added 60s decision timeout + attention checks.  
- Logged demands/payoffs to `Participant.vars` and exported CSV.

**Evidence of compliance:**  
- New subsection *oTree deployment and adaptations*.  
- Figures showing instructions and results.  
- Repository artifacts in *Data/Code Availability*.  

---

### 2. Missing required open-source software citations

**Original comment:**  
> “Please include formal citations for NashPy, Game Theory Explorer, and oTree following the software’s documentation.”

**Response:** I agree and added formal citations for **NashPy**, **GTE**, and **oTree**.

**Rationale:** Proper citation credits maintainers, enables reproducibility, and satisfies rubric requirements.

**Concrete edits made:**
- Added NashPy cite at first solver usage.  
- Added GTE cite in opening sentence of GTE subsection.  
- Added oTree cite at start of *oTree adaptations* section.  

**Evidence of compliance:**  
- In-text citations added at first use.  
- Bibliography updated with software entries.  

---

### 3. Minor writing and figure suggestions

**Original comment:**  
> “Several figures are not labeled or referenced precisely. Trim long LLM block quotes.”

**Response:** Implemented. All figures now have captions/labels; long quotes condensed.

**Rationale:** Precise figure referencing improves readability; summarizing LLM outputs preserves flow.

**Concrete edits made:**
- Added captions + labels to all figures.  
- Inserted vertical flowchart under *Introduction*.  
- Condensed LLM quotes to a representative line.  
- Removed non-scholarly links.  

**Evidence of compliance:**  
- Figure references appear near each discussion.  
- Flowchart satisfies rubric’s visualization requirement.  

---

### Summary mapping of comments to revisions

| Reviewer comment                           | Concrete edits                                               | Evidence / Where to look                    |
|--------------------------------------------|--------------------------------------------------------------|---------------------------------------------|
| oTree adaptation unclear                    | New *otree-adaptations* section; session types, payoff, UI   | Section otree-adaptations; oTree figures     |
| Add software citations                      | In-text cites for NashPy, GTE, oTree; biblio entries added   | Subsections; Bibliography                    |
| Figures unlabeled; long LLM quotes          | Captions + labels; condensed quotes                         | Figures and Section 4.2(b)                   |
| Rubric visualization (flowchart)            | Added vertical flowchart with forced placement               | Figure “flow-vertical”                       |

---

## Reviewer: Yanzhen Liu  
**Date:** 2025-09-17  
**Project:** *Simultaneous–Alternating–3P Bargaining Expansion*

I sincerely thank Yanzhen Liu for constructive and generous comments. Below are my responses.

---

### 1. Replicability
**Comment:** Outputs from Colab are included but more replicability is encouraged.  
**Response:** Agreed. Added explicit references to GitHub assets in text.  
**Change made:** File references added; Data/Code Availability updated.

### 2. Coherence
**Comment:** Link economist and computational parts more clearly.  
**Response:** Agreed. Added bridging sentence on inefficient equilibria.  
**Change made:** Transitional remarks added in theory and computation sections.

### 3. Resourcefulness
**Comment:** Ensure references/software coverage is complete.  
**Response:** Confirmed and added algorithmic game theory reference.  
**Change made:** Bibliography updated; in-text citations added.

### 4. Minor Writing Suggestions
**Comment:** Text too dense; improve readability.  
**Response:** Agreed. Increased spacing, shortened quotes.  
**Change made:** Adjusted table spacing; condensed dialogue blocks.

### 5. Organization and Flow
**Comment:** Add 2–3 summary sentences at section ends.  
**Response:** Fully agree.  
**Change made:** Added transition sentences at end of each section.

### 6. Ethical and Practical Implications
**Comment:** Validate with larger samples or pre-registered experiments.  
**Response:** Agreed. Will expand in PS2.  
**Change made:** Behavioral conclusion mentions pre-registration.

### 7. Courtesy and Encouragement
**Comment:** Reviewer describes project as solid and outstanding.  
**Response:** Grateful and motivated to maintain rigor.  

---

### Summary of Peer Feedback Integration

| Reviewer suggestion       | Revision implemented                                | Location                        |
|---------------------------|-----------------------------------------------------|---------------------------------|
| Strengthen replicability  | Explicit GitHub file references                     | Section “Computational Scientist” |
| Add coherence sentence    | Transitional remarks on equilibria                  | Theory + Computation sections   |
| Resourcefulness           | Software + new reference (Roughgarden 2016)         | Bibliography, in-text cites     |
| Improve readability       | More spacing, shorter quotes                        | Tables, Section 4.2(b)          |
| Improve cohesion          | Transition sentences added                          | End of each section             |
| Expand experiments        | Plan pre-registration & larger sample               | Behavioral conclusion           |

---

**Versioning and traceability:**  
The GitHub repository includes diffs, screenshots, session CSVs, code/notebooks, and GTE exports to support all revisions.
