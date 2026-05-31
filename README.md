# Climate Change and Its Effect on Hop Growth

## 📋 Project Overview
This project investigates whether the documented negative impacts of climate change on European hop production—specifically declining yields and essential alpha acid content—are mirrored in the United States. Focus is placed on **Yakima, Washington**, the leading hop-producing region in the country. 

The study leverages historical weather metrics and total agricultural output data from 2000 to 2024 to determine if shifting regional temperature and precipitation patterns are explicitly destabilizing domestic hop yields.

---

## 🛠️ Data Pipeline & Engineering

The study combines environmental telemetry with commercial crop statistics by blending two primary data sources:

1. **Environmental Data (`NOAA NCEI`)**:
   * Gathered localized historical temperature and precipitation datasets.
   * Handled incomplete/missing records across regional reporting metrics by pruning inconsistent reporting stations.
   * Isolated data exclusively from the **Yakima Airport** weather station to ensure measurement uniformity.

2. **Agricultural Telemetry (`USDA NASS QuickStats`)**:
   * Extracted historical hop yields, filtering records exclusively for annual output (measured in pounds) produced in Yakima, Washington.
   * Parsed data elements and compiled environmental variables alongside production figures within an unified `R` working data frame for cross-variable statistical visualization.

---

## 📊 Exploratory Visualizations & Key Findings

Using `ggplot2` in R, the analysis targets specific climate interactions to evaluate long-term trends:

### 1. Macro Climate Trends (Figure 1)
* **Temperature Dynamics**: Over the 24-year historical window, average localized temperatures display a steady upward trajectory, climbing by up to 5°F.
* **Precipitation Volatility**: Total regional rainfall and snowfall exhibit a minor overall downward pattern over time.
* **Indication**: The combined metrics confirm that Yakima is observing measurable localized climate shifts.

### 2. Output Analysis (Figures 2 & 3)
* **Temperature vs. Hop Production**: Production figures remained stagnant until 2005, dropped significantly around 2009, and surged rapidly after 2012. This commercial growth (peaking at 850 million pounds in 2022) correlates directly with the historic explosion of micro-breweries rather than shifting baseline temperatures. 
* **Precipitation Dynamics**: Annual rain and snowfall metrics display minimal direct statistical influence on yield outputs. This indicates that local farms successfully decouple from natural precipitation constraints by heavily utilizing advanced crop irrigation infrastructures.

---

## 💡 Analytical Conclusion

Unlike the clear production drops observed across traditional European hop-growing regions, the empirical data does not support the hypothesis that climate change is actively reducing hop production volume in the United States. 

While temperatures are steadily rising, modern commercial hop output variations are governed by market demand changes—such as the micro-brewery boom—and broader industry demand patterns, rather than localized environmental degradation
