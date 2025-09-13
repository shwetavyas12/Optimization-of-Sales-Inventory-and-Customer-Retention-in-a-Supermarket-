# Optimization-of-Sales-Inventory-and-Customer-Retention-in-a-Supermarket
**Capstone Project for the Post Graduate Diploma in Data Science, IIT Madras.**

This repository showcases the final analysis and strategic recommendations from a capstone project that transformed one year of a supermarket's operational data into a data-driven roadmap for optimizing performance and enhancing profitability.

# 1. The Strategic Challenge
Reliance Smart Point faced three core operational challenges that eroded efficiency and constrained growth, despite a stable customer base:

**Volatile Sales Performance:** Unpredictable revenue streams, particularly during festive seasons, hindered effective financial planning and promotional strategy.

**Inefficient Inventory Management:** A critical imbalance found as frequent stockouts in high-demand categories alongside overstocking of perishables. It resulted in significant lost revenue and product spoilage.

**Declining Customer Engagement:** A noticeable drop in customer footfall and retention, especially following promotional periods, signaled a weakening of customer loyalty.
The objective was to dissect these challenges using advanced analytics and deliver an actionable, high-impact strategy.

# 2. The Analytical Framework
A multi-faceted analytical framework was employed to move from raw data to strategic insight, ensuring each business question was met with the appropriate data science technique.
| Analytical Vertical | Methods & Models Employed | Strategic Purpose |
|---|---|---|
| **Sales Forecasting** | **Time-Series Analysis (Holt's Linear, Damped Holt)**, Naïve Benchmarking, and Backtesting Validation. | To master demand prediction in a high-volatility retail environment. |
| **Product Strategy** | **ABC Analysis**, **Contribution vs. Growth Matrix**, and **Coefficient of Variation (CV)** for demand stability. | To segment products by financial impact and predictability, guiding strategic resource allocation. |
| **Profitability Analysis** | **Margin vs. Sales Quadrant Analysis** and **Linear Regression** to model the profit-volume relationship. | To identify drivers of true profitability and prevent margin erosion from discounting. |
| **Inventory Efficiency** | **Days of Holding (DOH) Analysis** for perishables and **Pearson Correlation** to link holding times with sales. | To minimize spoilage and perfect the turnover cycle for fresh produce. |
| **Stock Availability** | **Service Level Monitoring** against an 80% on-shelf availability benchmark. | To eliminate revenue leakage from stockouts and solidify customer loyalty. |

**Tech Stack:** Python, Pandas, Matplotlib, Seaborn, Statsmodels, adjustText

# 3. Data-Driven Insights
The analysis surfaced four critical findings that became the foundation for the strategic recommendations.

**Insight 1: Standard Forecasts Fail to Capture Festive Demand Surges**

Linear models were incapable of accurately predicting the October sales spike, while the Damped Holt model proved superior in modeling seasonal trends without over-forecasting.

**Insight 2: High Volatility in Key Categories Creates Significant Stocking Risk**

Fruits and Beverages were identified as high-volatility categories (high CV), making them prone to forecasting errors. This contrasted sharply with the stable, predictable demand for Staples and Dairy.

**Insight 3: Overstocking Perishables Creates Cost Without Benefit**

The analysis proved that extended holding periods for vegetables had a negligible correlation to sales (r=0.04), confirming that overstocking directly increased spoilage risk with no corresponding revenue benefit.

**Insight 4: Stockouts in Key Categories Cause Direct Revenue Leakage**

Consistently failing to meet the 80% stock availability threshold in the Fresh & Frozen Foods category directly correlated with suppressed sales, representing a clear, measurable loss of daily revenue.

# 4. SMART Recommendations & Business Impact
The insights were translated into a set of specific, measurable, and actionable recommendations designed for immediate implementation and impact.

| Focus Area             | SMART Recommendation                                                                                                                        | Projected Business Impact                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Sales Forecasting** | **Deploy the Damped Holt model for all quarterly forecasts**, retraining it each quarter to master seasonal shifts.                             | Minimize overstock and lost sales through precise demand-supply alignment.                                |
| **Inventory Turnover** | **Cap weekly Days of Holding (DOH) for Vegetables at 2.5 days** and implement automated alerts for low stock.                                 | Drastically reduce spoilage costs and elevate customer trust with a guaranteed freshness proposition.      |
| **Stock Availability** | **Raise stock availability in Fresh & Frozen Foods to ≥85% by Q3 2025** using proactive, data-informed restocking.                             | Maximize revenue capture and fortify customer loyalty by ensuring critical products are always available. |
| **Profitability** | **Replicate successful, high-margin promotional campaigns** from Q2 and Q3 during the historically low-margin Q4 festive season.                | Achieve sustainable, profitable growth by decoupling revenue spikes from margin erosion.                  |

