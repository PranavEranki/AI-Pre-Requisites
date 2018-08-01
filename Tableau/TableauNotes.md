# These are the notes on using Tableau
No need to know how to code to use Tableau.

Inside Tableau, once you open up a file, you can do many things with it.

* Rename Variables
* Change Variable Types
* Join Tables

## Sheets
Click on sheets in the bottom left.

In sheets, you can map variables to each other by dragging fields from the dimensions and measures tab.

In the Udacity example, we map individual markets to the number of records they sell.

Aggregation
* Tableau automatically aggregates measures based on some variable.
* This could be summing the market per country, or summing the sales per year, etc.

Granularity
* Using more and more features in the marks section helps to visually encode your data, increasing granularity (the level of detail)

### Show me

This can be used to load graph templates which you can add to later.

Can be seen in the top right


## Hierarchies

Splits data, by drilling down into further sections.

Chronological data can automatically be sorted into hierarchies.

Click the [+] symbol on the dimensions data in the top to view a more hierarchical view of the data, split up more based on time. Click the [-] symbol in the same places or in new hierarchy views in the top to go back up the hierarchy of time.


__To make hierarchies manually__ you need to drag subcategories in your data onto a category, name the hierarchy, and accept.



## Filtering
Drag the variable you want to filter by into the filter.

Select how you would like to filter according to that variable(You'll understand better when you see it for yourself).

To further filter by marks, you can drag the attribute you wish to filter by into the marks area. Then, drag it onto the attribute you want to filter by - example would be dragging country onto the color to filter sales by country.

## Dual Axis

Drag measures onto the rows shelf in the top center to get multiple plots - one for column and row 1, and one for the column and row 2.

Then, right click on one of the labels in the rows category and click 'dual axis' to get a dual axis view.






# Creating Dashboards with Tableau

Dashboards are essentially snapshots, which combine multiple sheets together to best exhibit one idea or general trend.

[Here](https://www.tableau.com/solutions/gallery/sales-and-opportunities) is an example of a dashboard from Tableau themselves.

Because I cannot explain these concepts in greater detail through simple words, I have linked a [tutorial](https://www.tableau.com/learn/tutorials/on-demand/building-dashboard) from Tableau on how to build a Dashboard, along with the [documentation](https://onlinehelp.tableau.com/current/pro/desktop/en-us/help.htm#dashboards.html%3FTocPath%3DPresent%2520Your%2520Work%7CDashboards%7C_____0) for building dashboards.
