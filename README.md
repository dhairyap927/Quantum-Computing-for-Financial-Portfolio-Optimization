# 🧮 Portfolio Optimization using Classical and Quantum Methods

This project demonstrates how to solve the portfolio optimization problem using both **classical simulation** and **quantum algorithms (QAOA)**. It explores the **Efficient Frontier**, calculates the **Sharpe Ratio**, and introduces **Qiskit’s quantum optimization tools** for future-ready portfolio selection.

---

## 📌 Project Structure

### 1. **Classical Portfolio Optimization**
- Fetches historical stock data using `yfinance`.
- Calculates:
  - Daily returns
  - Mean returns
  - Covariance matrix
- Simulates **10,000 random portfolios**.
- Evaluates each portfolio using:
  - Expected annual return
  - Annual volatility (risk)
  - Sharpe Ratio (risk-adjusted return)
- Visualizes the **Efficient Frontier** and highlights the optimal portfolio.

### 2. **Quantum Optimization with QAOA**
- Converts the mean-variance optimization problem into a **Quadratic Unconstrained Binary Optimization (QUBO)** form.
- Uses Qiskit’s `PortfolioOptimization` tool to create the quantum-compatible problem.
- Solves using:
  - `QAOA` (Quantum Approximate Optimization Algorithm)
  - Classical optimizer (`COBYLA`)
  - Qiskit `Sampler` (simulator backend)
- Outputs an optimized binary vector that indicates which stocks to include in the portfolio.

---

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

## 📈 Results

- The classical approach provides a full **Efficient Frontier** with thousands of portfolios.
- The optimal classical portfolio is selected using the **maximum Sharpe Ratio**.
- The quantum solution uses QAOA to select a **combinatorially optimal subset of assets**, subject to risk-return constraints.

---

## 📸 Visuals

- Efficient Frontier Plot with Sharpe-colored portfolios
- Optimal Portfolio highlighted with a red star
- Optional QAOA circuit diagram showing the quantum logic used

---

## 🧠 How to Run

1. Install dependencies:
   ```bash
   pip install yfinance pandas numpy matplotlib qiskit qiskit-finance qiskit-optimization
   ```

2. Run the notebook step-by-step in [Google Colab](https://colab.research.google.com/) or Jupyter.

3. To try real quantum backends:
   - Set up an IBM Quantum account.
   - Use `QiskitRuntimeService` with your API token.

---

## 📚 References

- [Modern Portfolio Theory - Harry Markowitz](https://en.wikipedia.org/wiki/Modern_portfolio_theory)
- [Qiskit Documentation](https://qiskit.org/)
- [Quantum Approximate Optimization Algorithm (QAOA)](https://arxiv.org/abs/1411.4028)
