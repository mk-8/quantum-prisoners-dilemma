# Quantum Strategies in the Prisoner's Dilemma

## Overview
The introduction of quantum strategies in the Prisoner’s Dilemma can resolve the dilemma while ensuring an absolute advantage against any classical strategy. This project explores the impact of quantum strategies on the game dynamics and expected payoffs.

## Quantum Representation of the Game
In the quantum version of the Prisoner’s Dilemma, the classical strategies **Cooperate (|C⟩)** and **Defect (|D⟩)** are represented as quantum states. The overall game state is described as a vector in a Hilbert space with the basis states:
- **|CC⟩** (both cooperate)
- **|CD⟩** (Alice cooperates, Bob defects)
- **|DC⟩** (Alice defects, Bob cooperates)
- **|DD⟩** (both defect)

Here, the first letter in each state represents Alice’s move, while the second represents Bob’s.

## Quantum Strategy Framework
To incorporate quantum entanglement between Alice and Bob's moves, the game begins with a **unitary transformation** **Ĵ** applied to the initial state **|CC⟩**. This models any potential entanglement between their choices.

### Game Flow:
1. **Initialization:** The game starts in state **|CC⟩**, with a unitary transformation **Ĵ** applied.
2. **Player Strategies:** Alice and Bob apply their respective strategies, represented as **2×2 unitary operators** **ÛA** and **ÛB**.
3. **Measurement and Payoff Calculation:**
   - The final state is obtained by applying the inverse transformation **Ĵ†**, followed by a measurement:
     
     \[ |Ѱ_f⟩ = Ĵ^† (ÛA ⊗ ÛB) Ĵ |CC⟩ \]
   
   - The expected payoff for Alice is computed using:
     
     \[ A = rP_{CC} + pP_{DD} + tP_{DC} + sP_{CD} \]
     
     where **r, p, t, s** are standard payoff matrix values, and **P_{CC}, P_{DD}, P_{DC}, P_{CD}** are the measured probabilities of each outcome.

## Simulation and Analysis
Quantum strategies are modeled as a **two-parameter set of unitary matrices**. The game is then simulated across various settings of these parameters (𝜙, 𝜃) to analyze Alice’s expected payoff distribution.

---
### Future Work
- Extending the model to include mixed quantum strategies.
- Exploring Nash equilibria in the quantum domain.
- Investigating real-world implications of quantum strategies in decision-making.

## References
- Eisert, J., Wilkens, M., & Lewenstein, M. (1999). Quantum Games and Quantum Strategies.
- Meyer, D. A. (1999). Quantum Strategies.

## Contact
For any questions or contributions, feel free to reach out!

---

