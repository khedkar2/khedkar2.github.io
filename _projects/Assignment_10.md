---
name: Vega Lite Homework 10
tools: [Python, Alteir, vega-lite]
image: assets/pngs/Hw10.png
description: This is a project to display interactive plots using python and vega-lite
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Inter-active graphs using vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

This dashboard is useful to find out presseure distribution for specific area. User can select interested area/location within US for analysis.

<vegachart schema-url="{{ site.baseurl }}/assets/json/Interactivity.json" style="width: 100%"></vegachart>
In the above visualization we are trying to depict pressure distribution of a particular location given the latitude and longtitude.

Plot 1:

The first visualization is a scatter plot depicting a relation between latitude and longtitude. Each point in scatter plot represents a particular location. Overlap with Homework 9: some of our group members had worked on the https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv dataset for Homework 9. So we planned to use the same dataset for this assignment as well. We plotted a different graph as compared to Homework 9.

Design choices:

No special design choices are done for the first plot, excecpt setting the height and width.

Plot 2:

The second visualization is a histogram demonstrating pressure distribution. The histogram changes according to the selection in Plot 1. Overlap with Homework 9: There is no overlap with Homework 9 for the second visualization as well.

Design choices: For the second visualization, color is added in the encoding.

Interactivity:

Each point on the scatter plot represents a location and when the user drags and drops the selected area/point from the scatter plot to the histogram, the pressure distribution of the particular area is plotted on the histogram. We understand the pressure distribution of the particular area through this interactivity.



# Links for data and notebook

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/khedkar2/deepakg3.github.io/blob/main/python_notebooks/Assignment_10.ipynb" text="Notebook" %}
</div>