<p align="center">
  <img width="200" height="200" src="https://github.com/a-pradono/global_lithium/blob/main/images/header.png">
</p>
<p align="center">
Photo by <a href="https://unsplash.com/@john_cameron?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">John Cameron</a> on <a href="https://unsplash.com/photos/jblWzTQayxs?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
</p>


## Table of Contents

- [I. Introduction](#i-introduction)
- [II. Data and Methodology](#ii-data-and-methodology)
- [III. Results](#iii-results)
- [IV. Conclusions](#iv-conclusions)

## I. Introduction
Lithium is a metallic element that is widely distributed in the earth's crust at low concentrations. Lithium is a highly reactive metal that is used in a variety of applications, including the production of rechargeable batteries for smartphones, laptops, electronic vehicles (EVs), and energy storage systems. The demand for lithium is expected to increase significantly in the coming years, driven by the growth of the EVs market and the need for energy storage systems to support renewable energy. Therefore, it is crucial to ensure that there are enough reserves to meet this need as the demand for lithium rises. See the definition of [reserves](https://pubs.usgs.gov/periodicals/mcs2023/mcs2023-appendixes.pdf) on page 3 from the United States of Geological Survey (USGS). The objective of this project was to understand the global lithium reserves over time by using web scraping to data visualization processes.

## II. Data and Methodology
In this project, the data was retrieved from the USGS National Minerals Information Center website, which is available in this [source](https://www.usgs.gov/centers/national-minerals-information-center/lithium-statistics-and-information). The data frame includes a list of countries and reserves from 1996-2023. As they were obtained from an official website, the information is trustworthy. 

<p align="center">
  <img width="400" height="200" src="https://github.com/a-pradono/global_lithium/blob/main/images/workflow.png">
</p>

The workflow above demonstrates the processes of achieving the objective. First, web scraping is used to automatically extract multiple pdf files from the website. The pdf files were stored in the local path before further analysis. Once the data has been gathered and loaded, the data was cleaned and manipulated to use for usable insights. After pre-processing the data, multiple plots and charts have been made to highlight key insights and trends in the data.

## III. Results
The first figure below, explains the initial condition of the data that was first obtained. In the process of data wrangling, it found the row containing the keyword "United" in the first column and extract all rows below that row. Moreover, all pdf files were extracted and column year was added to indicate which data belong to the sources.  

<p align="center">
  <img width="500" height="200" src="https://github.com/a-pradono/global_lithium/blob/main/images/plot01.png">
</p>

This step involves identifying and correcting or removing any errors in the data frame such as missing values or incorrect values. Some countries including Bolivia, Democratic Republic of the Congo, Namibia, and Russia are dropped since every data was unavailable. This is what the data frame looks like after cleaning and manipulating.

<p align="center">
  <img width="200" height="200" src="https://github.com/a-pradono/global_lithium/blob/main/images/plot02.PNG">
</p>

A time series plot was made to understand the trend in lithium reserves since 1996. In general, the reserves have been increasing over the years, which might have been caused by some progresses in terms of exploration and discovery of lithium deposits, advancements in technology, or government policy. 

<p align="center">
  <img width="500" height="250" src="https://github.com/a-pradono/global_lithium/blob/main/images/plot03.png">
</p>

Based on the stacked bar chart below, there was a significant increase in lithium reserves from 2009 to 20210. Chile was dominated from the 1990s until today's world.

<p align="center">
  <img width="500" height="250" src="https://github.com/a-pradono/global_lithium/blob/main/images/plot04.png">
</p>

In addition, a bar chart race was built to provide valuable insights and might have been useful to industry professionals to make informed decisions. For instance, it can help identify which countries are major players or which ones are emerging. Based on the chart below, the top countries that have major lithium reserves are Chile, Australia, and Argentina in recent date.

<p align="center">
  <img width="500" height="300" src="https://github.com/a-pradono/global_lithium/blob/main/images/plot05.gif">
</p>

## IV. Conclusions
The objective of this project was to understand the global occurrences of lithium reserves over the year using end-to-end data science workflows. The conclusions made from this project are:
  * Web scraping of semi-structured pdf files was quite challenging since footnote can be read as the whole number in the results.
  * Some pdf files were required to define the area coordinates to detect the table data
  * Overall, the lithium reserves have generally been increasing over time and are dominated by Chile, Australia, and Argentina.
