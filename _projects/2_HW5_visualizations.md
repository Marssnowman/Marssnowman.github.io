---
name: Homework 5 - Illinois Building Visualizations
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Interactive visualizations of Illinois building inventory
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Homework 5: Illinois Building Inventory

## Visualization 1: Building Area by Agency

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_chart1.json" style="width: 100%"></vegachart>

## Visualization 2: Building Year vs. Square Footage

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_chart2.json" style="width: 100%"></vegachart>

## Data and Analysis


### Visualization 1: Building Area by Agency

The first visualization compares the total building area managed by the top 12 Illinois state agencies. I used a horizontal bar chart with quantitative encoding for total square footage and nominal encoding for agency names. The blue color scheme represents building area, with darker colors indicating larger values. In Python, I removed missing and invalid values, grouped the data by agency, calculated the total square footage, and selected the 12 largest agencies. The University of Illinois has the largest total building area among the agencies shown.

### Visualization 2: Building Year vs. Square Footage

The second visualization is an interactive scatter plot showing the relationship between building construction year and square footage. Both axes use quantitative encoding, and the y-axis uses a logarithmic scale to display buildings of different sizes. Building status is represented using different colors. I removed missing and invalid values and randomly sampled up to 1,800 buildings to improve performance. Users can hover over points to view building details and zoom or pan to explore the data. Many buildings were constructed during the second half of the twentieth century. This visualization may be useful for researchers and planners studying Illinois building characteristics.

### Data and Python Notebook

[The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/blob/main/building_inventory.csv)

[The Analysis](https://github.com/Marssnowman/Marssnowman.github.io/blob/main/python_notebooks/HW5_buildings.ipynb)

