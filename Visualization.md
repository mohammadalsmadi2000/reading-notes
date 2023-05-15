# Data Visualization 

## Introduction
Data visualization is a crucial aspect of data analysis and communication. It involves representing data in visual formats such as charts, graphs, and plots to gain insights, identify patterns, and convey information effectively. In this reading assignment, we explore three popular Python libraries for data visualization: Matplotlib, Seaborn, and Bokeh. We will examine their features, use cases, and understand how to create different types of plots using the Seaborn library. Additionally, we will discuss the role of the Seaborn Cheat Sheet in a Python developer's workflow.

## Key Differences between Matplotlib, Seaborn, and Bokeh
Matplotlib: Matplotlib is a versatile and foundational library for data visualization in Python. It provides low-level control over visualizations, allowing users to create a wide range of plots, including line plots, scatter plots, bar plots, histograms, and more. Matplotlib is highly customizable but can require more code for complex visualizations.

Example: A line plot showing the trend of stock prices over time would be more suitable for Matplotlib.

Seaborn: Seaborn is a higher-level library built on top of Matplotlib. It simplifies the process of creating visually appealing statistical graphics. Seaborn provides a set of high-level functions for creating various types of plots, including relational plots, categorical plots, and distribution plots. It offers aesthetically pleasing default styles and color palettes, making it easier to generate visually appealing visualizations with fewer lines of code.

Example:

* Relational plots: The scatterplot() function in Seaborn can be used to create a scatter plot that shows the relationship between two numeric variables. For example, visualizing the correlation between a car's horsepower and its fuel efficiency.
* Categorical plots: The barplot() function in Seaborn allows creating bar plots that display the relationship between a categorical variable and a numeric variable. For instance, comparing the average income across different education levels.
* Distribution plots: The histplot() function in Seaborn helps visualize the distribution of a single variable. For example, plotting the distribution of heights in a population.

Bokeh: Bokeh is a library primarily used for interactive and web-based data visualization. It is designed to create interactive plots, dashboards, and applications that can be displayed in web browsers. Bokeh emphasizes interactivity, allowing users to explore and interact with the visualizations.

Example: Creating an interactive scatter plot with tooltips that show additional information about each data point would be more suitable for Bokeh.

## Seaborn Plotting Functions
In Seaborn, the main functions to create different types of plots are:

1. Relational plots:
* scatterplot(): Creates a scatter plot to visualize the relationship between two numeric variables. It shows how one variable changes as the other variable changes.
Example use case: Analyzing the relationship between the hours studied and exam scores of students.

2. Categorical plots:

barplot(): Generates a bar plot to represent the relationship between a categorical variable and a numeric variable. It shows the average value of the numeric variable for each category.
Example use case: Comparing the average income across different occupations.

3. Distribution plots:

histplot(): Plots the distribution of a single variable using histograms.
kdeplot(): Estimates and plots the probability density function (PDF) of a continuous variable.
boxplot(): Displays the distribution of a numeric variable across different categories using box-and-whisker plots.
Example use case: Visualizing the distribution of ages in a population.

These functions provide a convenient way to create specific types of plots quickly, reducing the amount of code required
