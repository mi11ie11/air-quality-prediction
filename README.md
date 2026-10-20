# Dallas Air Quality (Ozone) Prediction

Forecasting daily maximum ozone in the city of Dallas, TX, using EPA monitor data
and weather variables (temperature, wind, pressure, humidity/dew point).

## Getting the data

The raw data (~550 MB) is **not** stored in this repo. Download it and place it in a
`data/` folder next to `final_project.qmd`:

```
data/
├── OZONE/         daily_44201_YYYY.zip
├── TEMPERTURE/    daily_TEMP_YYYY.zip
├── WIND/          daily_WIND_YYYY.zip
├── PRESSURE/      daily_PRESS_YYYY.zip
├── RHDEWPOINT/    daily_RH_DP_YYYY.zip
└── SPENDING_OI/   Affinity - City/County - Daily.csv
```

- EPA AQS daily files: <https://aqs.epa.gov/aqsweb/airdata/download_files.html#Daily>
- Spending data: Opportunity Insights Economic Tracker

## Running

Open `final_project.qmd` in RStudio and click **Render**. Required packages:

```r
install.packages(c("data.table", "ggplot2"))
```

## Collaborating

1. `git pull` before you start working.
2. Make changes on your own branch, then open a Pull Request into `main`.
3. Don't commit anything in `data/` or rendered `.html` files.
