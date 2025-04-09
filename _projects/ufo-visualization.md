---
title: "UFO Sightings Visualization"
excerpt: "A global analysis of 10,000 UFO sightings using Altair and Python"
layout: project
collection: projects
date: 2025-04-06
---

## Visualization 1: Top 10 UFO Shapes

This is a bar chart of the ten most frequently reported UFO shapes from sightings across the globe. I wanted to analyze what shapes people perceive when they see unidentified aerial phenomena across the world and how they describe it. This was interesting because shapes are ambiguous or they use people's imaginations to justify what they've seen - “light,” "disk," "triangle," etc. I wanted to compare if there were any similarities based on how people reported what they saw and the most common differentiations.

I created this chart by ensuring that any rows in which the shape was unknown were eliminated. Then I frequency counted and created a DataFrame of the ten most frequently reported UFO shapes. On the bar chart, I made the shape column the  x-axis and the count the quantitative y-axis. I used a blues colormap to convey report frequency, where darker blues equate to more sightings - this makes it clearer for the user to perceive and comprehend the data given. Tooltips on the right side provide the exact number should someone want to investigate further. Not only was this chart different than HW5, it also was an entirely different data set. 

![Visualization 2](/assets/pngs/visualization-2.png)

---

## Visualization 2: Global UFO Sightings Map

 The second graphic is of a world map overlayed with where 10,000 sampled UFO sightings took place. You can see the notebook to see how I conducted this. This is a strong plot because it's an interactive plot; the user can filter for sightings based on country and year, so they can explore and figure out how and when sightings change over time. I wanted to essentially showcase the sightings over time, in a geographical and chronological sense. I wanted it to also allow for country selection, so I implemented a dropdown filter was constructed using alt.binding_select(). I wanted to also have an intuitive numeric range slider to filter by year, so that was created through alt.binding_range(). But for that to happen, the datetime column used as a field for the slider field was converted to a datetime object and the year generated, allowing users to navigate by year. By filtering by year in addition to country, one can see when sightings happened and where - only to find out certain years had more reported or interesting trends exist in certain countries and not others. The best part about this is that it tells a story - it does a lot of data story telling, holds a narrative, allowing the data to serve as not just as an overview, but of international history and geography of how much we are intrigued by things that you see unidentified in the sky.
 
<iframe src="/assets/pngs/visualization.html" width="100%" height="600"></iframe>

This interactive map highlights the global distribution of UFO sightings from a 10,000-sample dataset.

---

## View the Full Notebook

- [**Open UFO Visualizations Notebook**](https://github.com/aleebe21/aleebe21.github.io/blob/main/_projects/ufo_visualizations.ipynb)
- [**Open the Dataset**](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv)
