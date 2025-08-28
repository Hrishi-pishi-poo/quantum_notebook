# quantum_notebook

A hands-on, math-first notebook collection that builds from **linear algebra** → **Fourier/PDEs** → **quantum mechanics** → **quantum computing**.
The goal is to produce a clean public portfolio: derivations, code, and small experiments that show real understanding (and are fun to read).

---

## What’s inside

```
quantum-notebooks/
  ├── 01-linear-algebra/
  │   └── linear_algebra_foundations.ipynb
  ├── 02-fourier-pdes/
  ├── 03-quantum-mechanics/
  ├── 04-quantum-computing/
  ├── data/
  ├── README.md
  └── requirements.txt
```

- **01-linear-algebra**: bras/kets, inner/outer products, projections, Pauli matrices, Hermitian/unitary operators, expectation values, Bloch vector.
- **02-fourier-pdes**: numerical Fourier transforms, convolution, diffusion/Schrödinger warm‑ups.
- **03-quantum-mechanics**: postulates, two‑level systems, spin, uncertainty, simple time evolution.
- **04-quantum-computing**: single‑qubit gates, circuits, measurement, simple simulators (optionally Qiskit/QuTiP).

---

## Setup

### Option A: pip (quick)
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python -m ipykernel install --user --name quantum-notebooks
jupyter notebook
```

### Option B: conda (optional)
```bash
conda create -n quantum python=3.11
conda activate quantum
pip install -r requirements.txt
python -m ipykernel install --user --name quantum-notebooks
jupyter notebook
```

**Requirements** (see `requirements.txt`):
- numpy, scipy, matplotlib, jupyter
- (optional) qutip, qiskit

---

## How to use the notebooks

- Each notebook mixes **derivations** (Markdown/LaTeX) with **executable code**.
- Run top-to-bottom. Cells are small and self‑documented.
- Every notebook ends with a **mini‑project** prompt, so you can commit artifacts to GitHub.

---

## Study path

1. `01-linear-algebra/linear_algebra_foundations.ipynb`
2. Add a short notebook in `02-fourier-pdes` (e.g., numerical Fourier of a Gaussian).
3. Build a spin‑1/2 notebook in `03-quantum-mechanics` (Stern–Gerlach toy model).
4. Do single‑qubit gates and measurement in `04-quantum-computing` (with/without Qiskit/QuTiP).

---

## Contributing / Style

- Keep cells short; prefer **one idea per cell**.
- Derive first, then code. Add references you used.
- Use plain **matplotlib** for plots (no style overrides); one figure per plot cell.
- Name files descriptively (snake_case) and commit often.

---

## License

MIT — use any pieces you like, but a star on the repo would be awesome :)
