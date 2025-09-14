# Economist Perspective

This folder documents the **theoretical analysis** of the bargaining game.

---

## 1. Game Definition

We study the **simultaneous-demand bargaining game** with $n$ players:

- Strategy set for each player $i$:  
  \[
  S_i = [0,100]
  \]

- If player $i$ chooses demand $d_i \in S_i$, the profile is $d = (d_1, \dots, d_n)$ with total  
  \[
  S = \sum_{j=1}^n d_j
  \]

- Payoffs:  
  \[
  u_i(d) =
  \begin{cases}
  d_i & \text{if } S \leq 100, \\
  0 & \text{if } S > 100.
  \end{cases}
  \]

This corresponds to the "divide-the-dollar" (or "cake-cutting") bargaining framework, extended to more than two players.

---

## 2. Equilibrium Concept

- **Nash Equilibrium (NE):**  
  A profile $d^\star = (d_1^\star,\dots,d_n^\star)$ is an NE if for all $i$:  
  \[
  u_i(d_i^\star, d_{-i}^\star) \geq u_i(d_i, d_{-i}^\star) \quad \forall d_i \in S_i
  \]

- Existence:  
  - In finite normal-form games, Nash proved existence of (possibly mixed) equilibria using a fixed-point theorem.  
    See *Osborne & Rubinstein (1994), A Course in Game Theory*, p. 22.  
  - For continuous games with compact strategy sets and continuous, quasi-concave payoffs, existence follows from **Glicksberg’s generalization** of Kakutani’s fixed-point theorem.  
    See *Shoham & Leyton-Brown (2008), Multiagent Systems*, Ch. 2.

---

## 3. Analytical Results

### (a) Two-player case
- **Efficient NE:** All $(d_1, d_2)$ with $d_1+d_2=100$.  
  These outcomes exhaust the surplus, and unilateral deviations either overshoot (yielding 0) or reduce one’s own payoff.  
- **Fairness:** From equal split $(50,50)$ to extreme $(99,1)$.

### (b) $n \geq 3$ case
- **Efficient NE:** All profiles with $\sum_i d_i=100$.  
- **Inefficient “zero-payoff” NE:** Profiles where $\sum_{j\neq i} d_j > 100$ for every $i$.  
  In such cases, no single player can unilaterally deviate to obtain a positive payoff.  
- This multiplicity introduces **coordination risk** absent in the $n=2$ case.

---

## 4. Alternating-Offers Extension

Following *Osborne & Rubinstein (1994), Ch. 7*:

- Model: Players alternate making proposals until agreement.  
- **Subgame Perfect Nash Equilibrium (SPNE):**  
  By backward induction, immediate agreement occurs on an efficient division.  
- With discount factors $\delta_1, \delta_2 \in (0,1)$:  
  \[
  \text{Proposer’s share } a^\star = \frac{1-\delta_2}{1-\delta_1\delta_2}, \qquad 
  1-a^\star \text{ to responder.}
  \]
- Proof idea: Stationarity + one-deviation property $\Rightarrow$ responders accept any offer $\geq$ their continuation value. Intersections of thresholds yield a unique efficient split.

---

## 5. Welfare & Fairness

- **Pareto efficiency:** NE are efficient iff $\sum d_i = 100$.  
- **Utilitarian welfare:** $100$ in efficient NE; $0$ in over-ask equilibria ($n \geq 3$).  
- **Fairness:** Equal splits minimize inequality; alternating-offers models give first-mover advantage.  
  See *Osborne & Rubinstein (1994), §§7.3–7.4, pp. 122–131.*

---

## 6. References

- Osborne, M. J., & Rubinstein, A. (1994). *A Course in Game Theory*. MIT Press.  
  - §7.3: Subgame Perfect Equilibrium, pp. 122–126.  
  - §7.4: Variants of Alternating-Offers, pp. 127–131.  

- Shoham, Y., & Leyton-Brown, K. (2008). *Multiagent Systems*. Cambridge University Press.  
  - Ch. 2: Strategic-form games and Nash equilibria.  

- Roughgarden, T. (2016). *Twenty Lectures on Algorithmic Game Theory*. Lecture 2: Equilibria and computation.  

