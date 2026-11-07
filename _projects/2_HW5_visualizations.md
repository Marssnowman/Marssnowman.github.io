---
name: Homework 5 - Bigfoot Sighting Visualizations
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Interactive visualizations of Bigfoot sighting reports
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Homework 5: Bigfoot Sighting Reports

## Visualization 1: Bigfoot Sightings by Season and Classification

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_bigfoot_chart1.json" style="width: 100%"></vegachart>

### Visualization 1 Analysis

The first visualization is a heatmap showing the number of Bigfoot sighting reports across different seasons and report classifications. I used nominal encoding for both season and classification, while color intensity represents the number of reports. The Viridis color scheme makes it easier to compare report frequencies, with brighter colors indicating larger counts. In Python, I removed missing values and filtered the data to include Winter, Spring, Summer, and Fall. The visualization shows that Class A and Class B reports are more frequent during the summer, while Class C reports are relatively uncommon.

## Visualization 2: Bigfoot Sightings by Year and Classification

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_bigfoot_chart2.json" style="width: 100%"></vegachart>

### Visualization 2 Analysis

The second visualization is an interactive line chart showing how Bigfoot sighting reports vary over time. The x-axis represents the year, while the y-axis shows the number of reports. Different colors distinguish Class A and Class B reports. In Python, I converted the date column into datetime format, extracted the year, removed missing values, and filtered the dataset to years between 1990 and 2022. The chart includes an interactive dropdown menu that allows users to select different seasons and compare reporting patterns. Users can also hover over data points to see the year, classification, and number of reports. This interactivity makes it easier to explore seasonal differences and changes over time.

## Data and Analysis

[The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/blob/main/bfro_reports_fall2022.csv)

[The Analysis](https://github.com/Marssnowman/Marssnowman.github.io/blob/main/python_notebooks/HW5_bigfoot_final.ipynb)
