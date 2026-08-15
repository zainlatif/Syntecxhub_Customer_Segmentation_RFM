# Customer Segmentation Using RFM Analysis

A data-driven customer segmentation project using **Recency, Frequency, and Monetary (RFM)** analysis to identify customer value, behavior patterns, and targeted marketing opportunities.

## Overview

This project analyzes retail customer transaction data to segment customers into actionable groups for strategic marketing and retention initiatives.

## Project Structure

```
├── dataset/
│   ├── raw/                    # Original SuperStore_Sales_Dataset.csv
│   └── processed/              # Cleaned data (cleaned_data.csv)
├── notebooks/
│   └── customer_segmentation_rfm.ipynb    # Main analysis notebook
├── src/
│   ├── customer_segmentation.py           # Core segmentation logic
│   ├── data_cleaning.py                   # Data cleaning utilities
│   ├── rfm_analysis.py                    # RFM calculation functions
│   └── visualizations.py                  # Plotting and visualization
├── reports/                    # Generated insights and outputs
└── certification/              # Certification materials
```

## Key Findings

- **Customer Segments**: 6 segments identified (Champions, Potential Loyal, New, At Risk, Lost/Hibernating, Other)
- **Dataset**: 5,901 transactions from 773 unique customers (2019-2020)
- **Total Revenue**: Calculated and profiled by segment
- **At-Risk Customers**: Identified for retention campaigns

## RFM Metrics

| Metric | Description |
|--------|-------------|
| **Recency** | Days since last purchase (lower = better) |
| **Frequency** | Number of unique orders |
| **Monetary** | Total revenue generated |

Each metric scored 1-5, with higher scores indicating greater value.

## Customer Segments & Actions

| Segment | Count | Action |
|---------|-------|--------|
| Champions / Loyal | High RFM | VIP rewards, referral programs |
| Potential Loyal | Medium-High RFM | Cross-sell campaigns |
| New | High R, Low F | Welcome offers, 2nd purchase incentive |
| At Risk | Low R, High F | Reactivation campaigns |
| Lost/Hibernating | Low RFM | Low-cost re-engagement |
| Other | Mixed | Segmented offers |

## Quick Start

1. **Install Dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

2. **Run Analysis**
   - Open `notebooks/customer_segmentation_rfm.ipynb`
   - Execute all cells to generate insights and visualizations

3. **Access Results**
   - Cleaned dataset: `dataset/processed/cleaned_data.csv`
   - Visualizations and reports in notebook outputs

## Technologies

- **Python 3.x**
- **Pandas** - Data manipulation
- **Matplotlib & Seaborn** - Visualization
- **Jupyter Notebook** - Interactive analysis

## Business Impact

- Identify high-value customers for premium experiences
- Prioritize at-risk customers for intervention
- Allocate marketing budget efficiently
- Improve customer retention and lifetime value

## Notes

- Analysis date anchored to maximum order date in dataset
- Negative profit rows retained (legitimate business losses)
- Segmentation thresholds based on RFM score distributions
- Combines behavioral data with strategic business context
