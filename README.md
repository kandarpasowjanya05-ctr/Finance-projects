# Automated Financial Auditing, P&L Modeling & DCF Valuation Engine

An end-to-end Python pipeline built in Google Colab that automates financial data ingestion, performs ledger control checks, structures monthly Profit & Loss (P&L) trends, and executes a dynamic 5-Year Discounted Cash Flow (DCF) valuation model with sensitivity analysis.

## 🚀 Project Highlights & Impact
* **Automated Trial Balance Verification:** Programmed an automated debit/credit balancing check that successfully validates ledger integrity with zero manual oversight.
* **Ledger Mapping & Safety:** Built a robust mapping validator that flags unmapped account codes in transaction data to prevent dirty data from distorting financial statements.
* **Multi-Sheet Executive Reports:** Designed a pipeline that computes critical KPIs (MoM Growth, Net/Gross Burn Rates, Opex-to-Revenue Efficiency) and exports them directly into production-ready CSV and multi-sheet Excel formats.
* **Scenario & Valuation Engine:** Developed a dynamic "What-If" scenario planner to test Enterprise Value (EV) under variable WACC and Terminal Growth rate structures.

## 📁 Repository Structure
```text
├── data/
│   └── Monthly_DCF.xlsx          # Source ledger & Chart of Accounts
├── notebooks/
│   └── financial_analysis.ipynb  # Main Colab notebook with complete execution
├── outputs/
│   ├── KPI_Summary_Report.xlsx   # Output Excel report with formatted KPI indicators
│   └── KPI_Summary_Report.csv    # Output CSV backup
├── requirements.txt              # Project dependencies
└── README.md                     # Project documentation
📊 Financial Insights Dashboard
1. Historical Performance (Jan - Apr 2026)
Monthly Cash Generation: Achieved an average monthly net cash flow of +$6,175.00, showing strong operational liquidity.
Operational Efficiency: Average Opex-to-Revenue hovered around 47.6%, reaching peak efficiency in March 2026 at 34.2% due to maximum operational leverage.
Cash Burn Safety: Documented an average monthly net surplus of $4,500.00, indicating no immediate capital-burn concerns.
2. Base Valuation Output (DCF Model)
Base Enterprise Value (EV): $670,882.51
Sum of PV of UFCF (Years 1-5): $215,625.88 (32.1% of total value)
PV of Terminal Value: $455,256.63 (67.9% of total value)
Assumptions: WACC = 12.0%, Terminal Growth = 2.5%, discrete 5-year forecast.
🛠️ Technology Stack & Libraries
Language: Python 3
Data Processing: Pandas, NumPy, OpenPyxl (Excel engine)
Visualizations: Matplotlib, Seaborn (Customized grouped bar charts & cumulative trends)
Interactive Display: IPython Styler (Conditional styling and color maps)
⚙️ How to Run Locally
Clone the repository:
git clone https://github.com/yourusername/financial-dcf-automation.git
cd financial-dcf-automation
Install dependencies:
pip install -r requirements.txt
Run the analysis: Open the notebook in Jupyter or Colab to execute the steps interactively.
