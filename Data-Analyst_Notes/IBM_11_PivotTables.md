
# ANALYZING DATA USING SPREADSHEETS #

# USING PIVOT TABLES #

### SUMMARY ###

- Pivot Tables:

    · To obtain usable and presentable insights into your data you need to use Pivot Tables. 

    · Pivot tables provide a simple and quick way to summarize and analyze data, to observe trends and patterns in your data and to make comparisons of your data. 

    · Pivot tables are dynamic, so as you change and add data to the original dataset on which the pivot table is based, the analysis and summary information changes too. 

    · A Data Analyst can use pivot tables to draw useful and relevant conclusions about, and create insights into, an organization’s data in order to present those insights to interested parties within the company. 


- Use this Pivot Table checklist to ensure your data is in a fit state to make a Pivot Table: 

    · Format your data as a table for best results.

    · Ensure column headings are correct, and there is only one header row, as these column headings become the field names in a Pivot Table.

    · Remove any blank rows and columns, and try to eliminate blank cells also.

    · Ensure value fields are formatted as numbers, and not text, and ensure date fields are formatted as dates, and not text.

    · Arranging Pivot Tables with Filters and Recommended Tables:

    · You use the Pivot Table Fields pane to add and arrange data fields in your pivot table. 

    · Recommended Pivot Tables are a list of suggested different combinations of data that could be used when creating a Pivot Table, based on the data selected in the worksheet. 


- Filters and Slicers:

    · Slicers are on-screen graphical filter objects that enable you to filter your data using buttons, which makes it easier to perform quick filtering of your pivot table data. 

    · Timelines are another type of filter tool that enable you to filter specifically on date-related data in your pivot table. This is a much quicker and more effective way of dynamically filtering by date, rather than having to create and adjust filters on your date columns. 



## CREATING PIVOT TABLE SIN EXCEL ##

> Now that we’ve learned how to use the VLOOKUP and HLOOKUP functions, in this video we’ll look at how to create and use Pivot Tables in Excel. We’ll first look at how to format our data as a table, then how to create Pivot Tables and use fields in a Pivot Table to analyze data, and lastly we’ll see how to perform calculations in a Pivot Table. 

- Having a worksheet full of informational data is all very well, but to really get some use out of it we need to analyze it from different perspectives to find answers to questions related to the data. Now, we’ve already used features such as filters and formulas to draw mathematical and logical conclusions about our data but not all questions can be answered easily using filters and formulas alone. In order to obtain usable and presentable insights into your data you need something else… and that something else is Pivot Tables. 

- PIVOT TABLES provide a simple and quick way, in spreadsheets, to summarize and analyze data, to observe trends and patterns in your data and to make comparisons of your data. A Pivot Table is dynamic, so as you change and add data to the original dataset on which the Pivot Table is based, so the analysis and summary information changes too. 

- A Data Analyst can use Pivot Tables to draw useful and relevant conclusions about, and create insights into, an organization’s data in order to present those insights to interested parties within the company. 

- Before you start to create a Pivot Table in Excel, it can be very helpful to first format your data as a table. The reason for this is not only to make it more organized and defined and to add table styles to your data, but primarily it makes it a lot easier when adding records to the dataset. 
    > In the car sales worksheet, let’s first select any cell within the data, and then on the Home tab, in the Styles group, choose ‘Format as Table’. Then choose a style from the gallery… note that Excel automatically knows the boundaries of our data range, but we can change this if we need to. And ensure you select ‘My table has headers’, if indeed it does. After you click OK and the data has been formatted as a table, note the filter drop-downs at the top of each column – these are automatically added when you format as a table. If we now scroll down to the bottom of the table… and start adding another row of data for another vehicle… when you click Tab or Enter, note that it is automatically formatted and included as part of our table. 
    
- OK, now let’s see how to create a basic Pivot Table, and how to use fields to arrange data in a Pivot Table. Just before we do that, there are a few things you should use as a checklist to ensure your data is in a fit state to make a Pivot Table from, and these are: 
    · Format your data as a table for best results.
    · Ensure column headings are correct, and there is only one header row, as these column headings become the field names in a Pivot Table Remove any blank rows and columns, and try to eliminate blank cells also.
    · Ensure value fields are formatted as numbers, and not text.
    · Ensure date fields are formatted as dates, and not text In the worksheet, we can just select any cell in the table. 
    
- Then, on the Insert tab, we click PivotTable. Note that in the ‘Select a table or range’ box, the table name – Table1 – is already entered for us. If we hadn’t just formatted this data as a table, we would specify the cell range here instead. 

- Under that, we need to decide whether we want to create the Pivot Table on a separate new blank worksheet, or on this worksheet – a new worksheet is the default – and is the most commonly used option. So, a new blank worksheet opens, displaying some basic Pivot Table instructions in the graphic on the left of the worksheet, and a ‘PivotTable Fields’ pane on the right. You can rename the worksheet for the Pivot Table if you wish. 

- To build the Pivot Table report we need to add some fields from the top of the PivotTable Fields pane, to one or more of the sections in the bottom part of the pane. 
    > For example, if we want to find out the total sales for each model of car, let’s drag the Manufacturer field to the Rows section of the report, and then we’ll drag the Model field there too. But this isn’t really the way we want it to look, so we’ll drag the Manufacturer field to appear at the top of the Rows section above the Model, which makes more sense with our data. Next, we’ll add the Price field to the Columns section, but again that really isn’t the way we want to view the data, so we’ll drag Price to the Values section instead, which makes a lot more sense and looks a lot better. Next, we’ll add the Unit Sales field to Values too, so now we can see both the individual price for each model and the number of unit sales of each model. Let’s add the Vehicle-type field to Columns, but that doesn’t seem very useful, so let’s remove that field, which we can do in two ways. 
        * Either by using the drop-down menu or, if we undo that, we can also do it by simply dragging the field out of the Columns section, either to the left over the worksheet, or to the top over the fields list above. 
        
- Let’s now look at how to perform a simple CALCULATION in a Pivot Table. 
    > If we look in the ‘Sum of Price’ column in our Pivot Table, we can see that the figures are formatted as General. So first, let’s change the format for these figures to US currency. This can be done by modifying the value field settings for the field in the relevant section of the PivotTable Fields pane. We’ll format the field as US dollars and show no decimal places.

    · Next, we’ll add a calculated field from the ‘PivotTable Analyze’ tab, using the ‘Fields, Items & Sets’ button. 
    > We want this field to calculate the total sales for each model by multiplying the price by the number of unit sales. When we create and add this formula, it gets added to the PivotTable Fields pane, as a field called Total Model Sales. And we can change the format to make it US dollars again. A new column called ‘Sum of Total Model Sales’ has now appeared in the Pivot Table in our worksheet. In row 5 we can see that there have been over 360 million dollars of sales of the Acura Integra model, and in row 7 we can see that there has been over a billion dollars in sales of the Acura TL model.

  
> In this video, we learned how to format data as a table, how to create a Pivot Table and use fields to analyze data in a Pivot Table, and how to perform calculations using Pivot Table data. In the next video, we’ll look at some other features of Pivot Tables.



## PIVOT TABLE FEATURES ##

> Now that we’ve learned how to create and use Pivot Tables in Excel, in this video we’ll look at some other features that we can use with Pivot Tables, including Recommended Pivot Tables, Filters, Slicers, and Timelines. 

- First, let’s look at RECOMMENDED Pivot Tables, which isn’t exactly a feature as such; it’s really more of a list of suggested different combinations of data that could be used when creating a Pivot Table. These recommendations are based on the data we select in the worksheet, and they are a great way to get started creating Pivot Tables if you don’t have much experience with them yet. 

    > For example, in the vehicle toy sales worksheet, if we select column B, which contains data about the quantity of items ordered, when we choose Recommended Pivot Tables from the Insert tab, then we are presented with a list of potential data combinations related to the order quantity information. However, if we select column F, which contains Order Size information, then the recommended pivot table list changes to reflect that data. And if we select column E, which contains sales information, then the pivot tables recommended are related to sales data. 
    > Let’s select the third one down, which is the sum of sales by territory; because that sounds like something we could get some useful insight from, by presenting it in a pivot table. Note that a new worksheet is opened containing the recommended pivot table, and a new pane opens on the right, called PivotTable Fields. Let’s rename the worksheet to something more meaningful. In the PivotTable Fields pane, you can see that some fields have already been added to the Rows and Values areas. 
    
    · Although it’s a recommended pivot table, we can still make it our own, by adding more fields for example. 
    > So, let’s add the Productline item to the Columns area using drag and drop. Now we have columns for each of the product lines in our pivot table, such as motorcycles, ships, and trains. In the pivot table, we can manually expand any field we want to view its contents. Here we can see that the order dates are located underneath the territory names in our pivot table. Note that this matches the order of the fields in the Rows area of the PivotTable Fields pane. We can manually collapse each of the fields too. But we also have the option of expanding all the fields at once, and collapsing them all too.
    

- The next feature we will delve into is pivot table FILTERING. Pivot table filters work in much the same way as the standard filters we used earlier in the course. Note that we already have some in-built filtering in this pivot table.

    > For example, the Row Labels header is a filter, and we can filter on any of the listed territories, such as Japan. Just like standard filters, it’s very simple to clear a filter in a pivot table. We also have a Column Labels filter, allowing us to filter on any of the productline items in this pivot table; for example we could show data only for the trains product. We also have the option of adding the Productline field as a standard filter instead of a column heading, by dragging it to the Filters area in the PivotTable Fields pane. 
    > And we can then use it as a standard filter, as we have done earlier in this course. The filter also allows us to select multiple filter items. But because it is now being used as a standard filter rather than a column header, we can’t see the split of the information on these two product lines; we just see a combined total. When we had the filter as a column header, the information on each product line was presented separately in each column. Let’s display all the field totals again. And we’ll drag the productline field back to the Columns area where it was previously, so we can see the split of our different product lines in the pivot table. 
    
    
- The next pivot table feature we will look at are SLICERS. Slicers are essentially on-screen graphical filter objects that enable you to filter your data using buttons. Slicers make it easy to perform quick filtering of your pivot table data, and they also display the current filter state, making it easier for you to know, and see, what data is currently being shown, and which is being hidden, by the filter. 

    > For example, if we remove the productline field from the pivot table by dragging it out of the PivotTable Fields pane, and then from the PivotTable Analyze tab, we click Insert Slicer, and then choose the Territory field as our slicer, we can see that the slicer can be freely moved around anywhere on the worksheet, and it contains buttons for each of the territory items, such as EMEA, North America, and Japan. 
    > We can also select the Multi-Select button to filter on multiple territories if we wish. We can click the Clear Filter button to clear all slicer filters. 
    > Let’s add another slicer to our worksheet for the productline field. However, be sure to select a cell in the pivot table first, because if you don’t, then the insert slicer button won’t work. 
    
    · Note that slicers can also be added from the Filters group on the Insert tab as well as from the PivotTable Analyze tab. 
    > We’ll select the Productline field this time for our slicer, and drag it near the top of the worksheet. As before, we can select only one slicer item, or we can turn on Multi-Select and choose several items to filter on in the slicer. Then let’s clear the slicer filters,and now let’s filter using both slicers. 
    
    · Note that when you use multi-select filtering, when you select an item, you are in fact filtering it out; that is, you are defining which items will NOT be displayed in the pivot table. This is the opposite behavior to when you are selecting single items in a slicer. 
    > So now we are displaying only ‘classic cars’, ‘trains’, and ‘trucks and buses’ products for the EMEA and North America territories. Now let’s clear those slicer filters, and put the productline field back in the Columns area of the pivot table, so it’s ready for the next feature we will explore. And let’s move these slicers out of the way, further down the worksheet. 
    
    
- The last useful feature for pivot tables we are going to look at, is TIMELINES. A Timeline is another type of filter tool that enables you to filter specifically on date-related data in your pivot table. This is a much quicker and more effective way of dynamically filtering by date, rather than having to create and adjust filters on your date columns.

    · We can add a Timeline for our pivot table either from the PivotTable Analyze tab, or from the Insert tab. Again, ensure you select any cell in the pivot table first. 
    > We’ll select the Orderdate field as our Timeline filter. Then we can drag it up the worksheet and enlarge it. The default for this timeline is to display data by month, but you can also filter by days or by quarters. You can select a single quarter; or you can select a range of quarters. In this case, we’ll select twelve months between quarter 3 of 2003 and quarter 2 of 2004. You use the Clear Filter button to clear a timeline filter. You can also filter by years. For example, here we have selected 2003 only.

    · And you can combine slicers and timelines as filters in a pivot table. 
    > For example, here we can filter the slicers to display only data for trains, in the EMEA and North America territories, and only in the year 2003. And if we filter on the year 2004 instead, you’ll see that there is no data being displayed; meaning that there were no sales of train products in 2004 in either the EMEA or the North America territories. 
    
    · Timelines and Slicers have their own tabs in the ribbon when you select them, and their properties can be modified to change how they look and how they work. 
    > For example, let’s change this Timeline to a light green shade, and let’s change this Slicer to a nice orange color. And lastly, to remove a timeline or slicer, you can either select it and press the Delete key, or right-click it and choose Cut. 
    

> In this video, we learned about some of the other features in Excel that we can use with Pivot Tables, namely; Recommended Pivot Tables, Filters, Slicers, and Timelines.


# Hands-on Lab 7: Using Pivot Tables #
Estimated time needed: 30 minutes

In this lab, first you will learn how to format data as a table, how to create a Pivot Table and use fields to arrange data in a Pivot Table, and how to perform calculations using Pivot Table data. Next, you will learn some other features that we can use with Pivot Tables, including Recommended Charts, Filters, Slicers, and Timelines.

### Software Used in this Lab
The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free ‘Excel for the web’ version as this is available to everyone.
Although you can use the Excel Desktop software if you have access to this version, it is recommended that you use Excel for the web for the hands-on labs as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Dataset Used in this Lab
The dataset used in this lab comes from the following source: https://www.kaggle.com/sudalairajkumar/indian-startup-funding under a CC0: Public Domain license.
Acknowledgement and thanks also goes to https://trak.in who were generous enough to share the data publicly for free.
We are using a modified subset of that dataset for the lab, so to follow the lab instructions successfully please use the dataset provided with the lab, rather than the dataset from the original source.

## Objectives

After completing this lab, you will be able to:
Format data as a table
Create a Pivot Table and use fields to arrange data in a Pivot Table
Perform calculations using Pivot Table data
Use the Recommended Charts feature (does not work with the ‘Basic’ Office for the web plan.)
Use the Filters feature
Use the Slicers feature
Use the Timelines feature


## Exercise 1: Introduction to Creating Pivot Tables in Excel

In this exercise, you will learn how to format data as a table, how to create a Pivot Table and use fields to arrange data in a Pivot Table, and how to perform calculations using Pivot Table data.

### Task A: Format data as a table
Download the file indian_startup_funding_Lab7.xlsx. Upload and open it using Excel for the web.

Select cell A2.
On the Home tab, in the Tables group, click Format as Table.
Select Light Gray, Table Style Medium 15.


### Task B: Create a pivot table and use fields to arrange data in a pivot table

Select cell D4
On the Insert tab, click PivotTable.
Click OK.

Double-click Sheet1, type Pivot1 and click OK.

In the fields list, drag Industry Vertical to Rows.

In the fields list, drag City Location to Rows above Industry Vertical.

In the fields list, drag Startup Name to Rows below Industry Vertical.

In the fields list, drag Amount in USD to Values.

Use the drop down arrow for the City Location and Sort By Value in descending order (Largest to smallest) by the Count of Amount in USD.

In the ribbon, select the PivotTable tab, click Settings, then in the PivotTable Settings pane, under Layout, select Single column.

Right-click on the row label Amritsar and select Expand/Collapse and Collapse Entire Field.


### Task C: Perform a simple calculation in a pivot table

In the PivotTable Fields pane, in the Values section, click the drop-down arrow next to Count of Amount in USD, and click Value Field Settings.

Select Summarize value field by > Sum.
Click OK.

Select the column called Sum of Amount in USD and then on the Home tab, select Accounting Number Format > $ English (United States).



## Exercise 2: Pivot Table Features
In this exercise, you will learn some other features that we can use with Pivot Tables, including Recommended Charts, Filters, Slicers, and Timelines.

Note: The ‘Recommended Charts’ feature only works with ‘full’ Office for the web plans (those plans that come with an Office 365 subscription). Recommended Charts do not work with the ‘basic’ plan that comes with a Microsoft Account.

### Task A: Use of the Recommended Charts feature (Optional: If you have a full Office for the web plan)
Switch to worksheet indian-startup-funding.

Select column F (City Location).

On the Insert tab, select Recommended Charts.

Click + Insert PivotChart.

Switch to worksheet indian-startup-funding again.

Select column C, D, E.

On the Insert tab, select Recommended Charts.

Choose the recommended chart, and click + Insert PivotChart.


### Task B: Use of the Filters feature
Switch to worksheet Pivot1.

In the Pivot Table, click the Row Labels arrow.
Select City Location, then Filter….
Just select Burnsville, Delhi, New York, then click OK to display the amounts for startups in these three cities only.

In the Pivot Table, click the Row Labels arrow.
Select City Location, then click Clear Filter From ‘City Location’ to display the startups in all cities again.


### Task C: Use of the Slicers feature
Download the file indian_startup_funding_Lab7_with_slicers_timelines.xlsx. Upload and open it using Excel for the web.

Switch to worksheet Pivot1 if you are not there.
In the City Location slicer, select Burnsville, then Delhi, then New York.
To filter by multiple selection in the City Location slicer, with New York still selected, press CTRL and select Burnsville, and then Delhi.
To filter using more than one slicer, in the Investors Name slicer, select Amour Infrastructure, then press CTRL and select Westbridge Capital, and then Breakthrough Energy Ventures.
In the City Location slicer, click the Clear Filter button, then in the Investors Name slicer, click the Clear Filter button.


### Task D: Use of the Timelines feature

In the Date timeline, click top right drop-down and select DAYS, then scroll left and right.
In the Date timeline, click top right drop-down and select QUARTERS.
In the Date Timeline, select 2019 Q1, then drag 2019 Q1 to 2019 Q3.
In the Date timeline, click the Clear Filter icon.
In the Date timeline, click top right drop-down and select YEARS, then select 2020 only.



> Congratulations! You have completed Lab 7, and you are ready for the next topic.