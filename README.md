# Social Media Content Performance Analytics Dashboard

A self-directed data analytics project simulating the workflow of a Marketing/Data Analyst role at an entertainment company — covering data ingestion, AI-powered sentiment analysis, SQL analysis, time series forecasting, and an interactive Power BI dashboard.

## Project overview

This project analyzes 5,000+ social media posts across 6 platforms (Instagram, Twitter, TikTok, Facebook, LinkedIn, YouTube) to track content performance, engagement trends, and franchise-level KPIs — mirroring real-world social media analytics workflows used by entertainment and media companies.

## Tech stack

- **Python** (pandas, numpy) — data cleaning and transformation
- **SQLite** — relational database for structured querying
- **HuggingFace Transformers** — AI sentiment analysis (RoBERTa model)
- **Statsmodels (ARIMA)** — time series forecasting
- **Power BI** — interactive dashboard and visualization
- **Matplotlib / Seaborn** — exploratory data analysis charts

## Project structure

```
social-media-analytics-project/
├── data/
│   └── social_media_data.csv
├── notebooks/
│   ├── phase1_social_analytics.ipynb       # Data cleaning + AI sentiment
│   ├── phase2_sql_boolean.ipynb            # SQL queries + Boolean filters
│   └── phase2b_arima_forecast.ipynb        # Time series forecasting
├── powerbi_exports/                         # KPI CSVs for Power BI
├── dashboard/
│   └── social_media_analytics_dashboard.pbix
├── charts/                                  # Exported PNG visualizations
└── README.md
```

## Key features

**1. AI-powered sentiment analysis**
Applied a pretrained RoBERTa model (`cardiffnlp/twitter-roberta-base-sentiment-latest`) via HuggingFace Transformers to automatically classify post captions as positive, neutral, or negative — validated against existing dataset labels.

**2. SQL analytics**
Wrote 14 analytical SQL queries covering engagement trends by platform, content type, posting time, release phase, and franchise group performance.

**3. Boolean social listening filters**
Built a custom Boolean query engine in Python supporting AND / OR / NOT logic — simulating social listening tools like Sprinklr for content filtering and classification.

**4. Time series forecasting**
Used ARIMA models to forecast post volume and engagement rate 6 months ahead, with 95% confidence intervals.

**5. Interactive Power BI dashboard**
4-page dashboard with KPI cards, trend charts, a franchise × platform heatmap, and interactive slicers for platform, franchise group, and release phase.

## Key insights

- Identified the highest-performing platform, content type, and optimal posting time for engagement
- Mapped engagement performance across 5 franchise content groups and 4 content release phases
- Forecasted content volume and engagement trends to support proactive content planning

## How to run this project

1. Clone this repository
2. Install dependencies: `pip install pandas numpy transformers torch scipy matplotlib seaborn statsmodels`
3. Open `notebooks/phase1_social_analytics.ipynb` and run all cells
4. Run `notebooks/phase2_sql_boolean.ipynb` to generate SQL analysis and Power BI exports
5. Run `notebooks/phase2b_arima_forecast.ipynb` for forecasting
6. Open `dashboard/social_media_analytics_dashboard.pbix` in Power BI Desktop to view the interactive dashboard

## Author

**Your Name**
[LinkedIn](https://linkedin.com/in/yourprofile) · [Email](mailto:your.email@email.com)
