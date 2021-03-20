# Web-Design-Challenge

This exercise is designed to practice the use of HTML and CSS to create a dashboard. The dashboard will present analysis completed in another project.

#### Context about past project###
This project was designed to study the relationship between the location of a particular city and its climate. In order to remove potential bias in the selection process, 500+ cities were selected on random using an existing Python library (https://pypi.python.org/pypi/citipy). Weather data for the selected cities was pulled using the OpenWeather Map API (https://openweathermap.org/api) on February, 9th 2021.

Once assembled, the dataset was used to create several plots using Matplotlib. These plots focused on factors such as maximum temperature, cloudiness, humidity, and wind speed, and compared them to the given city's latitude. The goal being to display trends across the globe and identify the correlation between the latitude and a given factor.
####################################

The dashboard created in this exercise should provide the source data (Resources/cities.csv) and visualizations created as part of the weather analysis, as well as explanations and descriptions of any trends and correlations witnessed. The dashboard will include 7 pages in total and a means to navigate between them. The page breakdown and requirements are as follows:

* A [landing page](#landing-page) containing:
  * An explanation of the project.
  * Links to each visualizations page. There should be a sidebar containing preview images of each plot, and clicking an image should take the user to that visualization.
* Four [visualization pages](#visualization-pages), each with:
  * A descriptive title and heading tag.
  * The plot/visualization itself for the selected comparison.
  * A paragraph describing the plot and its significance.
* A ["Comparisons" page](#comparisons-page) that:
  * Contains all of the visualizations on the same page so we can easily visually compare them.
  * Uses a Bootstrap grid for the visualizations.
    * The grid must be two visualizations across on screens medium and larger, and 1 across on extra-small and small screens.
* A ["Data" page](#data-page) that:
  * Displays a responsive table containing the data used in the visualizations.
    * The table must be a bootstrap table component. [Hint](https://getbootstrap.com/docs/4.3/content/tables/#responsive-tables)
    * The data must come from exporting the `.csv` file as HTML, or converting it to HTML. Try using a tool you already know, pandas. Pandas has a nifty method approprately called `to_html` that allows you to generate a HTML table from a pandas dataframe. See the documentation [here](https://pandas.pydata.org/pandas-docs/version/0.17.0/generated/pandas.DataFrame.to_html.html)

Navigation - Each page must include a navigation menu that meets the following guidelines:

* Has the name of the site on the left of the nav which allows users to return to the landing page from any page.
* Contains a dropdown menu on the right of the navbar named "Plots" that provides a link to each individual visualization page.
* Provides two more text links on the right: "Comparisons," which links to the comparisons page, and "Data," which links to the data page.
* Is responsive (using media queries). The nav must have similar behavior as the screenshots ["Navigation Menu" section](#navigation-menu) (notice the background color change).