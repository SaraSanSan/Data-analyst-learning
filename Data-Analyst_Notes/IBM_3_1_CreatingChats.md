
# VISUALIZING DATA USING SPREADSHEETS #

# CREATING CHARTS #

### SUMMARY ###

In this lesson you have learned:

- The importance of charts and how they are able to shape our data.

- How to use visualizations to provide meaningful information.

- How to use Excel to create line, pie, and bar charts.

- About Excel pivot tables in creating area and column charts using the PivotChart feature. 

- How to use a pivot table or pivot chart to filter data and how to expand and collapse data levels.


## INTRODUCTION ##

- It is often said that “a picture is worth a thousand words”. This phrase is especially relevant when it comes to Data Analytics. Data visualization plays an essential role in the representation of both small and large-scale data. 

- This course from IBM is designed to help you tell a compelling story with your data using various visualization techniques. You will work with both Excel and Cognos Analytics to acquire the basic skills needed to create different types of plots, charts and graphs and build interactive dashboards - which are important parts of the skillset required to become a Data Analyst. 

- You will not only learn data visualization techniques using Excel and Cognos Analytics but also practice using multiple hands-on labs and assignments throughout the course. 
    
    · In Module 1 you will learn about different types of charts and the Excel functions that are used to create basic charts and pivot chart visualizations. By learning how to manipulate these features and by creating visualizations, you will begin to understand the important role charts play in telling a data-driven story. 
    
    · In Module 2 you will learn about creating advanced charts and learn the basics of dashboarding and how to create simple dashboards in Excel. You will also learn how dashboards can be used to provide real-time snapshots of key performance indicators. 
    
    · In Module 3 you will learn about Cognos Analytics, including how to sign up for it, how to navigate around it, and how to easily create stunning dashboards. You will also learn some of the more advanced dashboarding capabilities of Cognos Analytics, and make your dashboards interactive. 
    
    · In the final module, you will complete a two-part hands-on final assignment lab, which will guide you on how to create visualizations in Excel, and how to create visualizations and dashboards in Cognos Analytics. This will involve you understanding what the scenario requirements are, and then creating visualizations and a dashboard to fulfil those requirements. 
    
- You will follow two different business scenarios throughout the course, with each using their own dataset; these different scenarios and datasets will be used in the lesson videos and in the hands-on labs. 

- After completing this course, you will be able to explain the Role Visualizations Play in Conveying a Story About Data; create Basic Charts, Pivot Charts, and Advanced Charts in Excel Spreadsheets; create a Simple Dashboard Using Excel.; provision an Instance of Cognos Analytics in the Cloud.; navigate Around the Cognos Analytics Interface and Leverage its Rich Visualization Capabilities; and build Interactive Dashboards Using Cognos Analytics with a Variety of Basic and Advanced Visualizations. You will also perform some intermediate level data visualization and dashboard creation tasks to address a business scenario. 

> The course team and other peers are available to help in the course discussion forums in case you require any assistance. Let’s get started with your next video where you will get an introduction to charts…



## EXCEL KEYBOARD SHORTCUTS ##

Task	Shortcut
Close a workbook	Ctrl+W
Open a workbook	Ctrl+O
Save a workbook	Ctrl+S
Copy	Ctrl+C
Cut	Ctrl+X
Paste	Ctrl+V
Undo	Ctrl+Z
Remove cell contents	Delete
Bold	Ctrl+B
Open context menu	Shift+F10
Expand or collapse the ribbon	Ctrl+F1
Move up one cell in the worksheet	Up arrow key
Move down one cell in the worksheet	Down arrow key
Move one cell left in the worksheet	Left arrow key
Move one cell right in the worksheet	Right arrow key
Move to the edge of the current data region in the worksheet (e.g. end of column)	Ctrl+Arrow key (e.g. Ctrl+Down arrow)
Move to the last cell on a worksheet	Ctrl+End
Move to the beginning of a worksheet	Ctrl+Home
Extend the selection of cells to the last used cell on a worksheet (lower right corner)	Ctrl+Shift+End
Move to the cell in the upper-left corner of the window (when Scroll Lock is On)	Home+Scroll Lock
Move one screen down in a worksheet	Page Down
Move one screen up in a worksheet	Page Up
Move one screen to the right in a worksheet	Alt+Page Down
Move one screen to the left in a worksheet	Alt+Page Up
Move to the next sheet in a workbook	Ctrl+Page Down
Move to the previous sheet in a workbook	Ctrl+Page Up
Edit the active cell and put the cursor at the end of the cell’s contents	F2
Enter the current time	Ctrl+Shift+colon (:)
Enter the current date	Ctrl+semi-colon (;)



## INTRODUCTION TO CHARTS ##

> In this video, we'll give an overview of several different types of charts and visualizations and discuss how they can be used to tell a story. Let's begin by looking at a line chart when comparing different but related datasets. 

- A LINE chart is a great way to display the information. They are able to display trends and show how a data value is changing in relation to a continuous variable. 
    · For example, if time is a continuous variable, how has the sale of a product or multiple products changed? 
    
- A PIE chart can show the breakdown of an entity into its sub-parts and the proportion of the subparts in relation to one another. Each portion of the pie represents a static value or category, and the sum of all categories is equal to a 100 percent. 
    · In this example, we have a Marketing Campaign with four distinct categories. Social Sites, Native Advertising, Paid Influencers, and Live Events. With this type of data representation, we can easily see the total number of leads generated per category. 
    
- A BAR Chart is the most common as they are easy to create and are great for comparing related data sets or parts of a whole. 
    · For example, in this bar chart, we can see the population numbers of 10 different countries and how they compare to one another. We can also use stacked bars in which each bar is divided into sub bars that are stacked end to end. In this stacked bar, we can see the population of each country split into four age ranges. 
    
- Would you like the graph to appear vertical and not horizontal? Then COLUMN charts would be a great pick. This type of chart can be used quite effectively to show change over time and to compare values side-by-side. 
    · For example, showing page views versus user's session time on a website as it changes on a month-to-month basis. 
    
    * While this type of chart looks similar to a bar chart, they cannot always be used interchangeably. For example, a column chart may be better suited for showing negative and positive values. 
    
- Next, we have TREEMAPS, which are useful for displaying complex hierarchies using nested rectangles. 
    · In this example, the treemap depicts statewide employment rates within the population of a country over the last year. The size of the rectangle represents the population and the color represents the employment rate. We can click on any region to see the employment data of the sub-regions within the selected region. 
    
- Trying to display a pipeline or different stages of a continuous process, then FUNNEL charts are the way to go. 
    · In this example, the funnel chart is showing the conversion rate at each stage of the sales process from lead generation to the final sale. 
    
- Another exceptional chart is the SCATTER chart. In this type of chart, the circle colors represent the categories of data and the circle sizes are indicative of the volume of data. 
    · For example, in this scatter chart, we can see each product line by the number of units sold and the revenue it brings. A scatter chart can be great for revealing trends, clusters, patterns, and correlations between data points. 
    
- Next we look at BUBBLE charts. This is a variant of scatter charts, and they are useful for comparing a handful of categories to one another in terms of relative significance. 
    · For example, understanding areas of significant expenditure in an organization's sales budgets. 
    
- Lastly, we have SPARKLINES. Sparklines do not include an axis or coordinates, yet they display trends simply and effectively. These are great for showing the general trend of a variation. 
    · For example, stock market price fluctuations from the opening to the closing of a trading day. 
    

> In this video, we learned about the importance of charts and how they are able to shape our data to provide meaningful information. In the next video, we will dive into more details about how to create and configure different types of charts in Excel.



## INTERVIEW: Using Visualizations to Tell a Data Story ##

> In this video, we will listen to several data professionals discuss the importance of using visualizations to tell a story about data. 

- Can you tell us about the importance of using visualizations to tell a story about data? 

- Visualizations are critical to storytelling with data. I think you're familiar with the phrase, a picture is worth 1,000 words, and that's really true here. You can get a much clearer picture of what's going on, with your data if you have clean and clear data visualizations. I also think data visualization is super helpful for the analysts that creates them, because it forces them to make choices about what's really important to show and what isn't important to show. For example, if you're debating whether you should look at things temporarily, you can debate like, is the overall trend the most important, okay, then I should do a time series data visualization. Do I think comparing one group versus another is more important than you're more likely to do a bar column chart. It's really important in clarifying the data analysts thinking. 

- Visualization is really important in telling a clear, concise story to stakeholders. Humans are visual creatures. You are more likely to tell a compelling story and get buy-in with visuals. I once got a job offer, was a visualized resume created by tableau. One of the best ways to present data is visually. 

- Numbers by themselves, for the most part, will tend to overwhelm people. If I woke up and I'm talking in a company meeting and I say, "Well, last year in 2019, we did $100,000." Or I could give you a graph and say 2018, we did 75,000, 2019, we did 100,000, and 2020 we're projected to do $125,000. If I put them in a graph and make it stand out and make it pretty. Non-accountants will and non-data people will gravitate towards the end it'll prompt them to ask different questions and have different ideas. By using maybe a PowerPoint or even Excel you can create graphs from the data, make it pretty, make sure that it made not just pretty but make sure that it highlights the important information of what you're trying to say. It will create and drive the conversation around what needs to be done and how best to maybe run the business or make different decisions. 

- Data visualization is a very important part of being helping people to understand the numbers that you're trying to present. The reason we want to gravity towards visualizations is that's how the brain really works. Brands much more able to process a high bar versus a low bar as opposed to looking at 100 rows or 100 lines in a spreadsheet. Using the visualizations and especially using the appropriate visualization for the given task can really help make sure that the user gets the easiest way to understand this. 

- As we talks about storytelling is really an important way for us to do this. Through the visualizations, that's really how we tell stories. We can augmented with, text or that's user-generated or system-generated, tell people really drill down further to their understanding. But starting with the visualization is the easiest way to help people quickly, effectively understand what's going on. Then you can have further discussions around what exactly they're doing.



## Creating Basic Charts in Excel: LINE, PIE & BAR CHARTS ##

> In this video we’ll look at how to create  a few basic types of charts in Excel. We’ll first create line charts, then pie charts, and lastly, bar charts.

- A LINE chart is a type of graph, used to show information as a series of data  points connected by straight lines. 
    · In a line chart, the horizontal axis typically represents time or a similar category, and the vertical axis typically represents numerical values. 
    · Because line charts can display continuous data over a given time period, they're perfect for showing trends in data at equal time intervals, such as days, months, quarters, or years. 
    · Line charts are ideal for scenarios where you have data that’s arranged in columns or rows, or where your  data contains multiple data series. 
    
    > On the car_sales worksheet of the Car Sales workbook, let’s first filter the data to display only Ford car models.
    Now let’s create a line chart with this data. We’ll select the data from 2 non-adjacent columns, in this case “Model” and “Price”. 
    Then we select Line chart from the 2-D Line category of the Charts group.
    Let’s change the chart title  to “Price of Ford Cars”, which we can do by simply double-clicking the chart title textbox, and editing the text. We now see a floating chart area containing our line chart, which displays the price trend of Ford cars across its models. Let’s move this line chart  to the left side of the worksheet below our data.


- A  PIE chart is a type of circular graph, used to show the relative contribution of different categories (which we see as slices), to make an overall total (which we see as a pie). 
    · Data points on a pie chart, that is, the slices, are represented as percentages of the complete pie. 
    · Pie charts provide a very simple visualization of differing data results, which we humans find very easy to comprehend. 
    · Pie charts are best used when you only have one data series, and when your data contains no  more than maybe a dozen categories,   otherwise the pie chart can start to look too busy and become difficult to read. 
    
    > For the pie chart, we’ll use the model names manufactured by Ford along with their unit sales.
    To create our pie chart, we’ll select the data from 2 non-adjacent columns; in this case, “Model” and “Unit Sales”.
    Then we select Pie chart from 2-D Pie category of the Charts group. 
    The new floating chart area contains our pie  chart, which displays the relative contribution of unit sales from individual Ford car models, which are the ‘slices’ of the pie, and they combine together to make an overall total of unit sales of Ford cars, which is the whole ‘pie’. 
    Let’s change the chart style to customize the look of the pie chart. There are numerous styles to choose from in the gallery and you can even make combinations of multiple styles; for example, here we’ve chosen style 3 and style 7, which gives us the percentage values displayed in each slice, and a nice dark contrasting background color. Let’s again move the chart, this time to the center of the worksheet below our data.


- A BAR  chart is a type of graph used to compare values across categories either using horizontal bars, or vertical bars in the case of COLUMN charts, which are a variety of bar charts. 
    · In a bar chart, the categories are usually arranged on the vertical axis, and the values are on the horizontal axis.  
    · Whereas, in a column chart, the categories are typically arranged on the horizontal axis, and the values are displayed on the vertical axis. 
    
    > To create our bar chart, we’ll select the data from 2 non-adjacent columns; in this case “Model” and “Retention %”.
    Then we select a style of bar chart from the 2-D Bar category of Bar Charts.
    The new floating chart area contains our bar chart, which displays comparative values for the retention percentage of the different  Ford models using horizontal bars. 
    Again, we can change the chart color to customize the look of the bar chart. If you just want to choose a color scheme based on a palette of colors, rather than a style, you can click the Change Colors button and then select a color palette from the list.
    Let’s also move this chart; this time to the  right side of the worksheet below our data.



## USING THE EXCEL PIVOT-CHART FEATURE ##

> Now that we’ve learned how to create a few basic types of charts in Excel, in this video we’ll look at how to create some other basic charts using the PivotChart feature from a pivot table in Excel. We’ll first create area charts, and then column charts from a pivot table. Please note that the price and resale values  in this sample dataset are not real data, and are merely used for explanatory and demonstration purposes.

- A PIVOT CHART is used to show the data series, categories, and chart axes the same way a basic chart is used, but connecting a pivot table with  it. Simply put, a pivot chart is nothing more than a graphical representation of a pivot table in Excel. 
    · It’s useful when we have a pivot table containing complicated data. A pivot chart can help us make sense of such data. 
    
- Let’s start with area charts. An AREA chart is a type of graph, used to show information as a series of data points connected using  straight lines with a filled area below it. Area charts can handle both positive and negative values like line charts. 

    > First let’s create a copy of the Pivot1 worksheet of the car sales workbook. In this copied worksheet of the car sales workbook, let’s first filter the data of the pivot table to display only Toyota car models. If we expand the field “Toyota”, we can see the details of different models from Toyota, such as the average price of each model, and the average year resale value.
    Now let’s create an area chart using the PivotChart feature with this  data. Here, let’s select the Area chart type, and choose the 3-D Area chart. Here we see a floating chart containing our area chart, which displays the trend of average price as well as average year resale value  of Toyota cars across its models.


- Note, that we can also FILTER the data in the pivot chart itself, rather than in the pivot table; this is one of the key differences between a standard chart and a pivot chart. 

    > So, in our pivot chart, let’s filter the data to display only Chevrolet car models. When we expand the field, the  pivot chart displays our data. Here we can see that it seems that the higher priced models don’t retain their value after one year compared to the lower priced models.

    > We can also use the Model filter drop-down in our pivot chart to filter on models too. 
    Now we are only displaying 7 of the 9 Chevrolet models in our pivot chart and its associated pivot table. So, we can see that when we make a change, such as adding a filter, directly in our pivot chart, those changes are immediately reflected in our pivot table data. And the reverse is obviously also true; if we make a change in our pivot table, that change is immediately viewable in our pivot chart. 
    

- Next, let’s have a look at column charts. A COLUMN chart is a type of graph used to compare values across categories using vertical bars. In a column chart, the categories are  typically arranged on the horizontal axis, and the values are displayed on the vertical axis. 

    > To create our column chart, let’s first create another copy of the Pivot1 worksheet of the car sales workbook.  
    In this copied worksheet of the car sales workbook, let’s again filter the data of the pivot table; but this time to display only BMW, Cadillac and Hyundai car models.
    Now let’s create a column chart using the PivotChart feature with this data. Here, let’s select the Column chart type, and choose the 3-D Clustered Column chart. The new floating chart area contains our column chart, which displays comparative values for the average price as well as the average year resale value for BMW, Cadillac and Hyundai cars using vertical bars. 
    From this chart data, we can see that it seems that both the Hyundai and BMW ranges, retain their one-year resale value better than the Cadillac models do. Now let’s view all the BMW models in the table and chart by expanding the cell in the pivot table. 
    But note that we can also use the plus and minus buttons in the chart to expand and collapse the data view too. These buttons can drill-down and drill-up through multiple category levels if you have multiple fields in the Axis (or ‘Categories’) section of the   PivotChart fields pane; for example if we had the models further categorized into model variants, and then into engine capacities, and then into colors, and so on. Now we can see all the models for all three manufacturers displayed in our column chart. 
    Note, however that these buttons can only be used to expand or collapse all fields. If you want to expand or collapse just one field then you need to do it in the pivot table rather than the chart, as we did in the previous step.
    Let’s change the chart style to customize the look of the column chart. There are numerous styles to choose from in the gallery; for example, here we’ve chosen style 9, which gives us a nice dark contrasting background color.


> In this video, we learned how to create area and column charts using the PivotChart feature from a pivot table in Excel. We also learned how to filter data using either the pivot table or the pivot chart, and we learned how to expand and collapse data levels using both the pivot table and pivot chart. In the next video, we’ll look at some advanced charts available in Excel.
