
## 🛠️ Technologies Used

| Tool        | Purpose                                |
|-------------|----------------------------------------|
| `Python`    | Core programming language              |
| `Pandas`    | Data manipulation                      |
| `NumPy`     | Numerical computation                  |
| `Matplotlib`| Data visualization                     |
| `yfinance`  | Historical stock data                  |
| `Qiskit`    | Quantum algorithms and simulation      |

---

## ▶️ How to Run the Project

### 1. 📦 Install Dependencies (with Version Control)
It is important to install **compatible versions** of Qiskit and other libraries to avoid dependency conflicts:

```
!pip install yfinance pandas numpy matplotlib
!pip -q install qiskit==1.3.1 qiskit-aer qiskit-algorithms qiskit-ibm-runtime pylatexenc
!pip install qiskit-optimization
!pip install qiskit-algorithms
!pip install qiskit-finance --quiet
```

> ✅ These versions are tested and compatible with this notebook setup.

---

### 2. 🚀 Execute the Notebook

You can run this notebook locally with **Jupyter Notebook** or use **Google Colab** for an online execution:

```bash
jupyter notebook Portfolio_Optimization.ipynb
```

Or open directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

### 3. 🔌 Optional: Run on Real Quantum Hardware

- Create an IBM Quantum account at [https://quantum.ibm.com](https://quantum.ibm.com)
- Replace simulator sampler with `QiskitRuntimeService` and set your IBM API token.
- Update backend name (e.g., `"ibm_brisbane"`) in the code.

---

## 📈 Results

- Classical optimization highlights the optimal Sharpe Ratio on the Efficient Frontier.
- Quantum optimization returns a binary selection of assets using QAOA and QUBO formulation.

---

## 📸 Visuals

- Efficient Frontier Plot
- Optimal Portfolio Marker
- QAOA Circuit Diagram (Optional)

---

## 📚 References

- [Modern Portfolio Theory - Harry Markowitz](https://en.wikipedia.org/wiki/Modern_portfolio_theory)
- [Qiskit Documentation](https://qiskit.org/)
- [Quantum Approximate Optimization Algorithm (QAOA)](https://arxiv.org/abs/1411.4028)
