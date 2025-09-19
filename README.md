# Data-Exploration-and-Business-Insights-Using-the-Northwind-Database

## Introduction
This project analyzes the Northwind sample database to uncover customer behavior, product performance, supplier reliability, and forecast future sales. The work focuses on six use cases: top customers, product performance, order trends, supplier analysis, sales forecasting, and profitability analysis.

## Key Findings
**Customers**
- Top customer: B’s Beverages — $6,154,115.34 in total sales.
- Top 10 customers each generated > $5.4M; these customers represent a substantial share of revenue.
- RFM segmentation identified Champions (e.g., Ana Trujillo, Bólido Comidas preparadas) and At-Risk/Hibernating segments for targeted retention programs.

**Products & Categories**
- Top product: Côte de Blaye (Beverages) — $53,265,900 in sales.
- Top category: Beverages — $92,163,180 total sales; followed by Confections and Meat/Poultry.
- Product-level analysis highlights high-revenue and high-profit items to prioritize for promotion.

**Order Trends**
- Yearly sales show growth to a peak then flattening: 2012 = $18.8M, 2015 peak ≈ $41.4M, 2023 = $33.1M.
- Monthly seasonality is present; rolling-average analysis shows short-term fluctuations and longer-term plateauing.

**Suppliers**
- Top supplier by sales: Aux joyeux ecclésiastiques — $56.9M.
- Avg supplier delivery time ~7.8 days; supplier segmentation highlights fast & high-volume suppliers to prioritize.

**Forecasting**
- ARIMA monthly forecast produced MAPE = 8.32% (MAE ≈ 266k). Forecast indicates stable but plateauing sales over the next 12 months.

**Profitability**
- Profitability was simulated (no product cost data in Northwind). Under simulated assumptions top products show positive profits (e.g., Côte de Blaye profit ≈ $21.3M). This result is a limitation—real cost data is required for definitive conclusions.

## Recommendations
1. Prioritize top customers with account management and retention programs.
2. Promote top, high-margin products; review pricing/costs for high-revenue/low-margin items.
3. Negotiate SLAs with top suppliers and move volume to reliably fast suppliers.
4. Integrate monthly forecasting into inventory and procurement planning.
5. Obtain actual cost data and re-run profitability analysis before making pricing or sourcing decisions.

## How to reproduce
1. Clone this repository  
   `git clone <your-repo-link>`
   `cd <repo-folder>`
2. Create and activate a conda environment
   `conda create -n trade_env python=3.11 -y`
   `conda activate trade_env`
3. Install dependencies
   `pip install -r requirements.txt`
4. Launch Jupyter Notebook and open the analysis notebook
   ```jupyter notebook```
   Then run the cells in order.

## Deliverables
- Notebooks: `notebooks/01_exploration.ipynb`, `notebooks/02_forecasting.ipynb`, `notebooks/03_supplier.ipynb`
- Data: `data/raw/` and `data/clean/`
- Visuals: `visuals/` (PNG charts)
- Requirements: `requirements.txt`
