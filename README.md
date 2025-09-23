
---

## 🔑 Features

- **Finance Data**: `yfinance` for `.NS` tickers (fallback synthetic OHLCV generator).  
- **News Data**: Mock India-focused news (RBI, SEBI, PLI, ARPU, etc.).  
- **Macro Data**: Mock RBI/NSO series (CPI, WPI, Repo Rate, USDINR).  
- **Evaluator–Optimizer**: Self-reflection + refinement loop to improve reports.  
- **Charts**: Price plots via `matplotlib`.  
- **Export Options**: HTML/PDF reports using `nbconvert`.  

---

## 🚀 Quickstart

1. **Open in Google Colab**  
   Upload `Financial_MultiAgent_Colab_NSE.ipynb` to Colab.

2. **Run All Cells**  
   Example run uses `RELIANCE.NS` (can change to `HDFCBANK.NS`, `INFY.NS`, etc.).

3. **Outputs**  
   - Price chart (6-month close prices).  
   - Draft → Evaluation → Final Research Report.  
   - Persistent notes in `/content/agent_memory_nse.json`.  

---

## 📊 Example Output (RELIANCE.NS)

- **Simple Returns**: 1M, 3M, 6M  
- **News Summary**: Capex in green energy, EPS beat, RBI repo rate hold, SEBI norms  
- **Macro Context**: CPI ~ 4.8%, WPI ~ 2.2%, Repo ~ 6.5%, USDINR ~ 83.6  
- **Evaluator Score**: ~0.85  
- **Final Report**:  
  - Preliminary view on growth in new energy & retail/Jio  
  - Monitor RBI policy meetings, SEBI rules, FPI flows  
  - Risks: regulatory costs, INR depreciation, commodity volatility  

---

## 👥 Team Contributions

- **Pavan Kumar Kallakuri** – *Agent Design & Orchestration*  
  - Designed `InvestmentResearchAgent` (planning, run loop, memory, evaluator–optimizer).  
  - Documentation & architecture.  

- **Sajesh Kariadan** – *Data Integration*  
  - Tool wrappers: `yfinance` (NSE), mock Indian news, RBI macro.  
  - Fallback data generation & plotting.  

- **Pratibha Kambi** – *Workflow Implementation*  
  - Built prompt-chaining NewsAgent, routing logic, evaluator–optimizer refinements.  
  - Reporting structure + export functions.  

---

## 🛠️ Tech Stack

- Python 3 (Colab/Jupyter)  
- `pandas`, `matplotlib`  
- `yfinance` (with `.NS` tickers)  
- `nbconvert` (for HTML/PDF export)  

---

## 📂 Repository Structure

