# Airbnb Price Prediction – London

Group project for **Text Mining for Economics & Finance** (TMEF)  
MSc Financial Technology · Imperial College Business School · 2025–26

---

## Overview

This project predicts Airbnb listing prices in London using text-based features extracted from listing descriptions and metadata. We explore n-gram models with LASSO regularisation and word embeddings across ~60,000 London listings.

---

## Data

Data is sourced from [Inside Airbnb](https://insideairbnb.com/get-the-data/).

1. Go to https://insideairbnb.com/get-the-data/
2. Find **London, England, United Kingdom**
3. Download `listings.csv.gz` (the detailed listings file)
4. Place the uncompressed file in the project root as `londonlisting.csv`

> The data files are excluded from this repository via `.gitignore` due to file size.

---

## Project Structure

```
├── Airbnb Price - London copy.Rmd   # Main analysis notebook
├── TMEF_dfm.R                       # Document-feature matrix helpers
├── vectorFunctions.R                # Word embedding / vector functions
├── final project.Rproj              # RStudio project file
├── graphs/                          # Generated plots (excluded from git)
├── londonlisting.csv                # Data file (excluded from git)
└── london.csv.gz                    # Compressed data (excluded from git)
```

---

## Requirements

- R (≥ 4.2)
- Key packages: `tidyverse`, `quanteda`, `glmnet`, `text2vec`, `ggplot2`

Install all dependencies by running the top of the `.Rmd` file, or:

```r
install.packages(c("tidyverse", "quanteda", "glmnet", "text2vec", "ggplot2"))
```

---

## Usage

1. Clone the repo and open `final project.Rproj` in RStudio
2. Download and place the data file as described above
3. Knit `Airbnb Price - London copy.Rmd` to reproduce the full analysis
