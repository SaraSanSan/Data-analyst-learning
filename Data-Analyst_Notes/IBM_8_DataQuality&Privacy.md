
# CLEANING & WRANGLING DATA USING SPREADSHEETS #

# BASICS OF DATA QUALITY AND PRIVACY #

### SUMMARY ###

- The Five Traits of Data Quality: 
    · Accuracy 
    · Completeness 
    · Reliability 
    · Relevance 
    · Timeliness 

- You can use the ‘Text Import Wizard’ to import data from other formats, such as plain text, or comma-separated value files. 

- The Three Fundamentals of Data Privacy: 
    · Confidentiality 
    · Collection and Use 
    · Compliance


## INTRODUCTION TO DATA QUALITY ##

> Data analysis can play a pivotal role in business decisions and processes. In order to use the data to make confident decisions, we must have the right information for the project and the data must be free from errors. In this video we will learn how to profile data to discover inconsistencies. Whether we are working with small sets of data or analyzing a spreadsheet with thousands of rows, one of the most difficult parts of the data analysis is finding and keeping clean data.

To help with this process and qualify the data, look for these five traits: Accuracy, Completeness, Reliability, Relevance and Timeliness. 

- ACCURACY is the first and most significant aspect to data quality. A data analyst must clean the data set by removing duplicates, correcting formatting errors, and removing blank rows. 

- COMPLETENESS: Another important aspect of data quality is determining if the information required to complete the data set is readily available. Why does this matter as a trait for quality data? Let’s say we are given the task to calculate the revenues of all sales per region. After collecting the data, we discover that no regions were specified. This data would then be considered incomplete and other sources would have to be considered to obtain the data required. 
    
- RELIABILITY: For instance, let’s say we are given the task to determine the agent revenue by customer. When gathering the data, we find the agents keep their own records and do not always update the information in the shared company database. With those factors in mind, we would then determine that the data in the shared company database was unreliable and new processes would need to be established to ensure reliable data.

- RELEVANCE: When collecting information, a data analyst must consider if the data being assembled is really necessary for the project. For example, when reviewing the data related to the sales revenue per customer, information such as customer birthdays and other personal information is also included. By making the determination early to exclude the personal information from the data set, the analyst would save themselves from having to review unnecessary information. 

- TIMELINESS: This trait refers to the availability and accessibility of the selected data. Let’s say our sales report is going to be used for weekly employee reviews, but our report is only refreshed once a month. This error in refreshing the data would cause our report to become outdated, and would have serious consequences for employee reviews. In this video we learned the important role of a data analyst in qualifying data. By considering the five traits of good quality data, an analyst can save time, avoid serious issues, and have data that is free from errors. In the next video we will take the collected data and learn how to import it to our spreadsheet.



## IMPORTING FILE DATA ##

> Now that you have learned about the importance of data quality, in this video you will learn how to import data from a text file using the Text Import Wizard, learn how to adjust column widths, and learn how to add and remove columns and rows. 

- As you know, by default Excel works with .xlsx or .xls files and opens them as workbooks. But Excel can also use data that is in other formats, such as plain text, or data that has been comma-separated and tab-separated. Sometimes, these source files will be saved with a .txt extension and referred to as ‘text’ files, but others might be saved with a .CSV file extension, and are typically referred to as CSV files. 
    · Here in Notepad, I have opened a text file that contains data about car sales, and it uses comma separated values (or CSVs) to separate each bit of data in a record. Notice that the top line holds headings, such as Manufacturer, Model, Engine_size, and so on, and each one is separated by a comma. We want these to become our headers when we import the file into Excel. The line below these headings is the first line of real data, and again you can see that each piece of data is also separated by a comma. There are 16 headings and there are also 16 pieces of data on each of the lines below the headings. If we scroll to the bottom, we can see that last data record is for the Volvo S80. 
    
    · Now, to open the file in Excel, we choose File, Open, and then either select the file from the recently used list, or click Browse to find the file we want to import. When we open the file, the Text Import Wizard launches automatically, and it will start to try and determine what your file is. Note that it has been detected as being a delimited file; that is, one that has its data fields separated by a character such as a comma or a tab. As we want the headings to become headers in Excel, we need to ensure that we select the option ‘My data has headers’. We can see a mini preview of the data in the preview box below. Then we click Next to proceed in the wizard. In step 2 of the wizard, we need to select our delimiter; that is, which character is separating our pieces of data; so we select Comma, and deselect any others. Note the data preview now starts to show us what the imported data will look like. You can scroll down and across this preview window to ensure that the data is going to look as you want and expect. It all looks OK, so we’ll continue with the wizard. In step 3 of the wizard, we can set the data format for each column. 
    · For example, you might want to change a column to Text or Date format. In this case we can just accept the default General format, and finish the import wizard. 
    
    · In Excel we can see that the headings in the text file have been imported as a header row. But also notice that some of the columns are not showing all the data; some of the headings are not showing in full and some of the data is not shown either; all you can see are a number of hashes in the cells. This is because the column widths are too narrow in some cases. If you remember, we can manually adjust a column’s width by dragging the divider across. But to change them all in one go, we select all the columns first, then double-click one of the selected column dividers. We can do a similar thing with rows by dragging to make them bigger or smaller, or double-clicking a row divider to autosize it. 

    · There are some columns that we have decided we don’t really need; namely Vehicle_type and Latest_Launch, so let’s remove those. This can either be done using the Delete drop-down menu in the Cells group on the Home tab, and select Delete Sheet Columns, or by selecting and right-clicking a column and deleting it that way. To add another column, you simply select the column to right of where you want your new column to be, then right-click the column and choose Insert. And let’s give the header a name, such as Year. To delete a row you don’t need, select the row, right-click it, and choose Delete. And to add a row, select the row below the place you want to add your new row, right-click the row, and choose Insert. 
    
    · If you want to save the file as an Excel file, you can either choose File, Save As, or you can click Save As in the yellow tooltip that appeared at the top of the worksheet when we imported the file, and then you would choose ‘Excel Workbook (*.xlsx)’ in the ‘Save as type’ box. 
    

> In this video, we learned how to import data using the Text Import Wizard, we learned how to adjust column widths, and we learned how to add and remove columns and rows. In the next video, we will discuss the importance of data privacy, including sensitive information, and personally identifiable data.



## BASICS OF DATA PRIVACY ##

> In this video, we will learn about data privacy and the regulations that govern the collected data. 

- When collecting customer data, specific regulations apply to how that data can used. By understanding data privacy regulations and getting familiar with the following three fundamentals, you can eliminate the risk of financial penalties and keep the trust of your customers. Confidentiality, Collection and Use, and Compliance. 

- CONFIDENTIALITY is an important element in data privacy and it acknowledges that the customer’s personal information belongs to them. The types of information that can be accessed by a data analyst can range from sales forecasts, to employee information, or even patient records. When accessing these types of records the analyst must be able to recognize the different types of personal data:

    · Personal Information or PI is any type of information that can be traced back to a specific individual. This type of information can include anything from emails to images. 
    · Personally Identifiable Information or PII is specific information that could be used to identify an individual. This type of information could include a social security number or a driver’s license number. 
    · And lastly , Sensitive Personal Information or SPI, may not necessarily identify a specific individual, but contains private information that needs to be protected because if made public it could possibly be use to harm the individual. The type of information can include data about race, sexual orientation, biometric or genetic information. 

By understanding personal data and the associated regulations, we can efficiently anonymize our data by removing unnecessary information. This type of action can help build consumer confidence and continue to develop the free flow of information. 


- When searching through data, the analyst must know the location of the company COLLECTING the data and the location of the respondent. Knowing where the data was collected is an essential element of data privacy and what regulations must be applied (COMPILANCE).

    · The General Data Protection Regulation or GDPR is a regulation specific to the European Union, and only applies to the jurisdiction of the individual. 
    · A new law created in Brazil, the LGPD, will take effect in August 2020. These new data policy regulations apply to individuals within Brazil, and ignores the location of the data processor. 
    · While the United States does not have one country-wide principle law for data privacy. Because of this individual states began to make their own regulations. For instance, California created the California Consumer Privacy Act (CCPA) to better protect customer data. 
    
    · There are also industry specific regulations that govern the collection and use of sensitive and personal data. For example, in Healthcare, HIPAA privacy rules govern the collection and disclosure of protected health information. In retail, the PCI standards govern credit card data, and failure to safeguard cardholder information can result in hefty fines. 
    
With a basic understanding of these policies, we are able to remain compliant when handling any sensitive information. Unfortunately, BREECHES in customer data is an all too common occurrence and understanding how to remain compliant is essential. 

Understanding the data privacy regulations of the European Union, the United States, and other countries as well as industries is key to keeping data safe. Companies must comply with these privacy regulations at all times and also make sure policies are readily accessible to EMPLOYEES. 
> For example, let’s say a data analyst downloads a spreadsheet of sensitive information. In order to complete the report by Monday morning, the analyst decided to take their work laptop home for the weekend. After driving home, the analyst accidently left the laptop in their car. The next morning, they found their car had been stolen along with the laptop. Because it is the responsibility of the company to keep customer data safe, this was a breach of privacy when the data left company property. This type of action could not only cost the company large amounts of money in fines and penalties, but could also reduce consumer confidence causing a significant impact to revenue. 


- While data privacy applies to most data that is collected, there are some instances where these regulations do not apply. In order for these laws and regulations not to apply, the particular collection of data must be completely anonymous. To make data anonymous means to exclude all data which ties it back to a particular individual. While this approach might not be practical in all circumstances, collecting data with privacy in mind could remove privacy limitations and make data collections more accessible. 


> In this video we learned about the importance of data privacy and the challenges that a data analyst can face when collecting and sorting through data. In the videos in the next lesson, we will learn about different methods for cleaning data in a spreadsheet.
