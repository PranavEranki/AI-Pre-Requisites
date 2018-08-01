# Why Data Visualization
* Easier to view data trends
* Easier to analyze data
* Easier to detect relationships between features


# Data Types

### Quantitative data:
* Discrete Data is countable data, whole numbers
* Continuous data is non-countable data (ex. income average), any number within a range

### Categorical Data
* Way of categorizing and labeling data into groups

### Ordered data
* Similar to categorical data, but the categories are ordered/ranked
  * Example - population bins
  * Example - class difficulty(hard,easy,etc)

### Time Series data
* Series of data collected via multiple measurements over time
* Has some implied ordering(i.e. data collection times )

# Visual Encoding
Position
* One value along x axis, another along y axis
* Different positions on graph mean different combinations of features
* Good for 2 dimensions

Retinal Variables
* Using size and other viewable features to make your different features on the visualization look different and distinguishable based on numerical data - example would be using different size and color of circles, instead of a point on a graph, to indicate some features.

# Best Visual Encodings
1. Position
2. Length
3. Angle and slope of lines
4. Area

# Exploring and explaining the data

## Preprocess Data
Extract the data from databases, csv files, etc.

Use tools like SQL or Web Scraping.

Then, clean the data - account for missing or unlabeled data, fix formatting, remove unnecessary features, etc.

## Exploring the data
You can use
* Bar Graphs
* Histograms
* Scatter Plots
* Other graph tools

To visualize your data

## Explaining the data
Look through your data - find trends, reasons for trends, and document them. Explain methods used to arrive to your conclusions.

# Data visualization tools spectrum

Visit this [image](https://github.com/PranavEranki/AI-Pre-Requisites/blob/master/images/spectrum.jpg) to see a spectrum of the different data visualization tools on their flexibility vs productivity.


# Figures
## Chart Types
Charts are visual encodings which use data types to portray a relationship.
Scatter Plots
* Normal
* Scatter plots with bubble circles / different colors with a key to represent another dimension or two.

## Basic Figures
* Bar charts
* Scatter plots
* Line plots
* Tables with custom colors and formatting
* Geospatial Plots (Plots for viewing geological data)
* Choropleth (Maps with colors denoting data, plus a key)
* Cartogram (Map distorted to match prominence of each region, might also have different colors)
* Small multiples (Series of similar scaled graphs used to compare data across groups)

# Most used plots
* Line charts
* Bar Charts*
* Scatter Plots
* Histograms

# Distribution Visualization tools
* Histograms for outliers
* Box and Whisker plots - more detailed, provide insight
* Violin Plots - more complicated, need more data
* Strip Charts - less data

# Graph Choosing
[Here](http://extremepresentation.typepad.com/files/choosing-a-good-chart-09.pdf) is an amazing pdf which details how to do some basic graph selection to find some of the best graphs to use for each situation.

# Pre-attentive processing
Detailing important information in ways which are easily distinguishable from the rest of the data, so users can easily pinpoint and understand trends in the important data.

# Color
Use different, bold colors to label your data - always provide a key. Only use color to either denote very hard to find trends, or to depict an entirely new dimension in your data. Do not use unnecessarily.

Also take into account color blindness if unnecessary

## Rules for using color


* Rule #1 - If you want different objects of the same color in a table or graph to look the same, make sure that the background—the color that surrounds them—is consistent.

* Rule #2 - If you want objects in a table or graph to be easily seen, use a background color that contrasts sufficiently with the object.

* Rule #3 - Use color only when needed to serve a particular communication goal.

* Rule #4 - Use different colors only when they correspond to differences of meaning in the data.

* Rule #5 - Use soft, natural colors to display most information and bright and/or dark colors to highlight information that requires greater attention.

* Rule #6 - When using color to encode a sequential range of quantitative values, stick with a single hue (or a small set of closely related hues) and vary intensity from pale colors for low values to increasingly darker and brighter colors for high values.

* Rule #7 - Non-data components of tables and graphs should be displayed just visibly enough to perform their role, but no more so, for excessive salience could cause them to distract attention from the data.

* Rule #8 - To guarantee that most people who are colorblind can distinguish groups of data that are color coded, avoid using a combination of red and green in the same display.

* Rule #9 - Avoid using visual effects in graphs.


# Chart junk
All visual elements that are not necessary for the comprehension of the graph, or distract the user.

Examples:
* Different grid blindness
* Background colors
* Unneeded text or font differences
* Pictures in graphs
* Shading / 3D effects

Remove all chart junk


# Data Integrity

You want to make your data as truthful as possible in its representation. Use constant axis labeling and scale your pictures according to area to keep differences seeming more realistic.
