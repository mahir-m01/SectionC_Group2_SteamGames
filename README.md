# Steam Games Analytics — Engagement, Popularity & Market Structure

## Project Overview

This project analyzes how pricing models, content structure, platform accessibility, and user feedback influence **game popularity, engagement, and player satisfaction** on the Steam marketplace.

The analysis combines exploratory data analysis, feature engineering, KPI design, and dashboarding to uncover market concentration patterns, engagement drivers, and discovery dynamics across Free-to-Play and Paid games.

The final output includes:

- A cleaned and feature engineered dataset

- A KPI-driven analytical framework

- Interactive dashboards built in Google Sheets

- Business-focused insights and recommendations

---
## Data Source

- **Dataset:** Steam Games Metadata

- **Source:** Kaggle (public Steam data)

- **Original Size:** ~50,000 games

- **Analysis Sample:** ~7,000 games

- **Sampling Method:** Top titles selected based on descending Peak CCU to focus analysis on active and relevant games

---
## Data Cleaning Notes (Summary)


- Removed non-analytical text, media, and metadata-heavy columns

- Standardized data types (dates, currency, percentages, numeric fields)

- Converted array-based fields (languages, genres, platforms) into count metrics

- Normalized platform indicators into Boolean format

- Standardized column naming for consistency

- Filled missing playtime values using column averages (used cautiously in analysis)


All cleaning and preparation steps were executed in **Google Sheets**, as required.

---
## Feature Engineering Highlights

Key analytical columns derived to support deeper analysis:

- **Total Reviews** = Positive + Negative

- **Weighted Sentiment** = `% Positive × ln(Total Reviews + 1)`

- **Pricing Type** (Free-to-Play / Paid)

- **Platform Count** (Windows + Mac + Linux)

- **Popularity Tier** (based on Peak CCU thresholds)

- **Discount Impact** = Discount × Peak CCU

- **Price Band, DLC Band, Recommendation Band**

These fields form the foundation for KPI calculations and segmentation-based insights.

---
## Key Insights (High Level)


- Free-to-Play games show **~5.7× higher average Peak CCU** than Paid titles

- The Steam catalog is **highly skewed**, with over **93% of games classified as Niche**

- A very small number of Blockbuster games generate a **disproportionate share of engagement**

- Higher recommendation volumes strongly correlate with higher Peak CCU (organic discovery effect)

- Multi-genre and content-rich games tend to achieve higher player concurrency

- Higher-priced games generally show **stronger sentiment**, though not broader reach

---
## Dashboard Summary

The dashboard provides an interactive, decision-focused view of the analysis:

- KPI cards for engagement, satisfaction, market structure, and discovery

- Charts segmented by Pricing Type, Popularity Tier, Content Depth, and Social Proof

- Slicers for dynamic filtering (pricing, genre count, popularity tier, DLC band, etc.)

- Dark theme inspired by the Steam desktop interface for visual consistency

- Navigation buttons for smooth movement across analysis sections

---
## Tools & Methods

- **Data Cleaning & Analysis:** Google Sheets

- **KPIs & Pivot Tables:** Google Sheets

- **Dashboarding:** Google Sheets

- **Documentation:** Google Docs → Markdown

- **Version Control:** GitHub

---
## Notes

This README provides a concise overview of the project.

Detailed methodology, formulas, advanced analysis, and business recommendations are available in the **Documentation** and **Presentation** folders.