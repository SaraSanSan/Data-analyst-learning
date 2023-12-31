
# ANALYZING DATA USING SPREADSHEETS #

# DATA ANALYSIS BASICS, FILTERING AND SORTING DATA #

### SUMMARY ###

- Before shaping your data, you need to visualize the final output, and ask yourself the following questions: 
    · How big is the dataset?
    · What type of filtering is required to find the necessary information?
    · How should the data be sorted?
    · What type of calculations are needed?

- There are several advantages to formatting your data as a table: 
    · Automatic calculations even when filtering
    · Column headings never disappear
    · Banded rows to make reading easier
    · Tables will automatically expand when adding new rows 

- The most basic way of shaping your data is to sort and filter it:
    · Sorting data helps you to organize it by a specified criteria, such as numerically, alphabetically, or chronologically.
    · Filtering our data makes it easier to control what data is displayed and what is hidden, based on filtered fields. 

- Excel Functions:
    · Functions in Excel are arranged into multiple categories; including mathematical, statistical, logical, financial, and date and time-based. 
    · Common functions for a data analyst include IF, IFS, COUNTIF, SUMIF, VLOOKUP, HLOOKUP 


## INTRODUCTION ##

> Now that we have learned how to collect and clean our data, it is time to decide the best method for analysis. In this video, we will discuss the importance of filtering, sorting, performing calculations, and shaping our data to provide meaningful information. 

- Deciding how to manipulate our data can sometimes be difficult. Before we make any changes or adjustments, we will need to visualize the final output. Below are some questions to ask before beginning the task. How big is the dataset? What type of filtering is required to find the necessary information? How should the data be sorted? What type of calculations are needed? 

- Now that we have visualized the final output, we must decide the best approach to shape our data. 

    · The most basic step would be to filter and sort the data. By sorting the data, we are able to organize it based on conditions such as alphabetically or numerically. For example, if we wanted to check for duplicate order numbers, we could sort the data and quickly see any duplicates. 
    
    · After sorting and removing the duplicate row, we find that the view needs to be more specific to meet our requirements. We now decide that we only want to see the data for the month of November. By adding a filter, we can now choose to only see items with a ‘MONTH_ID” that is equal to “11”. By filtering our data, we are now able to only see the rows that meet the filter criteria and it allows us to better analyze our information. 
    

- Becoming familiar with all of the tools to analyze data can seem daunting, but one key benefit of using a spreadsheet is the ability to use functions. FUNCTIONS in Excel are organized by several categories, including mathematical, statistical, logical, financial, and date and time-based. 

    · Let’s say we wanted to get an average of company revenue for the month of June. We realize there are over 100 items that would need to be calculated. In normal circumstances, to get an average, we would have to create a formula to add each row and divide by the total number of rows. This type of calculation would not only be very long, but can expose the analyst to possibly making a mistake. =B1+B2+B3…../160 With the use of a function, we would be able to simplify our calculation in one easy step: =AVERAGE(B1:B160) 


- While sorting and filtering data on our spreadsheet can be useful on its own, first converting your data to a table has many benefits. When we convert our data into a table, we are able to filter and calculate the data more efficiently. 

    · One example is the ability to easily calculate columns. For the column ‘MSRP’, we choose ‘Sum’ and we’re able to quickly calculate the sum of the column. If we then look at the data, and only want to calculate the ‘MSRP’ total based on Japan, we would filter the ‘Country’ column to only display Japan, and the column would then only add the values in the rows that were associated with Japan. 
    
    · While all data may not work in a table, there are quite a few advantages to formatting your data as a table: Automatic calculations even when filtering Column headings never disappear. Banded rows to make reading easier. Tables will automatically expand when adding new rows.


- Sometimes data needs to be more organized then what a basic tabular format can give us, and creating pivot tables with charts can be a better way to analyze and display the required information. In Excel we have the option of creating a pivot table to display and analyze our data, and optionally, an associated pivot chart. 

    · For example, let’s say we want to know what company ordered products in the month of October. From the original table of data, we create a pivot table to organize and analyze the required data, along with a pivot chart to display the information. By then adding the month filter to the newly created pivot table, we can see the results for the month of October not only in the table, but the changes are automatically updated in the pivot chart. 
    
    · When trying to single out specific information in a large dataset, a pivot table is a nice way to show only the information that is required. This allows us to quickly and easily scan the essential information. 
    
    · Pivot charts are a nice accessory to pivot tables, as they allow us to visually process data, and in most cases, will let the audience grasp the information quicker. The advantages of selecting a pivot table and chart are: Manipulate data without using formulas quickly, summarize large data sets, ability to display engaging charts and graphs.
    
    
> In this video, we learned about the importance of filtering, sorting, performing calculations, and shaping our data to provide meaningful information, and we learned about some of the tools to begin analyzing our data. In the next video, we will learn more about filtering and sorting our data.



## FILTERING & SORTING DATA IN EXCEL ##

> In the previous video we learned how to use the Flash Fill and Text to Columns features in Excel to help clean data. In this video we will discuss how to filter and sort our data to enable us to control what information is displayed, and how it’s displayed in our worksheets. 

- Filtering your data enables you to gain more control over which parts of your data are displayed at any given time in Excel. This can help with the visibility of data by narrowing down the data to within specified criteria and parameters, and it can also help when searching for specific pieces of data. 

- To FILTER your data, the first thing you need to do is turn filtering on, which is very simple. On the Data tab, click Filter, and that’s it. You will now see a small filter icon next to each of the column headers. 
    · As a sidenote; if you want to only filter on one or more columns, select those columns first, then click Filter. 
    · As another sidenote; if you format your data as a table, the columns automatically have filter controls added to them. 
    
    · So now, each column has a filter that can be applied to the data in that column. In the Orderdate column you can filter on the years, in Productline you can filter on the different product types, and in Customername you can filter on each customer by name. 
    · Let’s first filter on the year. We’ll select orders from 2004 only, by deselecting the other year. And if we wanted to, we could expand the year and filter by months also, but we won’t do that for now. If you look in the status bar at the bottom of the worksheet, you can see that there are only 50 out of 114 records now displayed. 
    · If you want to clear a filter, you can either click the ‘Clear Filter From…’ option, or click the Select All item in the filter list. 
    
    · Now let’s filter on the productline column, to display only the rows that hold data for sales of classic cars. And again, we’ll clear the filter. Lastly, we’ll filter on the customername column, and only display sales to Mini Gifts Distributors Ltd. And then clear that filter. So far, we’ve only applied one filter at a time, but suppose you want to filter down to a greater degree? We can do that too by just enabling all those filters together and now we are only displaying sales of classic cars, to Mini Gifts Distributors Ltd, in 2004. 
    
    · Remember, if you only want to CLEAR one filter, then click its filter button in the column header, and click the ‘Clear filter from’ option but if you want to quickly clear ALL filters, you can use the Clear button in the Sort & Filter group on the Data tab. 
    

- So far, we’ve used what are commonly referred to as AutoFilters, but you can also use custom filters to specify other criteria, to apply a filter to text or numbers.

    · For example, if you wanted to see sales orders that are over or under a certain value, you can do that with custom filters. For the sales column, let’s add a number filter that only displays sales that are over $2,000. If you look in the status bar, you can see that we are now showing 111 out of 114 records. Then let’s clear that filter and filter it the other way to display the sales orders that are BELOW $2000. We can see that there are only 3 orders that are below $2000. 
    
    · It’s important to note that the data rows that we don’t see have not been removed they are still there they have just been hidden from view by the filters. And this is indicated by the row numbers you see on the left in blue. The row numbers start at 69, and jump in large increments, indicating that there are many more rows of data in our dataset, than are currently being displayed. 
    
    · If we look at a column filter for a column that contains text, you will see that the menu item changes to ‘Text Filters’ instead of ‘Number Filters’, and you can see there are several text filter options. And if you want to turn off filtering altogether for a worksheet, just click the Filter button on the Data tab. 


- Now, let’s take a look at the basic SORTING capabilities in Excel. Sorting is a very important part of the role of a typical Data Analyst. You might need to organize your text-based data alphabetically, your number-based data numerically, or your date-based data chronologically. 

    · When you sort data using these logical parameters, it makes it easier for you to conceptualize and visualize your data in a more meaningful way. When sorting data, the first thing you need to do is select which data to sort. 
    
    · For example, if you want to sort your customers alphabetically, select a cell in the Customername column first and then either sort by A to Z or by Z to A. And if you want to sort your sales figures numerically, select a cell in the Sales column first and then either sort from smallest to largest or from largest to smallest. And lastly, if you want to sort your customer’s order dates chronologically, select a cell in the Orderdate column first, then sort from oldest to newest or from newest to oldest. 
    
    · But you can also sort your data by more than one column at a time. Simply select a cell in your data, then on the Data tab, click Sort. Then either use the Sort by column suggested, or use the drop-down list to select a different column; in this case we’ll choose the ‘Orderdate’ column as our first sorting criteria, and we’ll choose ‘Oldest to Newest’ in the Order drop-down list. 
    
    · To add a further sorting level, you click ‘Add Level’. Then you choose another sort column in the ‘Then by’ drop-down list, in our case we’ll choose Sales, and for this sort level we’ll choose ‘Largest to Smallest’ in the Order list. 
    
    · If you have a header row in your data – as we do here – then ensure you select the ‘My data has headers’ checkbox, then click OK to sort. 
    
    · So, the data is now sorted to list the oldest orders by order date first, then within each order date, if there are multiple instances with the same order date… then the next sorting level lists data by the largest order values first, down to the smallest order values. 
    

> In this video, we learned how to use the Filter and Sort tools in Excel to filter and sort our data to enable us to control what information is displayed, and how it is displayed in our worksheets.



## USEFUL FUNCTIONS ##

> Now that we’ve learned how to use the Filter and Sort tools in Excel to filter and sort our data to enable us to control what information is displayed, and how it is displayed in our worksheets, in this video we’ll discuss how to use some of the most common functions a Data Analyst might use; namely IF, IFS, COUNTIF, and SUMIF. 

- First up, let’s look at how to use the IF function. 
    · The IF function is one of the most used logical functions in Excel. 
    · The IF function enables you to logically compare a value against criteria you set in the function, and then return a result based on whether the result of the logical comparison is true or false. And these values can be text values or numeric values. 
    · An IF function essentially says; “if something is true, then return a value or do something, but if it’s not true, then return a different value or do something else”.

    > For example, in our vehicle toy sales worksheet, if we wanted to have a column that recorded whether the order had been shipped or not, you could add a new column to the right of the existing column – let’s call it shipped? and then enter the formula seen in cell H2 This formula is saying – if the text in G2 says ‘shipped’ then return ‘Yes’, and if it doesn’t then return ‘No’. You can then use the Fill Handle to copy this formula down the column. You can see that most of the cells do say ‘Yes’, but some don’t, as the order hasn’t been shipped for one reason or another. 
    
    · We could also use the IF function to emphasize the size of an order. So, if we add a new column to the right of ‘Sales’, and name it ‘3K plus or minus’ Then enter the formula seen in cell F2 This formula is saying – if the order is over three thousand, then return the text “Over 3k”, but if it isn’t, then return the text “Under 3k”. And we can copy the formula down the column. 
    
    · In an ideal world, you would only use the IF function to apply one or two conditions, but there may be scenarios where you want to apply multiple conditions. In these cases, you can use the ‘nesting’ capabilities of functions to bring together several IF statements in one formula; these are called ‘nested IF functions’. 
    > For example, if we add another column here for the order size. And then enter the formula seen in cell F2. You can see that this formula, contains multiple IF functions; one is needed for each condition one for Large, one for Medium, and one for Small and it requires three sets of parentheses. So, it’s a relatively long and complex formula, but it does work. Again, we can copy the formula down the column.

    · Even though Excel technically supports the nesting of up to 64 different IF functions in a formula, it is not a recommended best practice. Having multiple IF functions in a single formula can become extremely challenging to manage. 
    > For example, suppose you come across a formula like this that you haven’t used for some time, or even worse, was created by someone else; it could be quite difficult to work out how and why it is being used. Also, if your conditions increase, then you need to add more conditions to an already quite complex and long formula, which will only complicate matters more. 
    
- To resolve this issue, a new function was developed called IFS. 
    · The IFS function is only supported on Excel 2019, Excel for Microsoft 365, and Excel for the web. 
    · As the name suggests, this function can replace multiple nested IF functions being used in a single formula, to simplify matters. 
    · So, if we add a further column for order size but this time we’ll use the IFS function instead. 
    
    > As you can see in cell G2, this formula only has one set of parentheses instead of three, and only uses one function instead of three. Let’s copy that formula down the column too. Now let’s have a look at another example of using the IF function, but we’ll combine it with Conditional Formatting too. If we switch to the car sales worksheet… and add a new column to the right of the Year Resale Value column and call it ‘Retention %’. Then, we enter the formula seen in cell G2, which will divide the ‘Year Resale Value’, by the original ‘Retail Price’. We need to format this as a percentage. And then we can copy it down the column. Next, we’ll add a column to highlight the retention value for each car. The formula we add here in cell H2 uses the IF function to state that if the percentage in the previous column is greater than 69%, then mark it as ‘Good’, but if it isn’t, then mark it as ‘Poor’. Once again, we’ll copy the formula down the column. 
    
    > We could also use Conditional Formatting to highlight the retention value percentages even more. We select H2, and on the Home tab, click Conditional Formatting, and make a new rule. The condition in our rule will only format cells that contain a specific text value… and that value is the word ‘GOOD’. And if it does match that condition, then format it with a dark green font and fill the cell in pale green. Let’s copy that conditional formatting down the rest of the column. You can see that the cells that contain the word ’good’ are now formatted as we defined, but the cells containing the word ‘poor’ are not. Let’s add another conditional format rule. This time, we’ll select Manage Rules, because we are going to add another rule to our existing rule. he new rule will be the same as the previous one, with the exception of looking for a match with the word ‘poor’ instead, and formatting those matching cells with red text and a pink background fill. And once again, we copy that down the column. Now all the cells that contain the word ‘poor’ are formatted as red text with a pink cell fill. 


- Let’s now have a quick look at how to use the COUNTIF function. 
    · COUNTIF is one of the statistical functions provided in Excel. You can use it to count the number of cells that meet a certain criterion; such as the number of instances where an employee’s name appears in a list of sales invoices, or the number of occasions a particular part number appears in a list of purchase orders. 
    
    > Let’s switch to the vehicle toy sales worksheet. Suppose you want to find out how many of the sales orders in the list went to customers based in the United Kingdom. We enter the formula you see in cell AD7. Note that when we are using text as a criterion, we have to enclose the text in quotation marks. So there were 6 sales orders in the UK. And if you wanted to discover the same thing for French customers, then you would just edit the existing formula, or copy it and then edit it. You can see there were 14 orders for French customers. Notice that this time the text entered was in lowercase, and it still works; so names in this function are not case-sensitive. And let’s do the same for United States customers; there are 41 orders to customers based in the states. 
    
    · There is also a newer function called COUNTIFS which applies criteria to cells across multiple ranges to count the number of occasions where all criteria have been met. This removes the need to use multiple COUNTIF functions in a long and complex single formula. The COUNTIFS function is only supported on Excel 2019, Excel for Microsoft 365, and Excel for the web. 
    
- Now let’s take a quick look at how to use the SUMIF function, which is a very commonly used mathematical function in Excel. 
    · You use the SUMIF function to sum the values within a specified range that meet specified criteria. 
    
    > For example, you might want to add up only the salaries that are over a specified salary level, or you might want to find the total of all sales of a particular product category. We’ll enter the formula seen in cell AD10 This formula will add up each of the sales orders that have a total of more than 3,000 dollars. Again, notice that because we have used an arithmetic operator, that is the ‘greater than’ operator, we must enclose the criterion in quotes. If we specify a criterion that is only a number, we don’t enclose it in quotes. So, the total sum of all orders that were over 3,000 dollars is almost 470,000 dollars. 
    
    · You can also use wildcards such as ‘question mark’ (?) and ‘asterisk’ (*) when searching for partial matches, and you can also specify to extract values from a different column than the column where you have specified the criteria.
    > For example, if we enter the formula you can see in cell AD13, it will sum all the car sales in column E, for only those products in the ‘productline’ column that end in ‘cars’. 
    
    · There is also a newer function called SUMIFS that you can use to sum cells based on multiple criteria. This removes the need to use multiple SUMIF functions in a long and complex single formula. The SUMIFS function is only supported on Excel 2019, Excel for Microsoft 365, and Excel for the web. 
    

> In this video, we learned how to use the IF, IFS, COUNTIF, and SUMIF functions. In the next video we’ll look at how to use the VLOOKUP and HLOOKUP reference functions.



## USING VLOOKUP & HLOOKUP FUNCTIONS ##

> Now that we’ve learned how to use the IF, IFS, COUNTIF, and SUMIF functions, in this video we’ll look at how to use the VLOOKUP and HLOOKUP reference functions. 

- VLOOKUP is one of the most commonly used reference-type functions in Excel, and it enables you to find data referenced in a lookup table.
    · It stands for Vertical Lookup and therefore is a useful tool to use when you want to find something in a table or a range by row. 
    · Shortly, we will look at HLOOKUP, which stands for Horizontal Lookup, which looks for data by column instead. 
    
    · VLOOKUP works by using a common shared key between the source data and the lookup data in the lookup table. 
    · A typical VLOOKUP formula would look like: =VLOOKUP(B3,A2:B12,2,FALSE)
        * B3 is the lookup value, that is, the value or word you are looking for.
        * A2:B12 is the lookup table or range, that is, the table array or range of cells that contains the lookup value. In a formula, Excel references this as ‘table_array’. The lookup table can be on the same worksheet or in another separate worksheet. 
        * 2 is the lookup column number, that is, the number of the column in the lookup table that contains the value you are looking for. In a formula, Excel references this as ‘col_index_num’. 
        * FALSE is an optional parameter that determines whether the match found has to be exact (denoted by FALSE), or can be approximate (denoted by TRUE). 
            - In a formula, Excel references this as ‘[range_lookup]’. The square brackets round this argument in the formula, signifies that it is an optional argument, whereas the others are required arguments of a VLOOKUP formula. If you don’t specify the optional FALSE or TRUE parameter in your formula, it will default to FALSE; that is, an exact match is required. 
            - You can also use the number 0 instead of FALSE, and the number 1 instead of TRUE. 
            
    · OK, now let’s see the VLOOKUP function in action:
     > In the car sales worksheet, suppose we wanted a quick price list of our favorite cars. The first thing we need to do, is put the column containing the value we want to search for, in the leftmost column, as VLOOKUP requires this. Then we can delete the original column. We then enter the formula seen in cell V16, which is looking for the word ‘Corvette’ in the table array from cell A2 to G156, and then looks for the value in the fifth column – in this case, the ‘Price’ column – that matches the row containing ‘Corvette’ and returns an exact value of 45,705 dollars. Note that in this example, we are using a part of our existing data table as the lookup table, or table array. 
     > Let’s format that as US currency. Then we’ll format it to zero decimal places. In fact, rather than use the reference A25 in the formula, it will be easier to use the reference to the word Corvette in the mini table in this worksheet, where our list of favorite cars is. So that is V5, and the formula still works. Now, let’s copy that formula up to the favorite car table, above it in the worksheet. But there’s a problem, because when we copied the formula, the cell references changed. This happened because as we learned earlier in this course, the default state of cell references is relative, and we want them to be absolute in this case. So, let’s undo that copy operation. 
     > To make the cell references absolute, we need to add dollar symbols to all the cell references in the formula. This can either be done manually, or you can put the cursor in each cell reference in turn in the formula and press F4 each time, to automatically add the dollar symbols. Let’s try and copy the formula again and this time it works. 
     > If we use the Fill Handle on cell W5 to copy it down to the rest of the cars, it doesn’t work; in fact, we end up with the same result in every cell. Why? Because each one is referencing the same cells in the lookup value, because we used an absolute reference. All we need to do now, is modify the formula to remove the absolute reference for just the row parameter, in the lookup value part of the formula, by removing the dollar symbol. So in cell W5 we change $V$5 to $V5, then when we drag the Fill Handle down it will copy the formula correctly, and all the prices will be changed to reflect their correct retail price. 
     > Lastly, to show that the two tables are now connected by this VLOOKUP function, if we change the retail price for the Chevrolet Corvette in the main data table in cell E25, the price will also change in the favorite cars price list. 
     

- Let’s now take a quick look at the HLOOKUP function, which as we mentioned earlier, does the same thing, and works in virtually the same way, as the VLOOKUP function, but it looks for data in columns, rather than rows. 
    · So, HLOOKUP looks for a word or value in the top row of a table, and then returns a value in the same column from a row specified in the table array. 
    · Therefore, you would use HLOOKUP if your comparison values were situated in a row along the top of a data table. 
    · In contrast, you would use VLOOKUP if your comparison values were located in a column to the left of the data you want to find; as they were in the previous task. 
    · Of the two functions, VLOOKUP is used far more than frequently than HLOOKUP, because of the nature of most data tables. 
    
    · The syntax for HLOOKUP is identical to that of VLOOKUP except that you specify a row index number, referenced in a formula by Excel as ‘row_index_num’. This indicates the number of the row in the lookup table that contains the value you are looking for. 
    
    > Let’s create a small lookup table on the right hand-side of our main data table; a few columns have been hidden in this worksheet to make viewing a little easier. So we’ve now got Low HP, Medium HP, and High HP in the top row of the lookup table. Next, we’ll add Wingdings symbols as ratings for the 3 horsepower levels, 1 sad face for the low horsepower rating, 2 neutral faces for the medium rating and 3 happy faces for the high horsepower rating. Now, let’s add a new column to the right of the HP Level column, and call it HP Rating. Then in cell L2 we’ll enter the HLOOKUP function. This function will look for the value in cell K2, which in this case is ‘Medium HP’, and it will look for it in the cell range from Y21 to AA22, which is our little lookup table, and it will return the answer it finds in row 2 of the table under Medium HP, and use an exact value. Note that we’ve used some absolute references in this formula too. Notice that what is returned is the text ‘KK’, so we need to format the cell using the Wingdings font. Now, when we double-click the Fill Handle, the whole column shows the HP Rating symbols relevant to each row’s HP Level value. And we’re done. 
    

- Although VLOOKUP and HLOOKUP are regularly still used as the de facto functions for lookup references in Excel, there is a newer function called XLOOKUP. 
    · This version is only supported on Excel desktop versions from Excel for Microsoft 365, and on Excel for the web, as well as on Excel for iPad and iPhone, and Excel for Android tablets and phones. XLOOKUP is an improved and combined version of VLOOKUP and HLOOKUP together. It can work in any direction; vertically or horizontally. It also uses separate lookup array and return array values, instead of a single table array and a column or row index number. 
    

> In this video, we learned how to use the VLOOKUP and HLOOKUP functions in Excel to find and connect to data referenced in both vertical and horizontal lookup tables. In the videos coming up in the next lesson, we’ll start to look at using Pivot Tables in Excel.
