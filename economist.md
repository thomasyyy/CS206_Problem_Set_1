# Economist Perspective

This folder documents the **theoretical analysis** of the bargaining game and provides page/section citations to the textbooks required by the assignment.

---

## 1) Game Definition (Simultaneous-Demand Bargaining)

- Players: `n` (we analyze `n = 2` and `n ≥ 3`)
- Strategy set of player i: demands `d_i ∈ [0, 100]`
- Total demand: `S = Σ_j d_j`
- Payoffs:
  - If `S ≤ 100`: `u_i(d) = d_i`
  - If `S > 100`: `u_i(d) = 0`

**Intuition.** Everyone demands a share from a fixed pie of size 100. If the group stays within budget, each gets exactly what they asked for; otherwise, everyone gets 0.

---

## 2) Equilibrium Concept (Nash Equilibrium)

- A profile `d* = (d_1*, …, d_n*)` is a Nash equilibrium (NE) if no player can improve by changing only her own demand:
  - For every player i and every feasible deviation `d_i`,
    ```
    u_i(d_i*, d_-i*) ≥ u_i(d_i, d_-i*)
    ```
- Existence (textbook pointers):
  - Finite normal-form games: Nash’s fixed-point theorem (classic)
  - Continuous, compact strategy sets with continuity/quasi-concavity: Glicksberg’s theorem

**Citations:**
- Shoham & Leyton-Brown (2008), *Multiagent Systems*, Ch. 2 (definitions; existence)
- Osborne & Rubinstein (1994), *A Course in Game Theory*, Ch. 2 (background), Ch. 7 for bargaining

---

## 3) Analytical Results

### A) Two Players (`n = 2`)
- **NE set (pure strategies):** All pairs `(d_1, d_2)` with `d_1 + d_2 = 100`.
  - Any unilateral increase makes `S > 100` → both get 0 → not profitable.
  - Any unilateral decrease lowers your own payoff → not profitable.
- **Efficiency:** Every NE with `S = 100` is Pareto efficient (the pie is fully allocated).
- **Fairness:** Varies across equilibria, from equal `(50, 50)` to unequal `(99, 1)` etc.

### B) Three or More Players (`n ≥ 3`)
- **Efficient NE:** All `d` with `Σ_i d_i = 100`.
- **Inefficient “over-ask” NE (all get 0):**
  - Any profile `d` such that **for every player i**,
    ```
    Σ_{j ≠ i} d_j > 100
    ```
  - Intuition: Others already exceed the budget without you; no unilateral move can recover a positive payoff, so you can’t improve → NE.
- These zero-payoff equilibria **do not** exist for `n = 2` but appear for `n ≥ 3`.

**Welfare summary:**
- Utilitarian welfare = 100 at efficient NE; = 0 at over-ask NE.

---

## 4) Alternating-Offers Bargaining (Extensive Form; SPNE)

We also analyze the Rubinstein-style alternating-offers model (perfect information):

- Players alternate proposals; responders accept/reject.
- **Subgame Perfect Nash Equilibrium (SPNE):** Immediate agreement on an efficient division under standard assumptions (A1–A4 in Osborne & Rubinstein, Ch. 7).
- With geometric discounts `δ_1, δ_2 ∈ (0,1)`, the proposer’s share is a* = (1 - δ_2) / (1 - δ_1 δ_2) and the responder gets `1 - a*`.

**Key properties:**
- Stationary strategies; one-deviation property.
- First-mover advantage (even with equal patience).
- Variants (outside options, risk of breakdown, indivisibilities) shift SPNE in predictable ways.
- With more than two players, uniqueness fails and many SPNE can be supported.

**Citations:**
- Osborne & Rubinstein (1994), *A Course in Game Theory*, Ch. 7:
- §7.1–§7.3 (pp. 118–126): model & SPNE characterization (Proposition 122.1)
- Example 125.1: split-the-pie formula for `a*`
- §7.3.2 (p. 126): properties (efficiency, first-mover advantage)
- §7.4.3–§7.4.5 (pp. 127–131): variants and `n > 2`

---

## 5) Welfare & Fairness (Recap)

- **Pareto efficiency:**
- Simultaneous-demand: efficient iff `Σ_i d_i = 100`
- Alternating-offers: SPNE is efficient (immediate agreement)
- **Utilitarian welfare:**
- 100 at efficient NE, 0 at over-ask NE (for `n ≥ 3`)
- **Fairness:**
- Equal split minimizes inequality.
- First-mover advantage in alternating-offers.
- Outside options tilt the outcome toward better outside options.

---

## 6) How this maps to the assignment (Part 1)

- **Equilibrium concept**: Defined NE and SPNE; cited existence results (Nash/Glicksberg; O&R Ch. 7).
- **Analytical solution**: Characterized NE sets for `n=2` and `n≥3`; discussed efficiency/fairness.
- **Interpretation**: Multiplicity (continuum of NE; over-ask NE for `n≥3`), realism vs. SPNE refinement, bounded rationality and computational tractability pointers.

---

## 7) References (with page/section pointers)

- **Osborne, M. J., & Rubinstein, A. (1994).** *A Course in Game Theory*. MIT Press.  
- p. 117: simultaneous-demand split-the-pie description  
- Ch. 7 §7.1–§7.3 (pp. 118–126): alternating-offers model & SPNE (Prop. 122.1)  
- Example 125.1: proposer share formula  
- §7.3.2 (p. 126): efficiency, stationarity, first-mover advantage  
- §7.4.3–§7.4.5 (pp. 127–131): outside options, breakdown risk, `n>2`.

- **Shoham, Y., & Leyton-Brown, K. (2008).** *Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations*. Cambridge University Press.  
- Ch. 2: normal-form games, NE definitions, existence (incl. Glicksberg).




