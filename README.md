# TexasRealty — Analisi Statistica del Mercato Immobiliare (R)

![R](https://img.shields.io/badge/R-4.x-276DC3?logo=r&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-Visualizzazione-blue)
![dplyr](https://img.shields.io/badge/dplyr-Data%20Wrangling-orange)
![Statistics](https://img.shields.io/badge/Statistics-Descrittiva-green)

## Panoramica

Analisi esplorativa e statistica descrittiva del mercato immobiliare texano su più città e anni. Il progetto estrae insight azionabili su dinamiche dei prezzi, stagionalità delle vendite, concentrazione di mercato (indice di Gini) e inventario — con tecniche statistiche trasferibili a energy pricing, demand forecasting e market intelligence in qualsiasi settore con dati di mercato time-series.

## Valore Enterprise

| Settore / Azienda | Rilevanza |
|-------------------|-----------|
| Energy & Utilities (Enel, Terna) | Tecniche di analisi stagionale applicabili a energy pricing e demand forecasting |
| Financial Services | Market analysis, asset valuation, risk assessment |
| IT Consulting (Accenture, NTT Data) | EDA e statistica per clienti di qualsiasi settore |
| Retail & Real Estate Analytics | Pattern di stagionalità e concentrazione di mercato |

## Findings Principali

| Insight | Risultato |
|---------|-----------|
| Metrica più variabile | `median_price` — CV più alto tra tutte le variabili |
| Distribuzione più asimmetrica | `sales_volume` — forte skew destro (picchi stagionali) |
| Stagionalità vendite | Picco maggio–luglio, minimo gennaio–febbraio |
| Correlazione prezzo/inventario | r ≈ -0.61 (inversa — meno inventario, prezzi più alti) |
| Gini index vendite | ~0.38 — concentrazione moderata tra città |
| Città con prezzo mediano più alto | Bryan/College Station consistentemente sopra la mediana statale |

## Analisi Condotte

| Analisi | Tecnica R |
|---------|-----------|
| Tendenza centrale e dispersione | mean, median, SD, CV per variabile |
| Variabilità e asimmetria | Coefficiente di variazione, skewness |
| Indice di Gini | Concentrazione vendite e prezzi — `ineq` |
| Visualizzazioni | Boxplot, barplot mensili/annuali, scatter, heatmap stagionale |
| Correlazione inventario-prezzo | Pearson r sul dataset completo |

## Setup

```r
install.packages(c("ggplot2", "dplyr", "ineq", "knitr"))
source("ScriptR.R")
# oppure rendering completo:
rmarkdown::render("Progetto_vendite_immobiliari.Rmd")
```

## Stack Tecnologico

`R 4.x` · `ggplot2` · `dplyr` · `ineq` (Gini index) · `RMarkdown`

---

---

# TexasRealty — Texas Real Estate Market Statistical Analysis (R) 🇬🇧

![R](https://img.shields.io/badge/R-4.x-276DC3?logo=r&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-Visualisation-blue)

## Overview

Exploratory and descriptive statistical analysis of the Texas real estate market across multiple cities and years. Extracts actionable insights on price dynamics, sales seasonality, market concentration (Gini index), and inventory — with techniques transferable to energy pricing, demand forecasting, and market intelligence in any sector with time-series market data.

## Key Findings

| Insight | Result |
|---------|--------|
| Most variable metric | `median_price` — highest CV across all variables |
| Most skewed distribution | `sales_volume` — strong right skew (seasonal peaks) |
| Sales seasonality | Peak May–July, trough January–February |
| Price–inventory correlation | r ≈ -0.61 (inverse: less inventory → higher prices) |
| Gini index (sales) | ~0.38 — moderate market concentration across cities |
| Highest median price city | Bryan/College Station consistently above state median |

## Analyses Conducted

| Analysis | R Technique |
|----------|-------------|
| Central tendency & dispersion | mean, median, SD, CV per variable |
| Variability & asymmetry | Coefficient of variation, skewness |
| Gini index | Sales and price concentration — `ineq` |
| Visualisations | Boxplots, monthly/annual bar charts, scatter, seasonal heatmap |
| Price–inventory correlation | Pearson r on full dataset |

## Setup

```r
install.packages(c("ggplot2", "dplyr", "ineq", "knitr"))
source("ScriptR.R")
# or full report:
rmarkdown::render("Progetto_vendite_immobiliari.Rmd")
```

## Technologies

`R 4.x` · `ggplot2` · `dplyr` · `ineq` · `RMarkdown`
