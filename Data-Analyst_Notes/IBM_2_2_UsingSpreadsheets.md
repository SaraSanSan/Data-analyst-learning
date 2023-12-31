
# GETTING STARTED USING SPREADSHEETS #

### SUMMARY ###

- There are several features to modify views in Excel, and it is very straightforward to enter and edit data in a spreadsheet. 

- You can move or copy data within a worksheet or between worksheets, and you can use AutoFill to automatically enter data that is in a series or that fits a pattern. 

- You can format both cells and data in Excel. 

- A formula is made up of several component parts, and formulas can perform calculations using numbers directly or by using references to data in the worksheet. 

- You can use the Fill Handle in Excel to quickly copy formulas to other cells. 

- There are several different categories of function you can use for different purposes, and you can search for a function by name, or by category. 

- You can reference cells in the worksheet in your formulas by using relative, absolute, or mixed references. 

- You can make a formula absolute by adding a dollar symbol ($) to a cell reference. 

- If you get errors in your formulas, you can use the error-checking capabilities of Excel to resolve them. 


## VIEWING, ENTERING AND EDITING DATA ##

> Now that you have learned basic spreadsheet terminology and learned how to navigate your way around worksheets and select data in Excel, it’s now time to start entering some data. 

- First, we will look at some of the handy viewing features provided in Excel, and then we’ll enter some data, and then edit that data. 

- When you have a lot of data in your worksheet it can be useful to zoom in closer to a specific area of the data. The ZOOM SLIDER at the bottom right corner of the worksheet allows you to do just that. You can either click on the plus and minus buttons or drag the slider to select your preferred zoom value. You also have some zoom controls in the ribbon on the View tab. Zoom lets you pick a predefined zoom level or a custom one, the 100% button zooms the worksheet back to its original size, and Zoom to Selection enables you to select an area of data and then zoom into that specific selection only. 

- If you want to see several areas of your data at the same time while zoomed in, you can use the SPLIT BUTTON. This splits the screen into multiple sections; and you can scroll each section separately. If you only want two sections, you can remove either the horizontal or the vertical split by double-clicking on it. If you have headings in your columns like a header row, then you might want those to remain on screen while you move down the sheet. 

- To do that you need to use FREEZE PANES. You can freeze only the top row if you wish, or if that doesn’t suit, as is the case here, then you can select the row (or even just a cell in the row) below the row or rows you want to freeze, and then select Freeze Panes. You can do a similar thing for columns you want to freeze too. And you can even freeze both rows and columns at the same time. The trick here is to first select the cell that is both one row below where you want to freeze, and one column to the right of where you want to freeze. In this case, that is cell C4. Now we can scroll down the worksheet and across the worksheet and we can still see the header row and the Manufacturer and Model columns. 

- Now, if you have multiple workbooks open (notice I said workbooks and not worksheets) then you can switch between them by using VIEW, Switch Windows, or the faster method is to use the CTRL+F6 shortcut. 

- Now let’s enter some data into a blank worksheet. The easiest way to open a new worksheet from within Excel is to click the New button in the Quick Access Toolbar (or CTRL+N if you prefer keyboard shortcuts). So let’s enter some headings across the top of the worksheet; this is typically referred to as a ‘header row’. Note, that if you press Enter after typing data into a cell the next active cell is the one directly below, which is not what we want in this case. But, if we press Tab after we enter data in a cell, it selects the next cell along in the row as the active cell. Now we’ll enter some headings and press Tab after each entry. 

- Notice that the text is slightly longer in some of the cells and it either gets partly hidden by the next cell or overlaps it. If you click and hold the divider line between two columns, you can drag it left and right to resize it manually. If you want to do that automatically, you can double-click the divider line between two columns. As these are going to be headings for our columns, let’s make them bold. 

- Now let’s add another column between the parts and accessories columns. Simply select the right-hand of those two columns, then right-click and choose Insert to put another column to the left of the selected column. Let’s call it Servicing Sales. 

- To tidy up all our column widths simultaneously, we select all the columns from A to E, then double-click any of the divider lines between columns; this automatically reduces or increases each column’s width to fit the data in that column. 

- OK, now we have some headings, let’s enter some month data in column A. So, if we type Jan in cell A2 and press Enter then it takes us to the cell below, which is what we want in this case and we can type Feb in cell A3 and so on until we get to Dec in A13. 

- Now, let’s suppose you need to change a couple of your headings. You have several ways of editing existing data in a cell; You can either select the cell and then just start over typing. Or you can select the cell and press F2 on your keyboard to put the cursor at the end of the cell and make your changes. Or you can simply double-click somewhere on the cell to put the cursor at that position in the cell and make your changes. And you can even select the cell and then click in the formula bar to edit your cell data. Now let’s do the same for the parts and accessories column headings.

> In this video, we learned about some of the viewing options in Excel, and we learned how to enter and edit data in cells. In the next video, we will learn how to copy and fill data, and how to format the cells and data in a worksheet.



## COPYING, FILLING AND FORMATTING CELLS AND DATA ##

> Now that we have learned about some of the handy viewing features provided in Excel, and entered and edited some data, let’s discuss how to move, copy, and fill data, and how to format cells and data to suit our needs. 

- The first thing we are going to discuss is HOW TO MOVE DATA. 
    · So if you select a range of cells, in this case the headings in A1 to E1, and then hover over the top or bottom edge of a selected cell, and you will see the Move pointer, then you can drag the selection to another place on the worksheet. 
    · Alternatively, if you want to copy the data instead, you do the same thing but this time you also hold CTRL key as you select and drag the selection to another location and you will see the Copy pointer. 
    · If you are not comfortable with dragging, you can also use Copy and Paste menu commands or keyboard shortcuts. 
    · So if you select some data in column A and copy it to the clipboard then you simply select the new location and paste the copied data. 
    · You can also move or copy between worksheets, so let’s create a new worksheet. Then select some data from Sheet1, and this time let’s use the CTRL+C keyboard shortcut to copy it to the clipboard. Then choose the other worksheet and use the CTRL+V shortcut to paste the data. 

- However, notice that the COLUMN WIDTHS are not the same as the original source data, so let’s undo that and try another paste option. By default, when you paste the copied data, it uses the column width settings of the destination cells. So, to paste it and retain the column widths of the source data, you chose the special option under the Paste command, called Keep Source Column Widths. 

- As an alternative to having to enter data manually in a worksheet, you can use an Excel feature that automatically fill cells with data when it follows a sequential series or pattern. The feature is called AUTOFILL, and it can be especially useful when you need to enter lots of repetitive data into Excel, such as date information. 
    · For example, if you enter a month in a cell, even using a shortened version of the name, you can use what’s called the Fill Handle to select down to the end of the series, and AutoFill will work out what the series is, based on the selected data. Let’s try the same thing with days of the week. If you enter Mon in a cell, then drag the fill handle to use AutoFill, it will determine that you want to enter the days of the week sequentially. 
    · However, if you also enter Wed (for Wednesday) in the next cell down, and select both cells in the series, i.e. A16 and A17, and then drag the fill handle down, AutoFill determines that the sequence has changed to every other day, and fills in the data series for you. It’s important to select all cells that define the pattern when using AutoFill so that it can best determine what the pattern is, in this case cells A16 and A17. 
    · A similar thing applies to numerical patterns; if you enter 5 in a cell, and then use the fill handle to fill the data down the column. Because the data is not the name of a day or month for example, AutoFill can’t determine what the pattern is yet. So, In this case, it just copies the value 5 into every selected cell. However, if you enter the value 10 in B3, and then use the fill handle to fill the data down the column, AutoFlll determines that the pattern is incrementing by 5 each time and it fills in the remainder of the data pattern for you. 
    
- We are now going to look at FORMATTING our data, and there are essentially two distinct parts to this. 
    · First, there’s formatting of the cells themselves (with a fill color and a bold border for example and bold text within it). 
    · And then there’s formatting the data in the cells (for example, making it text format, number format, or a specific currency or accounting format).

    > Let’s open the car sales worksheet we used previously. Then select the headings in cells A3 to P3 either using the mouse, or you could use the shortcut keys CTRL+SHIFT+Right Arrow. On the Home tab, click the Styles drop-down arrow, and select a style color for your cells. Then you can make the selected cells bold. Then you select the data in the Manufacturer column either using the mouse, or the shortcut keys CTRL+SHIFT+Down Arrow. In the Styles drop-down arrow, select another style color for the selected cells. Again you can make the cells bold. Then you select the data in the Model column again either using the mouse, or the shortcut keys CTRL+SHIFT+Down Arrow. In the Styles drop-down arrow, select another style color for the selected cells. This time you could make the selected cells italic. And you can also change the font size and style. Lastly, you can select all the other cells in the data by using the mouse or the CTRL+SHIFT+Right Arrow then Down Arrow, and apply borders to the data cells. Now it’s time to format the cell data. The sales figures in columns C and D can be formatted to display only two decimal places; just select the data and click the Decrease Decimal button. We also have an issue with a couple of the car models. If you look in cells B129 and B130, where the model name is supposed to be displayed, you can see there are actually two dates listed instead. And if you look in the Number Format box, the format type is Custom. This has happened because the model numbers are supposed to be the Saab 9-5 and the Saab 9-3 but when the files were imported from CSV files these two cells must have been incorrectly determined to be date values and not just numbers. You can fix this by formatting these two cells as Text, and then enter the correct values of 9-5 and 9-3. The last thing we shall do is format some data as currency. If you look at the heading in column F it says it is Price in thousands of dollars, and cell F4 is using the General format. So, let’s change the format of this column to American currency format. We select the column, F in this case, then select More Number Formats from the drop-down list, then we choose the Currency option, and the correct currency symbol and format. And we’re done. 
    

> In this video, we learned how to move, copy, and fill data, and how to format cells and cell data to suit our needs. In the next video, we will look at the basics of formulas, learn how to perform simple calculations, and learn how to select ranges and copy formulas.



## THE BASICS OF FORMULAS ##

> Now that we have learned how to move, copy, and fill data, and how to format cells and data, next we will take a look at the basics of formulas, including some basic calculations, selecting ranges in formulas, and how to copy formulas. 

- A typical formula is made of several key components:

    · The equal sign starts the formula off and lets Excel know you are creating a formula in this cell. 

    · The next part is the function, which performs the calculation. For example, the SUM function adds up the values in referenced cells or cell ranges. 

    · Then comes the reference, which is the cell or range of cells you want to include in your calculation, and these need to be enclosed in parentheses.

    · You also have operators, which specify what type of calculation to perform. 
        * Common arithmetic operators include: addition, subtraction, multiplication and division. And these are represented by symbols: the plus symbol for addition, the minus symbol for subtraction, the asterisk for multiplication, and the forward slash for division. 
        * There are other types of operators too: Namely comparison, text concatenation, and reference. 

    · You may also use constants in your formulas, which as the name suggests are numbers or values which you can enter directly into a formula, and which don’t change. This might be a whole number such as 5, it might be a percentage such as 10%, or it might even be a date. So, a typical formula might be =SUM(B5*20), which would take the value in cell B5 and multiply it by 20. 
  
- Let’s start with a few basic calculations:

    > Suppose you want to add up January and February sales of accessories. You would start by typing an equal sign, which lets Excel know you are entering a formula. Then you type in the function you wish to use, in this case the SUM function. Note the description. Next you type an open parenthesis, then you select your cell range, which in this case would be E2 to E3, so you could enter that as ‘E2,E3’ then a close paranthesis and press Enter. And if you wanted to add March sales as well, then you would have to extend the cell range to include E4. So you could type E2,E3,E4 as your range and it will work. Remember, to edit a cell, you select the cell, and either edit it directly in the formula bar, or press F2, or double-click the cell. However, it’s very cumbersome and not very flexible to do it this way, because if you wanted to add up the entire column then you’d have to type every cell reference, one after the other. So thankfully, there’s a better way. Instead of typing each cell to include in the reference, you just put a colon between the first and last values in our range, so E2:E4, in this case. And if you wanted the whole column, then you would enter E2:E13 in your formula. But there’s another way of doing it, and that’s by using your mouse to select the range, so you still type =sum then open parenthesis, but select the range with your mouse (or SHIFT + arrow keys) and just press Enter. Excel will add the close parenthesis for you. To total these columns up, and add some tax, you’d add some headings first for Subtotals, and Tax at 20%. Then your formula will need to multiply the value in Subtotals by 20%. If you want to add up all the column subtotals and calculate the taxes, then you could repeat the previous process for each column, but that’s very time consuming, and you don’t need to, because Excel has some neat tricks to do this for you. Just select the fill handle in the bottom right corner of the cell, and drag across to the other cells to copy the formula; this is called AutoFill. Notice how the formula is copied, but the row references change in relation to the cells’ position on the worksheet. So what was E2:E13 has become B2:B13. These are known as relative references, but more on that later in the course. And you can do the same thing for the tax values in row 16. Now, you need a row for showing the totals. The calculation here is simply the subtotal value in cell B15, added to the tax in B16. And again, you can use the fill handle to copy the formula across. If you want to total the sales of all products by month, you’d add a column heading; notice how the cell style is copied to the new heading automatically. Remember, to widen a column, either drag the divider manually, or double-click the divider. Then enter the formula in cell F2 as you’ve done before. However, Excel has another trick up its sleeve. It’s called AutoSum and is found on the Home tab, in the Editing group. This is a great little shortcut for some simple common functions like Sum, Average, Count, Max, and Min, but you can choose other functions too. You want ‘Sum’ for this particular calculation. Notice that it also has a keyboard shortcut of ‘Alt plus equals’, and then press Enter, and it’s done. Now you can use the fill handle to copy down the remaining values. But hold on, there is one more Excel trick to show and it’s a good one! Suppose your column of data was very long; you might have to drag the fill handle down over several pages, which isn’t easy to do and can easily lead to errors when selecting large lists of data values. Rather than needing to drag down to the rest of the column, you can just double-click the fill handle, and it will automatically copy the formula to all the remaining cells in that column. This one is a real time-saver. Finally, let’s format all these values to use the US dollar currency format. 
    

> In this video, we learned about the basics of formulas, how to perform simple calculations, how to select ranges in formulas, and how to copy formulas. In the next video, we will look at how to use some of the common functions used by Data Analysts and discover some more advanced functions.



## INTRO TO FUNCTIONS ##

> Now that you have learned about the basics of formulas, learned how to perform some basic calculations, and how to select ranges and copy formulas, next we will have an introduction to functions, including using some common statistical functions. And then we will learn about some more advanced functions that a Data Analyst might also use. 

- First, let’s look at some common functions used for STATTISTICAL CALCULATIONS. So, we’ll add some row headings for average, minimum, maximum, count, and median. Then in cell B20, let’s work out the average of the car sales for the year, from the table above. On the Home tab, in the Editing group, we click the AutoSum drop-down list and choose Average. Now, because AutoSum tries to add up the values directly above it in the column, we need to modify the cell range here to B2 to B13. Then we can use the Fill Handle as we’ve seen before to copy the formula across to column E. For the minimum calculation in B21, we select Min from the AutoSum list. And again, we need to modify the cell range. So this calculates the lowest value in our range. And fill across to column E. And for the maximum calculation, we select Max from the list. And then modify the range. And once again, copy the formula across. This calculates the highest value in our range. In B23 we will calculate the Count, which basically just means the number of values that exist in the selected range. So, we select Count Numbers from the list. Then modify the range. For the median calculation, we can select ‘More Functions’ from the AutoSum list,then select ‘Statistical’ as the category, and scroll down to find the MEDIAN function. The ‘median’ returns the exact middle of a range of selected values. Note that if you’re selecting an odd number of values it will return the figure that is the middle value in your selected range, but if you have selected an even number of values in your range, it will return the middle figure between the two middle values in your range. Once again, we need to change the cell range to B2 to B13. And we can then copy this formula across to column E. 
    
> You’ve seen AutoSum and some of the common statistical functions in Excel, but there are another 400-plus other functions available, so let’s explore just a few of those now. 

- On the FORMULAS TAB, in the Function Library group, there are drop-down lists for several function categories. 

    · The first is a list of ‘Recently Used’ functions, which updates automatically as you use them. 
    · Then you have functions related to ‘Financial’ calculations. If you hover over the name of a function, you see a short description for each one; so here we have the accrued interest function, and here is the interest rate function. 
    · The ‘Logical’ list has BOOLEAN operator functions such as AND, IF, and OR. There are several functions related to Text, such as CONCAT, which is an updated version of a previous function called CONCATENATE (which is still supported by the way for backwards compatibility), FIND, and SEARCH. There are also several functions related to dates and times, such as NETWORKDAYS, WEEKDAY, and WEEKNUM. 
    · In the ‘Lookup & Reference’ list there are functions such as AREAS, HLOOKUP, SORTBY, and VLOOKUP. 
    · In the ‘Math & Trig’ list you’ll find lots of useful mathematical functions, such as POWER, SUMIF, and SUMPRODUCT, alongside many functions for trigonometric purposes, such as cosine, sine and tangent. 
    · There is also a ‘More Functions’ list which provides several more function categories, such as Statistical, Engineering, and Information. In the ‘Statistical’ list you’ll find functions such as Average, Count, Max, Median, and Min; we saw some of these used earlier in this video. 
    
    · If you’re struggling to find the function you want in these lists, you can also search for a function; just click the ‘Insert Function’ button on the Formulas tab, and then either browse the category lists available, or choose ‘All’ and look down the alphabetical list for the function you want. Alternatively, type the name of a function you want to find, and click ‘Go’ to search for it, then select the one you want from the returned search. 
    

> In this video, we learned about the basics of functions, how to use some of the more common functions that a Data Analyst might employ, and looked at some of the more advanced functions available in Excel. In the next video, we will look at referencing data in formulas; specifically differentiating between relative and absolute references, and error handling in formulas.



## REFERENCING DATA IN FORMULAS ##

> Now that you've had an introduction to functions, seeing the use of some common statistical functions and learned about some of the more advanced functions that a data analyst might use, in this video will look at the difference between relative, absolute, and mixed references in formulas as well as how to use them. And we'll learn about formula errors in Excel. 

- It's important to understand the difference between relative and absolute references when creating your formulas.

    · By default, in Excel, cell references are always RELATIVE REFERENCES. The term relative is the key here, because it means that when you reference a cell, you are in fact referencing the cells position in relation to the cell that the formula is in. That is why when we have been copying formulas from one cell to another so far in this course, using either copy and paste or the fill handle, we haven't needed to modify the cell references because Excel assumes you are using relative references. When the formulas are copied, the cell references are changed to match the relative positions of the cells that are being copied to. 
    
    · So now we know that relative references are the default in Excel, but how do we make it so that the cell references don't change when we copy them? For that you need to use ABSOLUTE REFERENCES in contrast to relative references. Absolute references to cells stayed the same when you copy a formula containing such references. 
    
    · Lastly, there may also be some instances where you only want one of the cell reference identifiers to be absolute and the other one to be relative. For example, you might want the row identifier to be absolute, but the column Identifier to be relative, or vice versa. These are called MIXED REFERENCES and an example of this would be equal sign a dollar sign one plus A3 where a dollar one. Has a relative column and an absolute row or dollar 8. Three has an absolute column. Ando relative RO. In contrast to relative and absolute references, when you copy a formula containing mixed cell references, any relative cell references will change, whereas any absolute cell references will stay the same in the copied formula. 
    
- First, let's look at an example of using relative references in a formula. For example, if we enter the formula equals A1 plus a 3IN cell, four note the blue an red highlighted cells in a one, and a three. These denote the cells being relatively referenced in the formula. If we copy the formula to the cell directly below using the fill handle, we can see that the result changes, and if we look at the copied formula. You can see that the blue and red cell references have changed relative to their position on the worksheet. The formula has been changed to equals A2 plus a four in the copied formula. That is, each cell reference has moved one cell down and if we copy and paste the formula to see seven, you can see that the results also changes and again we can see that the blue and red cell references in the copied formula have changed now. 

- Let's look at an example of how to use absolute references in a formula. All you need to do to make a cell reference absolute is put a dollar sign in front of the column and or row identifiers in the formula. For example, if we enter the formula equals dollar sign a one plus sign a dollar 3IN cell E4. Note the blue and red highlighted cells in a one and a three. These denote the cells being. Absolutely referenced in the formula. When we copy the formula using the fill handle, you can see that the result stays the same this time and if we look at the copied formula you can see that the blue and red cell references haven't changed. The formula is still equal sign dollar a dollar one plus a dollar three in the copied formula. That is, the cell references haven't changed. Similarly, if we then copy and paste the formula to E7, you can again see that the result stays the same this time and we can see that the blue and red cell references haven't changed. The formula is still equal sign dollar a dollar one plus dollar a dollar three in the copied formula. That is, the cell references haven't changed. 

- Lastly, will look at an example of how to use mixed references in a formula so. If we enter the formula equals a dollar one plus dollar 8, three in cell G4. Note the blue and red highlighted cells in A1A three. These denote the cells being referenced in the formula. If we copy the formula to the cell below using the fill handle, you can see that the result changes, but it's a different result from the previous examples. And if we look at the copied formula, you can see that the first blue cell reference has stayed the same. But the second red cell reference has changed. If we copy and paste the formula to G7, you can see that the same thing happens. The result changes and again we can see that the first blue cell reference has stayed the same in the copied formula, while only the red cell reference has changed. 


- Now we'll have a quick introduction to dealing with formula ERRORS in Excel. 
    · Because of the complexity of writing formulas, especially the more complicated ones, there are bound to be occasions when you make a mistake in the syntax or in the data selection which will lead to a formula error. 
    · Errors are typically denoted by displaying in the cell that is supposed to be displaying the result. 

    · One of the error codes in this list when you see multiple hash symbols in a cell, it's not really an error, it just means the column either isn't wide enough to display the whole word or value. Or it contains a negative date or time value? So if we type control plus semi colon, then space then control plus shift plus semi colon, it enters today's date and the current time. But the cell is too narrow to display it. So what we see is multiple hash symbols. If we adjust the column width we can now see the cell contents. So as I said, this really shouldn't be considered as an error. 

    · However if we enter the formula seen in Cell I7. When we press enter, we see a hash name error. This error was caused by trying to use an X as a multiplication operator when in fact it should be an asterisk. Note the small green triangle in the top left corner of the cell. Also note that when you select the cell and exclamation mark appears, providing you with a hint about what caused the error. In this case it says the formula contains unrecognized text. When you click the dropdown error next to the exclamation mark for an error, you see several options. The first line also gives you a clue on the nature of the error. This one says invalid name error, so it was probably a mistyped cell reference value or function name. If you click help on this error, uh, help pane opens with specific information related to this error. If you click show calculation steps, a dialog box opens displaying the current syntax with the error underlined. And you can try to evaluate the error if you are certain the error is incorrect, you can choose ignore error, and if you want to edit the formula, click edit in Formula Bar and the cursor will be focused in the formula bar so that you can try and correct the formula error.

    · If you click error checking options, the Excel Options Dialog Box is opened at the section related to error checking rules and you can modify these options to suit your needs. Each of the errors you make which generate one of the error codes listed at the start of this video will have a different reason and a different solution For more information on each of these errors and typical solutions visit the link provided. 
    

> In this video we learned about referencing data in formulas, specifically differentiating between relative, absolute, and mixed references, and how to use them. And we learned about formula errors in Excel.
