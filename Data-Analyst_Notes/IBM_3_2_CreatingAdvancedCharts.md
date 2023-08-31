
# CREATING VISUALIZATIONS AND DASHBOARDS WITH SPREADSHEETS #

# CREATING ADVANCED CHARTS #

### SUMMARY ###

In this lesson you have learned:

- How to create treemaps, scatter charts, and histograms in Excel.

- About the different charts available in Excel, and how each one is different in displaying data.

- How to create filled map charts and sparklines in Excel.



## Creating TREEMAPS, SCATTER CHARTS & HISTOGRAMS ##

> Now that we've learned how to create basic charts in this video we'll look at how to create some advanced charts in excel. We'll first create tree maps, then scatter charts, and lastly histograms. Please note that the price and resale values in this sample data set are not real and are merely used for  explanatory and demonstration purposes.

- A TREE MAP chart is  used to compare values across hierarchy levels and show proportions within hierarchical levels as rectangles. 
    · Tree maps are a good way of displaying lots of data in one graphical asset because they use the color and closeness of proportional shapes within the chart to represent hierarchical data categories. 
    · Which is a difficult thing to achieve with most other types of chart. 
    
    > In the tree map worksheet of the car sales workbook let's first select the data from two non-adjacent columns model and unit sales. Now let's create a tree map chart with this data we select tree map chart from the hierarchy category of the charts group. We now see a floating chart area containing our tree map chart which displays the proportion of the unit sales of ford cars within hierarchical levels as rectangles. Let's change the chart title to unit sales of ford cars which we can do by simply double-clicking the chart title text box and editing the text. Let's change the chart style to customize the look of the tree map chart there are numerous styles to choose from in the gallery for example here we've chosen style 2. We can easily see from this tree map chart that the f-series model is by far the biggest proportion of our ford car sales. Followed by the explorer and tourist models. which constitute a similar proportion of our ford car sales. While the contour model shows the smallest proportion of ford car sales.


- A SCATTER  CHART is a type of graph used to compare two sets of numerical data values and show relationships between those sets of numerical values. 
    · A scatter chart combines the two sets of values on the x and y axes into single points of data and then displays them in clusters in the chart.  
    · For this reason you will also sometimes see them referred to as xy charts. 
    · Common uses include the comparison of statistical scientific or engineering data values. 
    
    > To create our scatter chart let's first select the data from two adjacent columns price and year resale value in the scatter worksheet of the car sales workbook. Now let's create a scatter chart with this data we select scatter chart from the x y scatter category of the charts group which compares the price of cars from all manufacturers with their year resale value let's change the chart title to comparing price with year resale value, which we can do by simply double-clicking the chart titled text box and editing the text. Let's change the chart style to customize the look of  the scatter chart there are numerous styles to choose from in the gallery for example here we've chosen style 8. Now let's add some axis titles for both the horizontal x-axis and the vertical y-axis. We'll call the horizontal retail price and the vertical year resale value. We can see  from this scatter chart that as the retail price increases so does the differential between the retail price and the year resale value. Generally speaking the lower priced cars retain their resale  value after one year better than the higher priced cars. 


- A HISTOGRAM is a graph that shows the distribution of the data grouped into bins. 
    · Although a histogram  may look like a column or bar chart it's totally different while a bar chart is used to compare data a histogram is used to display distribution of data. 
    
    > To create our histogram let's first select the data from two non-adjacent columns model and price in the histogram worksheet of the car sales  workbook. Now let's create a histogram with this data we select histogram from the statistical category of the charts group. The new floating chart area contains our histogram. Which displays frequency distribution of the price of cars from all manufacturers. Note how excel automatically puts the different price ranges into nine equally sized separate bins for you. The first bin contains cars priced between nine thousand two hundred and thirty five dollars and eighteen thousand six hundred and thirty five. The second bin contains cars priced between eighteen thousand six hundred and thirty five dollars and twenty eight thousand thirty five dollars and so on. Up to a maximum price range of eighty four thousand four hundred and thirty five dollars to ninety three thousand hundred 835. Let's change the chart title to count of car models by price range which we can do by simply double-clicking the chart title text box and editing the text. Let's change the chart style to customize the look of the histogram. There are numerous styles again to choose from in the gallery for example here we've chosen style 3. This style shows the count values of the individual rectangles for each price range   rather than using a vertical scale on the y-axis so from this histogram chart we can easily see that the largest proportion of car models are in the 18635 dollar to 2835 price range. With a count of 62 models in this range, followed by the cheapest price range of 9235 to 18635 dollars which has a count of 42 models and the fewest count of models in a price range is shared by the two most expensive price ranges with only one model in each bin. 
    
    · Although excel chooses your bin ranges automatically when you create a histogram, you can change the bin sizes to suit your needs. This is done by opening the formatting pane for the relevant chart element. In this case the horizontal axis in the axis  options section you can choose to display bins by several factors including bin width and by number of bins. 

    > For example, when we change the bin width value you can now see 15 bins in the chart because the price ranges are much narrower.   Bins 2 and 3 have the two highest counts of 34 and 33 respectively and bin 14 shows no models in this price range at all and if we change the axis options to display a set number of bins then the histogram updates again to show the price ranges split into the number of bins specified. That is 10 bins and once again we can see that bin 2 has the largest proportion of models in its price range and if we choose automatic then the histogram  reverts back to the format we started with.  



## Creating FILLED MAP CHARTS & SPARKLINES ##

> In this video we’ll look at some more advanced charts in Excel. We’ll first create a filled map chart, and then add sparklines to our data, and lastly, we’ll briefly discuss some of the other charts available in Excel. 

- A FILLED MAP chart is a type of chart used to compare values and show categories across geographical regions. 
    · This chart is suitable for data which contains geographical regions like countries, states, or postal codes. 
    
    > In the Map Chart worksheet of the car sales workbook, let’s first copy data from the pivot table containing country of sale and sum of unit sales. Then paste the copied data beside the table. Now let’s create a filled map chart with this data. After selecting the data, we select Filled Map chart from the Map category of the Charts group. The new floating chart area contains our filled map chart, which displays the sum of unit sales of cars across different countries of sale. Let’s change the chart title to “Sum of Unit Sales of Cars by Country”, which we can do by simply double-clicking the chart title textbox and editing the text. 
    > Let’s change the chart style to customize the look of the filled map chart. There are numerous styles to choose from in the gallery to suit your preference. We can see from this filled map visualization that the darker blue color, which denotes the larger number of unit sales, is covering the United States, while the paler blue colors, which denote medium numbers of unit sales, are covering areas such as Canada, Western Europe, and Scandinavia. And the almost-white color, which denotes the lowest number of unit sales, is predominantly covering Eastern Europe, India, Japan, and Australia. 
    
    
- SPARKLINES are mini charts placed inside single cells to represent a selected range of data. 
    · They are typically used to show data trends, such as seasonal increase-decrease, economic cycles, and share, rate, or price fluctuations. They can also be used to highlight max-min values. 
    · A sparkline provides the greatest impact when it is placed close to the data it represents. 
    
    > To create our sparklines, let’s first select data from the 4 adjacent columns, “Unit Sales Q1”, “Unit Sales Q2”, “Unit Sales Q3” and “Unit Sales Q4” in the Sparklines worksheet of the car sales workbook. Now let’s create sparklines with this data. We’ll select the ‘line’ type of sparkline from the Sparklines group. We then need to specify where we would like our sparkline to appear on the worksheet. We can do this by either typing in the cell reference in the Location Range box, or better still just click the cell in the worksheet where you want it to appear and Excel will fill it in for you. Note that it uses an absolute reference by adding dollar symbols to the cell references. And then we can copy that sparkline down the rest of the column. We now see a column containing our sparklines, which displays the trend of the unit sales of Ford cars over the four quarters of a year. Let’s name the column header of the column with the sparklines in as ‘Quarter Sales Trends’. Let’s adjust the column width, and let’s also adjust the row height to display the sparklines more clearly. Let’s also display maximum and minimum values on the sparklines. Let’s change the chart style to customize the look of the sparklines. There are several styles in the gallery for you to choose from. And finally, let’s adjust the weight of the lines in the sparklines to make them stand out a bit. 
    > These Sparklines show us that Ford Escort unit sales started low in the first quarter and then increased in quarters 2 and 3 and then declined again in quarter 4. We can also determine that generally across the majority of the range of Ford car models, quarter 3 is the best quarter for unit sales over the year, with a couple of exceptions such as Mustangs in quarter 4 and Focus models in quarter 2. 
    
    
- Lastly, let’s have a look at some other available charts in Excel:

    - The WATERFALL chart type is used to show cumulative effect of a series of positive and negative values. 
    · This is suitable for data which represents inflows and outflows like financial data. 
    
    - The FUNNEL chart type is used to show progressively smaller stages in a process. 
    · This is suitable for data which shows progressively decreasing proportions. 
    
    - The STOCK chart type is used to show the trend of stock’s performance over time. 
    · This is best suited to data with a series with multiple stock price values like volume, open, high, low, and close. 
    
    - The SURFACE chart type is used to show trends in values across two dimensions in 3-D surface areas or 2-D contoured charts. 
    · This is most suitable when categories and data series are both numeric. 
    
    - The RADAR chart type is used to show values relative to a center point.
    · This is most suitable when categories are not directly comparable.
