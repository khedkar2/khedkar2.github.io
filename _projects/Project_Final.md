---
name: Digital Government Database Dashboard - Final Project
tools: [Python, Alteir, Jupyter Notebook]
image: assets/pngs/Hw10.png
description: This is a project to analyse digital goverment database through interactive plots.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Dashboard using Alteir

Group Number: 29

Group Members: Aditya Khedkar Deepak Gajarmal Divyanka Phadtare Sowmya Mamidi

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

The World Bank Group is one of the world’s largest source of funding particularly for developing countries. The WBG is committed to eradicating poverty, sharing prosperity and promoting sustainable development. It is important to understand and analyze significant global efforts.

Digital governance is the application of modern framework technologies to improve government services. Governments at all levels are undergoing digital transformation  in order to deliver government services and programs more efficiently, in a transparent manner, and cost-effectively. Today, digital government transformation has become critical for meeting the expectations of modern citizens. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/Project_Dashboard.json" style="width: 100%"></vegachart>

The dataset was created during examination and recording of project information which was spearheaded by Integrated Digital solutions for all WBG investments. The dataset is classified as Public and comes under the Access to Information Classification Policy. Users inside as well as outside the World Bank have access to the dataset. In terms of metadata - geographical coverage ecompasses different countries around the world and includes all World Bank Group client countries. The granularity list consists of projects. In terms of temporal coverage the dataset spans from 1995 to 2022. Due to limited scope and time constraints, we are considering the Digital Government Projects Database (July 2020). The periodicity represented is annual. The Digital Government Projects Database (July 2020) dataset is basically a snapshot of operations portal data on the relevant World Bank Group funded programs within the specified period. The main source is the World Bank projects database. 

Dashboard Design:

The following dashboard has 4 interactive plots: 1] Bar plot showing number of total projects approved in a year. This plot is helpful to visualize the time-series instance present in the dataset.It is convenient for a user to select range of interested years through x-axis. The rest of the plots will update themselves automatically as per the user selection. 2] Stacked Bar plot showing practice showing sum of total World Bank commitment according to the project status. Each project has 1 of the following status- ACTIVE, CLOSED or PIPELINE.The graph is useful in finding out budgets allocated by World Bank according to the status of the projects for the selected years. 3] The third plot is a scatter plot showing correlation between IDA which is funds allocated by World Bank for e-governance and Net Funds allocated.It can be useful to identify any unusual behaviors in IDA funds. 4] The last plot is a pie chart showing percentages of ACTIVE,CLOSED and PIPELINE projects in given years.This plot is useful for user to priortize their focus according to the status of the project. For instance, if a number of Pipelined projects are greater than a certain threshold then summarized data associated with the projects.


Interactivity:

Each point on the scatter plot represents a location and when the user drags and drops the selected area/point from the scatter plot to the histogram, the pressure distribution of the particular area is plotted on the histogram. We understand the pressure distribution of the particular area through this interactivity.



# Links for data and notebook

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://datacatalog.worldbank.org/search/dataset/0038056/Digital-Governance-Projects-Database" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/khedkar2/khedkar2.github.io/blob/main/python_notebooks/Group23_Project_Part2.ipynb" text="Notebook" %}
</div>