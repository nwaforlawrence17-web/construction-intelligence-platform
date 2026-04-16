# 🏗️ Construction Intelligence Platform

A high-performance, executive-grade data product for monitoring multi-country construction project health. This platform ingests messy operational data, normalizes financial metrics across currencies (USD, NGN, KES, GHS, ZAR), and generates a high-fidelity glassmorphism dashboard for strategic decision-making.

## 📊 Core Features

- **Multi-Currency Normalization**: Automated conversion of project budgets and actual costs into a unified USD baseline.
- **Enterprise KPI Engineering**: Real-time calculation of Cost Overrun, Asset Efficiency Ratios, and Delivery Delay Flags.
- **Executive Dashboard**: A premium, single-file HTML interface featuring:
  - Global filters (Geography, Asset Class, Contractor).
  - Glassmorphism design tokens for a professional enterprise feel.
  - Interactive Plotly.js visualizations.
- **Modular Pipeline**: Clean separation of data cleaning, analysis, and orchestration logic.

## 📂 Repository Structure

```text
construction-intelligence-platform/
│
├── data/
│   ├── raw_data.csv         # Original messy operational dataset (2,200+ records)
│   ├── cleaned_data.csv     # Sanitized, USD-normalized production data
│   └── dashboard_data.json  # Sanitized analytics payload for the UI
│
├── scripts/
│   ├── data_cleaning.py     # Module for currency normalization and standardization
│   ├── analysis.py          # Module for KPI engineering and risk profiling
│   └── pipeline.py          # Orchestrator that runs the end-to-end flow
│
├── reports/
│   └── executive_summary.md  # Strategic deep-dive for leadership (CTO/COO)
│
├── dashboard/
│   └── index.html           # The final, production-ready executive dashboard
│
├── assets/
│   ├── styles.css           # Global theme and glassmorphism styling
│   └── template.html        # Source HTML template for automated updates
│
└── README.md                # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Pandas
- NumPy

### Installation
```bash
pip install pandas numpy
```

### Running the Pipeline
To ingest new data and refresh the dashboard:
```bash
python scripts/pipeline.py
```

## 🛡️ Business Impact
- **Risk Mitigation**: Identifies regional leakage nodes (e.g., South Africa representing 33% of portfolio risk).
- **Operational Optimization**: Highlights bottom-performing assets (e.g., Graders at ~69% efficiency) for maintenance intervention.
- **Capital Recovery**: Quantifies strategic savings opportunities in high-variance procurement zones.

---
*Developed for Executive Strategic Analysis.*
