# Quantum-optics-
# 🧠 Electromagnetically Induced Transparency (EIT) Simulation  
### Using the Lindblad Master Equation — *QuTiP Implementation*

This project simulates **Electromagnetically Induced Transparency (EIT)** in a three-level Λ-type atomic system using the **Lindblad master equation** formalism.  
It models realistic **decay** and **dephasing** channels and visualizes both **steady-state** and **time-dependent** quantum dynamics.

---

## 🔬 Features

- Full **Λ-type three-level atom** (`|1⟩`, `|2⟩`, `|3⟩`)
- Includes all major **decay channels**:
  - |3⟩ → |1⟩ (γ₁₃)
  - |3⟩ → |2⟩ (γ₂₃)
  - |2⟩ → |1⟩ (γ₂₁)
- Includes **pure dephasing**:
  - Ground-state dephasing (γ₁₂_deph)
  - Excited-state dephasing (γ₃₃_deph)
- Solves the **Lindblad master equation** using [QuTiP](https://qutip.org)
- Produces:
  - **Steady-state EIT spectrum** (absorption & dispersion vs probe detuning)
  - **Time-dependent simulation** (`mesolve`) showing coherence & population dynamics
- Displays characteristic **EIT transparency dip** and **slow-light dispersion**

---

## 📈 Outputs

- **Absorption** ∝ Im(ρ₁₃)
- **Dispersion** ∝ Re(ρ₁₃)
- **Population dynamics** for |1⟩, |2⟩, |3⟩
- Interactive plots of steady-state and transient evolution

Example results:
- A **transparency dip** (EIT window) appears in absorption.
- The **dispersion curve** shows a steep slope near resonance, illustrating slow light.

---

## ⚙️ Requirements

- Python ≥ 3.8  
- [QuTiP](https://qutip.org)  
- NumPy  
- Matplotlib  

Install dependencies:

```bash
pip install qutip numpy matplotlib

