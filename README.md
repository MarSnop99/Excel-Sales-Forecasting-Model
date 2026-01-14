# Advanced Demand Forecasting (Excel + Solver)

An analytical project comparing the effectiveness of two sales forecasting strategies: **Top-Down** vs. **Bottom-Up**.
The goal was to determine the most cost-effective and accurate method for the "Superstore" retail chain.

## Business Problem
The company required a reliable sales forecast to optimize inventory levels.
**Research Question:** *Is it worth investing time in building complex models for each category separately (Bottom-Up), or is a single aggregated model sufficient (Top-Down)?*

## Methodology and Tools
*   **Engine:** Excel (Holt-Winters Triple Exponential Smoothing).
*   **ETL:** Power Query (cleaning and aggregation of raw transactional data).
*   **Optimization:** **Excel Solver (GRG Nonlinear)** – automated tuning of Alpha, Beta, and Gamma parameters to minimize error.
*   **Success Metric:** MAPE (Mean Absolute Percentage Error).

## Key Business Insights
1.  **Cost Efficiency:** The analysis revealed that the complex Bottom-Up model (summing forecasts from 3 categories) **did not provide an accuracy advantage** over the simpler Top-Down model (MAPE for both was approx. 43%).
2.  **Recommendation:** Adopting the **Top-Down** method is recommended. It achieves the same results with **3x less analyst workload** and a lower risk of operational error.
3.  **IT Implications:** Lower model complexity results in easier maintenance and faster report calculation times.

## File Structure
*   `Conclusion & Comparison` - Executive dashboard comparing the methods.
*   `Forecast_TopDown` - Main aggregated model (optimized via Solver).
*   `Aggregated_Data` - Data after the ETL process in Power Query.
