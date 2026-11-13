# Bike-Sharing Analysis

How do annual members and casual riders use a Chicago bike-share service differently? This analysis uses all of 2020's Divvy trip data (about 3.5 million rides) to compare when and how long each group rides, and suggests how to convert casual riders into members.

**Read the report:** https://anushreebhat2001.github.io/bike-sharing-analysis/

## Key findings

- 42% of casual rides happen on weekends, compared with 27% of member rides.
- The median casual ride is 22 minutes, twice the 11-minute median for members.
- Both groups peak in summer, but casual riding is far more seasonal.

## Reproducing it

The report is written in R with Quarto (`cyclistic-analysis.qmd`).

1. Install R (4.1+), [Quarto](https://quarto.org), and the R packages: `install.packages(c("tidyverse", "rmarkdown", "knitr"))`
2. Download the 2020 trip data from https://divvy-tripdata.s3.amazonaws.com/index.html: `Divvy_Trips_2020_Q1.zip` and `202004-divvy-tripdata.zip` through `202012-divvy-tripdata.zip`. Unzip the CSVs into a `data/` folder in this repo.
3. Run `quarto render cyclistic-analysis.qmd`, which writes `index.html`.

Data is provided by Motivate International Inc. under the [Divvy data license](https://www.divvybikes.com/data-license-agreement).
