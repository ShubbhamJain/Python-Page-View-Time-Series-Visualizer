# Page View Time Series Visualizer

<br />

This project is built to visualize time series data using a line chart, bar chart, and box plots. We used use Pandas, Matplotlib, and Seaborn to visualize a dataset containing the number of page views each day on the forum from 2016-05-09 to 2019-12-03. The data visualizations will help us understand the patterns in visits and identify yearly and monthly growth.

Use the data to complete the following tasks:
* Use Pandas to import the data from "fcc-forum-pageviews.csv". Set the index to the "date" column.
* Clean the data by filtering out days when the page views were in the top 2.5% of the dataset or bottom 2.5% of the dataset.
* Create a `draw_line_plot` function that uses Matplotlib to draw a line chart similar to "examples/Figure_1.png". The title should be "Daily Forum Page Views 5/2016-12/2019". The label on the x axis should be "Date" and the label on the y axis should be "Page Views".
* Create a `draw_bar_plot` function that draws a bar chart similar to "examples/Figure_2.png". It should show average daily page views for each month grouped by year. The legend should show month labels and have a title of "Months". On the chart, the label on the x axis should be "Years" and the label on the y axis should be "Average Page Views".
* Create a `draw_box_plot` function that uses Searborn to draw two adjacent box plots similar to "examples/Figure_3.png". These box plots should show how the values are distributed within a given year or month and how it compares over time. The title of the first chart should be "Year-wise Box Plot (Trend)" and the title of the second chart should be "Month-wise Box Plot (Seasonality)". Make sure the month labels on bottom start at "Jan" and the x and x axis are labeled correctly.

For each chart, we make sure to use a copy of the data frame. Unit tests are written under `test_module.py`.

### Development

For development we are using `time_series_visualizer.py` and `time_series_visualizer.ipynb` to write functions and `main.py` to test these functions.

### Testing 

We imported the tests from `test_module.py` to `main.py` for our convenience. The tests will run automatically whenever we run the code written in `main.py`.
