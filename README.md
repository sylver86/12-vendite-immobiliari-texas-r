# Texas Real Estate Sales Analysis — Descriptive Statistics in R

![R](https://img.shields.io/badge/R-4.x-276DC3?logo=r&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-Visualisation-blue)
![dplyr](https://img.shields.io/badge/dplyr-Data%20Wrangling-orange)

## Overview

Exploratory and descriptive statistical analysis of the Texas real estate market, covering multiple cities over several years.
The analysis extracts actionable insights on price dynamics, sales seasonality, market concentration, and inventory trends — skills transferable to any domain involving time-series market data (energy pricing, asset management, demand forecasting).

---

## Key Findings

| Insight | Detail |
|---------|--------|
| Most variable metric | `median_price` — highest coefficient of variation across cities |
| Most asymmetric distribution | `sales_volume` — strong right skew, driven by seasonal peaks |
| City with highest median price | Bryan/College Station consistently above state median |
| Seasonal pattern | Sales peak in May–July, trough in January–February |
| Market inequality (Gini index) | Moderate concentration in listings across cities (~0.38) |
| Inventory trend | Months of inventory inversely correlated with median price (r ≈ -0.61) |

---

## Analysis Structure

1. **Dataset loading** — `realestate_texas.csv` (city, year, month, sales, median price, listings, months of inventory)
2. **Exploratory analysis** — variable types, central tendency (mean, median), dispersion (SD, variance, CV)
3. **Variability & asymmetry** — identified highest-variability and most-skewed variables with statistical justification
4. **Gini index** — calculated for sales and price variables to measure market concentration
5. **Visualisations** (ggplot2):
   - Box plots: median price comparison across cities
   - Bar charts: monthly and annual sales trends
   - Scatter plots: price vs. inventory relationship
   - Heatmap: seasonal sales pattern by month/year

---

## Dataset

**Source:** `realestate_texas.csv` — Texas real estate market data  
**Variables:** `city`, `year`, `month`, `sales`, `volume`, `median_price`, `listings`, `months_inventory`  
**Coverage:** Multiple Texas cities across several years

---

## Setup

```r
# Install required packages
install.packages(c("ggplot2", "dplyr", "ineq", "knitr"))

# Run the analysis
source("ScriptR.R")
# Or render the full report
rmarkdown::render("Progetto_vendite_immobiliari.Rmd")
```

---

## Technologies

`R 4.x` · `ggplot2` · `dplyr` · `ineq` (Gini index) · `RMarkdown`
