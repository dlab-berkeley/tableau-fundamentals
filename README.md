# D-Lab Tableau Fundamentals Workshop

[![Open Slides](https://img.shields.io/badge/open-slides%20-purple)]
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repository contains the materials for the Tableau Fundamentals workshop. 

Check out D-Lab’s [Workshop Catalog](https://dlab-berkeley.github.io/dlab-workshops/) to browse all workshops, see what’s running now, and review prerequisites.


## Learning Objectives

After this workshop, you will be able to:

- Import data into Tableau Public
- Create a series of basic visualizations including bar sharts and heatmaps
- Connect two visualizations into a dashboard
- Considering publishing open data

This workshop does not cover the following:

- Python connectivity
- Indepth design


## Installation Instructions

Signup for a Tableau Public Account (link to [create an account](https://id.tableau.com/register?clientId=wcS7HwY98qdfgBREHT7Xoln7ipc75U0a))

# Additional Resources

Check out the following resources to learn more about [Workshop topics]:

* [Vizualization fo the Day](https://public.tableau.com/app/discover/viz-of-the-day) - examples of vizualizations using Tableau
* Data & Statistics guide [with UC Berkeley Library](https://guides.lib.berkeley.edu/information-studies/data)
* UC Berkeley Library's [guide to data vizualization](https://guides.lib.berkeley.edu/data-visualization)

# About the UC Berkeley D-Lab and UC Berkeley Library

D-Lab and UC Berkeley Library works with Berkeley faculty, research staff, and students to advance data-intensive social science and humanities research. Our goal at D-Lab is to provide practical training, staff support, resources, and space to enable you to use R for your own research applications. Our services cater to all skill levels and no programming, statistical, or computer science backgrounds are necessary. We offer these services in the form of workshops, one-to-one consulting, and working groups that cover a variety of research topics, digital tools, and programming languages.  

Visit the [D-Lab homepage](https://dlab.berkeley.edu/) to learn more about us. You can view our [calendar](https://dlab.berkeley.edu/events/calendar) for upcoming events, learn about how to utilize our [consulting](https://dlab.berkeley.edu/consulting) and [data](https://dlab.berkeley.edu/data) services, and check out upcoming [workshops](https://dlab.berkeley.edu/events/workshops).



# Contributors

Bee Lehman, Ph.D. (Literatures and Digital Humanities Librarian)

# Lesson Plan
##The End Goal
The end goal of the session is to be able to create a basic Tableau dashboard. Here is an example of a professional dashboard:
![Screenshot of a Tableau dashboard with four viz.](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/DataAfrik-TableauDashboard.jpg?raw=true)

Example: Tobiloba Babajide, “Datafrik Hotel Dashboard,” Tableau Public, January 6, 2025, [https://public.tableau.com](https://github.com/user-attachments/assets/33ff7416-77ce-43a6-8dd4-fcd73d7998ef).

![Screenshot of alternate Tableau dashboard, showing varrying design elements via Starwars themeing.](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/StarWarsTableauDashboard.jpg?raw=true)

Example: Lilla Rasztik, “The Character Network of Star Wars,” Tableau Public, August 6, 2024, [https://public.tableau.com](https://github.com/user-attachments/assets/cbb2f7f2-e911-4a03-b14f-e04bc399edec).

##To get There:
Start by:
Identifying Goals

Thinking about tabular, structured Data
- What is dataset
- Picking a dataset
- Setting up columns and rows

![Screenshot of Tabular data in Excel](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/ExcelCapture-Census.jpg?raw=true)

SAVE THE ORIGINAL 
 - work with a copy
 - 
Using your preferred program:
 - Name your file something identifiable
 - Name your tabs (but easier with single sheet instead of full book)
 - Label your columns

![Screenshot showcasing combining data sheets into single sheet](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/ExcelCapture-Census-singlesheet.jpg?raw=true)

Let's take a look at the census data.
  - [Link to Google Sheet with tabs](https://docs.google.com/spreadsheets/d/1NjDU7KgSFlXDHW5Hm7uw3_NWiX0q9UBsJeFYfkU7qEU/edit?usp=sharing)
  - [Link to Google Sheet with single sheet](https://docs.google.com/spreadsheets/d/1M0LWhsAaPcXOyexzLF2q4GDpVvHrshp9EZkdRp9wV6Y/edit?usp=sharing)

What kind of vizualizations do we want?
 - [Data Visualisation Catalogue](https://datavizcatalogue.com/)

## Uploading the Data
Let's upload the data and get it set up for use.

![Screenshow with arrows showing the Tableau Public data import popup](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/Tableau-addData-marked.jpg?raw=true)

Look at the upper left hand corner of the Tableau Public window. Select the data tab and opt to import data. In Tableau public, there are limited data types you can import. In the professional version, there are significantly more tie-ins for data.

Once you've imported your data, look at the right screen panels and tell Tableau how you want the program to understand your data. You can, for example, tell Tableau that your dates are temporal data and that your geographic columns--including cities, counties, and countries--are geographic data.

[Screenshot of Tableu Public data screen wtih data type drop down menu active](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/Tableau-ImportingData-2.jpg?raw=true)

## Creating Your First Viz: Text Table
Now that we're added our data, let's create our first vizualization by going to "Sheet 1." 

![Screenshot of Tableau Public data screen drawing attention to adding sheets](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/Tableau-Capture-datasourcesandtypes.jpg?raw=true)
The link for sheet one as well as adding additional sheets is located in the bottom, left hand corner of the Tableau window.

Let's start by creating a Text Table (displays tabular data). 
- From your list of types on the left, drag your Year data into column
- Drag your Group into row
- Drag "population count" under the "Marks" box into "Text."

![Screenshot of Tableau window with text table example](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/Tableau-TextTable.jpg?raw=true)

Tableau will automatically aggregate measures (the quantitative data we pulled into "Text"), allowing for rapid summarization of the larger datasheets you uploaded. And, text tables can be phenomenal ways to highlight specific, precise numbers without being overwhelmning. 

We know have our first vizualization. 

## Sheet 2: Bar charts and line graphs

Tableau automatically divisdes data into measures (quantitative data) and dimensions (qualitative data) as we saw above with a focus on measures. They also divide data into discrete and continuous. 

Take a look at your list of column headers on the left hand side of the screen. The data list should be in blue and green, denoating discrete (blue) and continuous (green) data. 
Establishing that your data is discrete or continuous allows you to determine vizualization types and connections between your data. Years, for example, can be viewed as seperatemoments in time  or dates that flow from one to the next. 

![Graph from Tableau's data information displaying their continuous versus discrete categories](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/TableauScreenCapture-continuousvdiscrete.jpg?raw=true).

As you can see from the chart and graph above, the distinction permits different kinds of visualizations. To build a bar chart with our data, we can
- Drag Year to Columns
- Drag Population Count to Rows
- Drag Group to Marks (color)
- Makes sure "Bar chart" is selected under the "Marks" drop down list.

## Vizualization Design
Vizualizations are about communication. To ensure that your vizualizations communicate what you want them to, think about placement, sizes, and color choices after you've decided on the type of vizualization.

Colors
Color choices are incredibly important in vizualizations. First and foremost, you want your colors to contrast or blend in order to convey meaning. Second, you should also think about the cultural implications of different color choices. Red, for example, is viewed as a "happy" color for most of the world and as an "angry" color in some, specific communities. White, in contrast, can mean both death or purity. 

Filters
Sometimes we are working from an enormous data set and we don't want every vizualization to show all of your data. Showing population growth once a decade, for example, might suffice when looking at a century. 
To limit our data, we can "filter" it by dragging our data categories into the "filter" box above "marks."

![Tableau capture of filter popup](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/TableauCapture-Filters.jpg?raw=true)

## Mapping in Tableau
One of my favorite vizualization types are maps. To create a map in Tableau, add geographic data directly into the Sheet, largest first. If in the United States:
- Country
- State
- County
- City



To turn your map into a heat map, you can drag measures into your colors. 
If you want prefer a point map, then you can draw them into categories like lables. 

## Creating a Dashboard
At this point, you should have
- a textual chart
- a bar chart or line graph
- a map of Bay Area counties showing population density or otherwise

Look at the bottom, left hand corner of your Tableau window and click the icon for adding a dashboard (it looks like a four-quadraent quare). 
- Drag Sheets into Dashboard
- Organize your sheets and filters
- Include Objects as desired

![Tableau dashboard screenshow showing different viz and filters.](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/TableauCapture-quickdashboard.jpg?raw=true)

Warning! Changes to the base sheets will be reflected in the Dashboard.

## Publishing
When you're ready, make sure to publish your data. Be aware that Tableau Public will not store drafts and you must publish publically in order to save your material. 

![Tableau window capture with arrow pointing to "publish" button on upper right.](https://github.com/dlab-berkeley/tableau-fundamentals/blob/main/TableauCapture-PublishButton.jpg?raw=true)

Remember! This is a public release of your data. don't use sensative information.

Also, consider cleaning up your dashboard with by:
 - Namng Sheets/Dashboards
 - Run Optimizer

# Questions
Bee Lehman, Ph.D. (Librarian)
beelehman@berkeley.edu
