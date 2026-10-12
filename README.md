# Qiskit Fall Fest 2026 - Vishnu Institute of Technology

This repository contains my solutions to all 4 challenges for the **Qiskit Fall Fest 2026** organized by **IBM Quantum** and **Vishnu Institute of Technology**.

---

## Repository Structure

| File | Challenge Name | Description |
| :--- | :--- | :--- |
| [`challenge_1_predict_the_output.ipynb`](./challenge_1_predict_the_output.ipynb) | **Challenge 1: Predict the Output** | Investigating single-qubit circuits with X and H gates; comparing theoretical predictions with 100-shot simulations. |
| [`challenge_2_biased_coin.ipynb`](./challenge_2_biased_coin.ipynb) | **Challenge 2: Make the Quantum Coin Biased** | Using Ry rotation gates to create biased quantum coin states (75:25 and 25:75) and answering the challenge question. |
| [`challenge_3_change_correlation.ipynb`](./challenge_3_change_correlation.ipynb) | **Challenge 3: Can you change the correlation?** | Starting from an entangled Bell state (00 & 11) and adding an X gate to flip the correlation to opposite outcomes (01 & 10). |
| [`challenge_4_correlation_switch.ipynb`](./challenge_4_correlation_switch.ipynb) | **Challenge 4: Quantum Correlation Switch** | Designing a 2-qubit circuit that toggles between correlated outcomes and anti-correlated outcomes using minimal quantum gates. |

---

## Summary of Results

### Challenge 1: Predict the Output
- **Circuit A (1x X gate):** Theoretical: 100% `1` | Actual (100 shots): `{'1': 100}`
- **Circuit B (2x X gates):** Theoretical: 100% `0` | Actual (100 shots): `{'0': 100}`
- **Circuit C (1x H gate):** Theoretical: 50% `0` / 50% `1` | Actual (100 shots): ~50:50 distribution

### Challenge 2: Make the Quantum Coin Biased
- **Circuit 1 (Ry(π/3)):** Biased towards `0` (~75% `0`, ~25% `1`).
- **Circuit 2 (Ry(2π/3)):** Biased towards `1` (~25% `0`, ~75% `1`).
- **Challenge Question Answer:** Included in the final cell, explaining state vector rotations on the Bloch sphere and Born's rule.

### Challenge 3 & 4: Quantum Correlation & Switch
- **Correlated Circuit (Bell State):** $H \to CX \implies$ Outcomes: `00` and `11`.
- **Anti-Correlated Circuit (Correlation Switch):** $H \to CX \to X \implies$ Outcomes: `01` and `10`.

---

## Tools & Libraries Used
- **Language:** Python
- **Quantum Framework:** Qiskit / Qiskit-Aer
- **Visualization:** Matplotlib / Qiskit `plot_histogram`
- **Simulation Shots:** 100 shots per experiment
