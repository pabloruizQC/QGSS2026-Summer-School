# IBM Quantum Global Summer School 2026 (QGSS 2026)

**IBM Quantum · Qiskit · Summer 2026**

My lab work for the IBM Quantum Global Summer School 2026 — a hands-on progression through quantum computing with Qiskit: the runtime service and primitives, entanglement and GHZ states, the relationship between circuit depth and entanglement, hardware-aware transpilation, and execution on real IBM devices and noisy simulators. Labs were developed and run against IBM Quantum backends (156-qubit devices) and Qiskit fake/noisy simulators.

## Structure

```
my-work/     my completed lab notebooks
reference/   course lecture / episode notebooks (IBM Quantum materials, for reference)
```

## Labs

### Lab 0 — Setup & primitives

| My work      | Summary                                                                                                                                                                                                 |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Lab0.ipynb` | IBM Quantum account setup (API key + instance CRN, `save_account`, `QiskitRuntimeService`), single-qubit circuits, the **Sampler** primitive (H → ~50/50 counts), and the **Estimator** primitive with a single-qubit Z observable (`SparsePauliOp("Z")`). |

### Lab 1 — Entanglement, GHZ states & circuit depth

| My work                | Summary                                                                                                                                                                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `QGSS2026_Lab1.ipynb`  | Building GHZ states and the link between entanglement and circuit depth; naive linear CX chain vs. logarithmic-depth fan-out; topology-aware GHZ construction on line and heavy-hex subgraphs; a BFS spanning-tree GHZ generator scaling to 64 qubits; transpilation for real backends (`initial_layout`, CZ counts, SWAP avoidance); and a naive-vs-efficient fidelity/depth comparison on the **FakeTorino** noisy simulator. |

## Toolbox

Python · Qiskit · Qiskit Runtime (Sampler & Estimator primitives) · Qiskit Aer / fake backends · IBM Quantum (`ibm_fez`, `ibm_marrakesh`, `ibm_kingston`) · NumPy · Matplotlib · NetworkX

## Credit

Lecture / episode notebooks under `reference/` are IBM Quantum Global Summer School 2026 course materials (© IBM Quantum), included for personal reference. Everything under `my-work/` is my own.
