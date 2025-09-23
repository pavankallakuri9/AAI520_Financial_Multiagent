# 🇮🇳🧠📈 Multi-Agent Financial Analysis System (NSE / India Edition)

> Autonomous agentic AI system for **NSE stock research** using multi-agent workflows.  
> Built for **investment research**, with **prompt chaining, routing, evaluator–optimizer**, and persistent **memory across runs**.  
> Example run: `RELIANCE.NS`.

---

## 📌 Project Overview

This project demonstrates how **autonomous agents** can perform equity research in the **Indian stock market** (NSE).  
The system fetches prices, processes news, contextualizes macro data, routes tasks to specialist agents, and generates a **self-refined research note**.

- ✅ **InvestmentResearchAgent** – central orchestrator (plans → runs → evaluates → optimizes → learns).  
- ✅ **Specialist Agents** – Earnings, News, Market.  
- ✅ **Workflow Patterns** – Prompt Chaining, Routing, Evaluator–Optimizer.  
- ✅ **Memory** – stores lessons across runs (`agent_memory_nse.json`).  
- ✅ **Colab Notebook** – fully runnable with mock data (no API keys required).  

---

## 🏗️ System Architecture


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

##👥 Team Contributions 

**Pavan Kumar Kallakuri – Agent Design & Workflow Implementation**
- Designed InvestmentResearchAgent including planning logic, run loop, and memory keeper.
- Built prompt-chaining NewsAgent and routing logic.
- Led evaluator–optimizer integration and refinement.
- Drafted system architecture and internal documentation.

**Sajesh Kariadan – Data Integration & Reporting**

- Developed tool wrappers for yfinance (NSE), mock Indian news, and RBI macroeconomic data.
- Created fallback data generators and visualizations.
- Implemented reporting structure and export functions (PDF/HTML).
- Managed GitHub repository and version control.


---

## 🛠️ Tech Stack

- Python 3 (Colab/Jupyter)  
- `pandas`, `matplotlib`  
- `yfinance` (with `.NS` tickers)  
- `nbconvert` (for HTML/PDF export)  

---

## 📂 Repository Structure

