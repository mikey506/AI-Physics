# Voxel Recursive AGI Simulation Framework

A research-grade, grid-based simulation exploring the emergence of **Artificial General Intelligence (AGI)** from multi-agent, multi-physics interactions inside a dynamic **voxel** environment. The system blends ideas from cellular automata, thermodynamics, quantum mechanics, evolutionary dynamics, reinforcement learning, and predictive world-models—while remaining **Pyodide-compatible** for in-browser execution.

> **License:** Apache-2.0 (permissive, includes explicit patent grant; ideal for open collaboration while protecting contributors). See the **[License](#license)** section.

---

## ✨ Key Capabilities

### Core Dynamics & Physical Models
- **Dynamic Voxel Grid** — 2D grid that scales (grows/shrinks) with emergent complexity (fractal dimension).
- **Cellular Automata Core** — Life-like rules seed complex local/global patterns.
- **Deltic Mechanics & Thermodynamics** — Conceptual internal-combustion/diesel-inspired dynamics affecting efficiency and voxel state.
- **Quantum Thermodynamics** — Quantum-statistical influences on local energy/efficiency.
- **Special Relativity (Conceptual)** — Per-voxel Lorentz factor modulates local interaction cadence.
- **Particle System** — Independent particles interact with voxels, including qubit “flip” events (Particle–Voxel Symbiosis).
- **Energy Conservation** — Global energy budget clamps voxel/particle dynamics when exceeded.

### Quantum & Entanglement
- **Qubits per Voxel** — Each voxel carries a (conceptual) qubit with decoherence, simple circuits, and error correction.
- **Entanglement Propagation** — Diffusion-like spread of entanglement correlations.
- **Quantum Error Correction** — Simplified bit-flip correction for coherence maintenance.
- **Gate Evolution** — Sequences of H, X/Y/Z gates evolve per-step.
- **Quantum Tunneling** — Rare non-local state transitions between distant voxels.
- **QuTiP Subgrid (Optional)** — When installed, a smaller subgrid can run more detailed quantum evolution via QuTiP.

### AI, Learning & Optimization
- **Agentic Voxel Swarms (Actor–Critic)** — PyTorch Actor modulates actions; Critic rewards stability, maze success, and ethics.
- **World Model (LSTM)** — Predicts near-future grid patches; forecasts feed back into current updates.
- **Hybrid Optimizer (Simulated Annealing)** — Anneals NN weights, conceptually inspired by quantum annealing.
- **Multimodal Voxel Communication** — (Conceptual) DistilBERT encodes/decodes voxel patches as an emergent “language.”
- **Reinforcement Learning Influence** — Global Q-learning signal nudges collective behavior.

### Adaptation, Evolution & Safety
- **Self-Healing Diagnostics** — Detects/repairs NaN/Inf via interpolation or zeroing.
- **Adaptive Mutation Rates** — Tuned by biodiversity (Shannon entropy).
- **Evolved Interaction Functions & Constants** — Parameters and pseudo-constants mutate/are selected by global cost.
- **Meta-Recursion** — Rare self-replication events copy internal state (“echo universes”).

### System Control & External Grounding
- **External Data Grounding (Simulated/Optional Real)** — Sine/stock data (via `yfinance` when available) influences dynamics.
- **Vision Modulation (Optional)** — If OpenCV is available, camera input can modulate a key parameter.
- **Ethical Alignment Penalty** — High variance penalized to encourage stable/ethical states.
- **Biodiversity Goals** — Shannon entropy modulates noise/reward to sustain diversity.
- **Fractal Injection** — Mandelbrot dust seeded when diversity collapses.
- **Fractal Dimension & Singularity Horizon** — Complexity analysis guides grid scaling.
- **Time-Reversal Mode** — Roll back to a prior stable snapshot when cost spikes.
- **Multi-Scale Hierarchy** — Super-voxels aggregate/feedback into local updates.
- **Predictive Forecasting** — LSTM-predicted states influence present actions.
- **Misalignment Simulator (Rogue Mode)** — Randomized behavior for a voxel subset simulates internal misalignment.
- **Benchmark Mazes** — A* mazes provide concrete problem-solving checkpoints.

---

## 🧰 Installation

**Prerequisites**
- Python 3.9+ (recommended 3.10/3.11)

**Core dependencies**
```bash
pip install numpy pygame torch
```

**Optional extras**
- **Real data grounding:** `pip install yfinance`
- **Vision modulation:** `pip install opencv-python`
- **Multimodal embeddings:** `pip install transformers`
- **Quantum subgrid:** `pip install qutip`

> **Pyodide note:** In browser (Pyodide), heavy deps (`yfinance`, `opencv-python`, `transformers`, `qutip`) are not available. The simulation auto-switches to **simulated behaviors** and disables file I/O for state persistence.

---

## ▶️ Usage

Run the simulation:
```bash
python engine.py
```

A Pygame window will display the evolving voxel grid and the particle system.

**Keyboard controls**
- `Q` or `Esc` — Quit
- `R` — Toggle **Rogue Mode**
- `T` — Trigger **Time-Reversal Mode**
- `S` — (Conceptual) Save current state (disabled in Pyodide)
- `L` — (Conceptual) Load a saved state (disabled in Pyodide)


---

## 🧭 Architecture Overview (high level)

- **`engine.py`** — Voxel Engine (Core)

> The above modules are a recommended organization for maintainability; adapt to your current file layout as needed.

---

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome! Please:
1. Open an issue describing the idea/bug with reproducible steps.
2. For PRs, include small, focused changes and unit tests where feasible.
3. Agree to license your contributions under the **Apache-2.0** license.

Consider adding pre-commit hooks (formatting, linting) and simple headless smoke tests for CI (e.g., few steps without Pygame).

---

## 🔒 Responsible Use

This is an experimental research simulator. It **does not** implement real-world safety guarantees. Please use responsibly, avoid misuse, and document anomalous behaviors. If you study emergent misalignment, prefer sandboxed environments and deterministic seeds.

---

## 📜 License

**Apache License 2.0** — a permissive license with an explicit patent grant that supports commercial and non-commercial use, distribution, modification, and private use, while protecting contributors and users.

- SPDX Identifier: `Apache-2.0`
- Copyright © 2025 Voxel Recursive AGI Simulation Contributors

You should include a `LICENSE` file with the full text of Apache 2.0. The standard template is available from the Apache Software Foundation.

---

## 🙌 Acknowledgments

- Community projects in cellular automata, PyTorch RL, QuTiP, and Pyodide for inspiration and building blocks.
- Contributors and reviewers who push this framework toward clarity, reproducibility, and insight.

---

## Quick Start Checklist

- [ ] Install Python 3.10+ and `numpy pygame torch`
- [ ] (Optional) Install extras: `yfinance`, `opencv-python`, `transformers`, `qutip`
- [ ] Run `python your_script_name.py`
- [ ] Press `R` to explore **Rogue Mode** and `T` for **Time-Reversal** snapshots
- [ ] File an issue with results, ideas, or anomalies you observe 🎛️
