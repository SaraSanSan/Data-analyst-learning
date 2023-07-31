
# ANALYZING AND MINING DATA #

### SUMMARY ###

- Statistics is a branch of mathematics dealing with the collection, analysis, interpretation, and presentation of numerical or quantitative data. 

- Statistical Analysis involves the use of statistical methods in order to develop an understanding of what the data represents. 

- Statistical Analysis can be:
    · Descriptive: that which provides a summary of what the data represents. Common measures include Central Tendency, Dispersion, and Skewness.
    · Inferential: that which involves making inferences, or generalizations, about data. Common measures include Hypothesis Testing, Confidence Intervals, and Regression Analysis.

- Data Mining, simply put, is the process of extracting knowledge from data. It involves the use of pattern recognition technologies, statistical analysis, and mathematical techniques, in order to identify correlations, patterns, variations, and trends in data. 

- There are several techniques that can help mine data, such as, classifying attributes of data, clustering data into groups, establishing relationships between events, variables, and input and output.  

- A variety of software and tools are available for analyzing and mining data. Some of the popularly used ones include Spreadsheets, R-Language, Python, IBM SPSS Statistics, IBM Watson Studio, and SAS, each with their own set of characteristics, strengths, limitations, and applications.



## OVERVIEW OF STATISTICAL ANALYSIS ##

- STATISTICS is a branch of mathematics dealing with the collection, analysis, interpretation, and presentation of numerical or quantitative data. 

> It’s all around us in our day to day lives. Whether we’re talking about average income, average age, or highest-paid professions... it’s all statistics. Today, statistics is being applied across industries for decision-making based on data. For example, researchers using statistics to analyze data from the production of vaccines to ensure safety and efficacy, or companies using statistics to reduce customer churn by gaining greater insight into customer requirements.

- STATISTICAL ANALYSIS is the application of statistical methods to a sample of data in order to develop an understanding of what that data represents. It includes collecting and scrutinizing every data sample in a set of items from which samples can be drawn. 

    · A SAMPLE: is a representative selection drawn from a total population, where population is a discrete group of people or things that can be identified by at least one common characteristic for purposes of data collection and analysis. 
    > For example, in a certain use case, population may be all people in a state that have a driving license, and a sample of this population that is a part, or subset, of the population could be men drivers over the age of 50. 
    
- Statistical METHODS are mainly useful to ensure that data is interpreted correctly, and apparent relationships are meaningful and not just happening by chance. Whenever we collect data from a sample, there are two different types of statistics we can run:

- DESCRIPTIVE statistics to summarize information about the sample.
    · Descriptive Statistics enables you to present data in a meaningful way allowing simpler interpretation of the data. Data is described using summary charts, tables, and graphs without any attempts to draw conclusions about the population from which the sample is taken. The objective is to make it easier to understand and visualize raw data without making conclusions regarding any hypotheses that were made. 

    · For example, we want to describe the English test scores in a specific class of 25 students. We record the test scores of all students, calculate the summary statistics, and produce a graph. Some of the common measures include:
    
        * CENTRAL TENDENCY, or locating the center of a data sample. These measures tell you where most values in your dataset fall. 
            1. So, in the earlier example, the MEAN score, or the mathematical average, of the class of 25 students would be the sum total of the scores of all 25 students, divided by 25, that is, the number of students. 
            2. If you order the above dataset from the smallest score value to the highest score value of the 25 students and pick the middle value— that is the value with 12 values to the left and 12 values to the right of a score value, that score value would be the MEDIAN for this dataset. If 12 students have scored less than 75%, and 12 students have scored greater than 75%, then the median is 75. Median is unique for each dataset and is not affected by outliers. 
            3. MODE is the value that occurs most frequently in a set of observations. For example, if the most common score in this group of 25 students is 72%, then that is the mode for this dataset. 
            
        * DISPERSION is the measure of variability in a dataset. Common measures are:
            1. VARIANCE defines how far away the data points fall from the center, that is, the distribution of values. When a distribution has lower variability, the values in a dataset are more consistent. However, when the variability is higher, the data points are more dissimilar, and extreme values become more likely. Understanding variability can help you grasp the likelihood of an event happening. 
            2. STANDARD DEVIATION tells you how tightly your data is clustered around the mean. 
            3. RANGE gives you the distance between the smallest and largest values in your datasets. 
        
        * SKEWNESS is the measure of whether the distribution of values is symmetrical around a central value or skewed left or right. Skewed data can affect which types of analyses are valid to perform. 
        
        * There are other tools as well, for example, using CORRELATION and SCATTERPLOTS to assess the relationships of paired data. 


- INFERENTIAL statistics to make inferences or generalizations about the broader population. 
    · Inferential statistics takes data from a sample to make inferences about the larger population from which the sample was drawn. Using these methods you can draw generalizations that apply the results of the sample to the population as a whole. 
    
    · Some common methodologies include:

        * HYPOTHESIS TESTING: For example, for studying the effectiveness of a vaccine by comparing outcomes in a control group, hypothesis tests can tell you whether the efficacy of a vaccine observed in a control group is likely to exist in the population as well.
        
        * CONFIDENCE INTERVALS incorporate the uncertainty and sample error to create a range of values the actual population value is like to fall within.
        
        * REGRESSION ANALYSIS incorporates hypothesis tests that help determine whether the relationships observed in the sample data actually exist in the population rather than just the sample. 
        

- There are various SOFTWARE packages to perform statistical data analysis, such as Statistical Analysis System (or SAS), Statistical Package for the Social Sciences (or SPSS), and Stat Soft. 

> Statistics form the core of data mining by: Providing measures and methodologies necessary for data mining; and Identifying patterns that help identify differences between random noise and significant findings. Both data mining and Statistics, as techniques of data analysis, help in better decision-making.



## WHAT IS DATA MINING? ##

- DATA MINING or the process of extracting knowledge from data, is the heart of the data analysis process: 
    · It is an interdisciplinary field that involves the use of pattern recognition technologies, statistical analysis and mathematical techniques. Its goal is to identify correlations in data, find patterns and variations. Understand trends and predict probabilities.
    > It essentially helps separate the noise from the real information and helps businesses focus their energies on only what is relevant.

- PATTERN recognition is the discovery of regularity's or commonality's in data.

    > Consider the log data for logins to an application in an organization. It contains information such as the username, login timestamp, time spent in each login session, and activities performed. When we analyze this data to gain insights into the habits or behaviors of users, for example, the time of the day when maximum users tend to login or user roles that typically spend the maximum hours logged into the application or modules in the workflow application that are being used where examining the data manually or through tools to uncover patterns hidden in the data. 

- A TREND, on the other hand, is the general tendency of a set of data to change overtime. 
    > For example, global warming in the short term, like a year on year basis temperatures may remain the same or go up or down by a few degrees, but the overall global temperatures continue to increase overtime, making global warming a trend.

- Data mining has APPLICATIONS across industries and disciplines. 
    > For example, profiling customer behaviors needs and disposable income in order to offer targeted campaigns, financial institutions, tracking customer transactions for unusual behaviors, and flagging fraudulent transactions using data mining models. The use of statistical models to predict a patients likelihood for specific health conditions and prioritizing treatment. Accessing performance data of students to predict achievement levels and make a focused effort to provide support where required. Helping investigation agencies deploy police force where the likelihood of crime is higher. Aligning supply and logistics with demand forecasts. 
    
- There are several TECHNIQUES you can use to detect patterns and build accurate models for discovery, be it descriptive, diagnostic, predictive, or prescriptive modeling. Let's understand some of the most commonly used:

    · CLASSIFICATION is a technique that classifies attributes into target categories. For example, classifying customers into low, medium, or high spenders based on how much they earn.

    · CLUSTERING is similar to classification, but involves grouping data into clusters so they can be treated as groups. For example, clustering customers based on geographic regions anomaly.
    
    · OUTLIER detection is a technique that helps find patterns and data that are not normal or unexpected. For example, spikes in the usage of a credit card that can flag possible misuse.

    · ASSOCIATION rule mining is a technique that helps establish our relationship between two data events. For example, the purchase of a laptop being frequently accompanied by the purchase of a cooling pad. 
    
    · SEQUENTIAL patterns is the technique that traces a series of events that take place in a sequence. For example, tracing a customer shopping trail from the time they log into an online store to the time they log out.

    · AFFINITY grouping is a technique used to discover co-occurrence in relationships. This technique is widely used in on line stores for cross selling and up selling their products by recommending products to people based on the purchase history of other people who purchased the same item.

    · DECISION TREES help build classification models in the form of a tree structure with multiple branches, where each branch represents a probable occurrence. This technique helps to build a clear understanding of the relationship between input and output.

    · REGRESSION helps identify the nature of the relationship between two variables, which could be causal or correlational. For example, based on factors such as location and covered area, a regression model could be used to predict the value of a house.



## TOOLS FOR DATA MINING ##

The commonly used software and tools for data mining are: Spreadsheets, R-Language, Python, SPSS Statistics, IBM Watson Studio and SAS. 

- SPREADSHEETS, such as Microsoft Excel and Google Sheets, are commonly used for performing basic data mining tasks. 
    · Them can be used to host data that has been exported from other systems in an easily accessible and easy-to-read format. 
    · You can pivot tables to showcase specific aspects of your data, which is vital when you have huge amounts to sort through and analyze. 
    · They also make it relatively easier to make comparisons between different sets of data. 

    · Add-ins available for Excel, such as the Data Mining Client for Excel, XLMiner, and KnowledgeMiner for Excel, allow you to perform common mining tasks, such as classification, regression, association rules, clustering, and model building. GoogleSheets also has an array of add-ons that can be used for analysis and mining, such as Text Analysis, Text Mining, Google Analytics.

- R is one of the most widely used languages for performing statistical modeling and computations by statisticians and data miners. 
    · R is packaged with hundreds of libraries explicitly built for data mining operations such as regression, classification, data clustering, association rule mining, text mining, outlier detection, and social network analysis. Some of the popular packages include: 
        * tm, a framework for text mining applications within R, provides functions for text mining. 
        * twitteR provides a framework for mining tweets. 
    · R Studio is a popularly used open-source Integrated Development Envionrment (or IDE) for working with the R programming language. 
    
- PYTHON libraries are commonly used:

    · PANDAS is an open-source module for working with data structures and analysis. It is possibly one of the most popular libraries for data analysis in Python. It allows you to upload data in any format and provides a simple platform to organize, sort, and manipulate that data. Using Pandas, you can: perform basic numerical computations such as mean, median, mode, and range; calculate statistics and answer questions regarding correlation between data and distribution of data; explore data visually and quantitatively; visualize data with help from other Python libraries.

    · NUMPY (NumPy) is a tool for mathematical computing and data preparation in Python. NumPy offers a host of built-in functions and capabilities for data mining. 
    
    · JUPYTER NOTEBOOKS have become the tool of choice for Data Scientists and Data Analysts when working with Python to perform DM and SA. 


- IBM SPSS stands for Statistical Process for Social Sciences. While the name suggests its original usage in the field of Social Sciences, it is popularly used for advanced analytics, text analytics, trend analysis, validation of assumptions, and translation of business problems into data science solutions. SPSS is closed source and requires a license for use. SPSS has an easy to use interface that requires minimal coding for complex tasks. It comprises of efficient data management tools and is popular because of its in-depth analysis capabilities and accurate data results. 
    
- IBM Watson Studio, included in the IBM Cloud Pak for Data, leverages a collection of open source tools such as Jupyter notebooks, and extends them with closed source IBM tools that make it a powerful environment for data analysis and data science. It is available through a web browser on the public cloud, private cloud, and as a desktop app. Watson Studio enables team members to collaborate on projects, that can range from simple exploratory analysis to building machine learning and AI models. It also includes SPSS Modeller flows that enable you to quickly develop predictive models for your business data. 
    
-  SAS ENTERPRISE MINER is a comprehensive, graphical workbench for data mining. It provides powerful capabilities for interactive data exploration, which enables users to identify relationships within data. SAS can manage information from various sources, mine and transform data, and analyze statistics. It offers a graphical user interface for non-technical users. With SAS, you can: identify patterns in the data using a range of available modeling techniques; explore relationships and anomalies in data; analyze big data; validate the reliability of findings from the data analysis process. SAS is very easy to use because of its syntax and is also easy to debug. It has the ability to handle large databases and offers high security to its users. 
    
    
> Your decision regarding the best tool for your needs will be driven by the data size and structures the tool supports, the features it offers, its data visualization capabilities, infrastructure needs, ease of use, and learnability. It’s fairly common to use a combination of data mining tools to meet all your needs.




# COMMUNICATING DATA ANALYSIS FINDINGS #

### SUMMARY ###

- Data has value through the stories that it tells. In order to communicate your findings impactfully, you need to: 

    · Ensure that your audience is able to trust you, understand you, and relate to your findings and insights.
    · Establish the credibility of your findings.
    · Present the data within a structured narrative.
    · Support your communication with strong visualizations so that the message is clear and concise, and drives your audience to take action.

- Data visualization is the discipline of communicating information through the use of visual elements such as graphs, charts, and maps. The goal of visualizing data is to make information easy to comprehend, interpret, and retain. 

- For data visualization to be of value, you need to:
    · Think about the key takeaway for your audience.
    · Anticipate their information needs and questions, and then plan the visualization that delivers your message clearly and impactfully.

- There are several types of graphs and charts available for you to be able to plot any kind of data, such as bar charts, column charts, pie charts, and line charts. 

- You can also use data visualization to build dashboards. Dashboards organize and display reports and visualizations coming from multiple data sources into a single graphical interface. They are easy to comprehend and allow you to generate reports on the go.

- When deciding which tools to use for data visualization, you need to consider the ease-of-use and purpose of the visualization. Some of the popularly used tools include Spreadsheets, Jupyter Notebook, Python libraries, R-Studio and R-Shiny, IBM Cognos Analytics, Tableau, and Power BI. 



## OVERVIEW OF COMMUNICATING AND SHARING DATA ANALYSIS ##

> The data analysis process begins with understanding the problem that needs to be solved and the desired outcome that needs to be achieved. And it ends with communicating the findings in ways that impact decision making. Data projects are the result of a collaborative effort spread across business functions involving people with multi-disciplinary skills, with the findings being incorporated into a larger business initiative. The success of your communication depends on how well others can understand and trust your insights to take further action. So, as data analysts, you need to tell the story with your data by visualizing the insights clearly and creating a structured narrative explicitly targeted at your audience. 

- Before you begin to create the communication, you need to reconnect with your audience. Begin by asking yourself these questions:
    · Who is my audience? What is important to them? What will help them trust me? 
    · Your audience is mostly going to be a diverse group—in terms of the business functions they represent, whether they play an operational or strategic role in the organization, how impacted are they by the problem, and other such factors. 
    · Your presentation needs to be framed around the level of information your audience already has. 
    · Based on your understanding of the audience, you will decide what, and how much, information is essential to enable a better understanding of your findings. It’s tempting to bring out all the data that you’ve been working with, but you have to consider what pieces are more important to your audience than others. 
    
- A presentation is not a data dump. Facts and figures alone do not influence decisions and move people to action. You have to tell a compelling story. Include only that information as is needed to address the business problem. Too much information will have your audience struggling to understand the point you’re making. Begin your presentation by demonstrating your understanding of the business problem to your audience. It’s easy to fall back on the assumption that we all know what we’re here for, but reflecting your understanding of the problem that needs to be solved, and the outcome that needs to be achieved, is a great first step in winning their attention and starting with trust. 

- Speaking in the language of the organization’s business domain is another important factor in building a connect between you and your audience. The next step in designing your communication is to structure and organize your presentation for maximum impact. Reference the data you have collected. Remember that the data, the very basis of everything that you are communicating, is like a black box for the audience. If you’re unable to establish the CREDIBILITY of your data, people don’t know that they can trust your findings. 
    · Share your data sources, hypotheses, and validations. 
    · Work towards establishing credibility of your findings along the way: don’t gloss over any key assumptions made during the analysis.
    · Organize information into logical categories based on the information you have—do you have both qualitative and quantitative information, for example? Be deliberate in taking a top-down or bottom-up approach in your narrative. Both can be effective—depends on your audience and use case. 
    · Be consistent in your approach. It’s important to determine what communication formats will be most useful to your audience. Do they need to take away an executive summary, a fact sheet, or a report? How is your audience going to use the information you have presented, that should determine the formats you choose. 
    · Insights must be explained in a way that inspires action. If your audience doesn’t grasp the significance of your insight or are unconvinced of its utility, the insight will not drive any value. A thousand-word essay will not have the same impact as a visual in creating a clear mental image in the minds of your audience. 
    · A powerful visualization tells a story through the graphical depiction of facts and figures. Data visualizations—graphs, charts, diagrams, etc, are a great way to bring data to life. Whether you’re showing a comparison, a relationship, distribution, or composition, you have tools that can help you show patterns and conclusions about hypotheses. 
    
> Data has value through the stories that it tells. Your audience must be able to trust you, understand you, and relate to your findings and insights. Establishing credibility of your findings, presenting the data within a narrative, and supporting it through visual impressions, you can help your audience drive valuable insights.



## INTRODUCTION TO DATA VISUALIZATION ##

- Data visualization is the discipline of communicating information through the use of visual elements such as graphs, charts, and maps. Its goal is to make information easy to comprehend, interpret, and retain. 

- Imagine having to look through thousands of rows of data to draw interpretations and compare that to a visual representation of that same data summarizing the findings. Using data visualization, you can provide a summary of the relationships, trends, and patterns hidden in the data, which, if not impossible, would be very hard to decipher from a data dump. 

- For data visualization to be of value, you have to choose the visualization that most effectively delivers your findings to your audience. And for that, you need to begin by asking yourself some questions. 
    > What is the relationship that I am trying to establish? Do I want to compare the relative proportion of the sub-parts of a whole, for example, the contribution of different product lines in the total revenue of the company? Do I want to compare multiple values, such as the number of products sold, and revenues generated over the last three years? Or, do I want to analyze a single value over time, which in this example could mean how the sale of one specific product has changed over the last three years. Do I need my audience to see the correlation between two variables? The correlation between weather conditions and bookings in a ski resort, for example. Do I want to detect anomalies in data—for example, finding values in data that could potentially skew the findings? 

- What is the question I’m trying to answer is not just an overarching question in the data visualization design and process. You need to be able to answer this question for your audience with every dataset and information that you visualize. You also need to consider whether the visualization needs to be static or interactive. An INTERACTIVE visualization, for example, can allow you to change values and see the effects on a related variable in real-time. 

- So, think about the key takeaway for your audience, anticipate their information needs and the questions they may have, and then plan the visualization that delivers your message clearly and impactfully. Let’s look at some basic examples of the types of graphs you can create for visualizing your data:

    · BAR CHARTS are great for comparing related data sets or parts of a whole. For example, in this bar chart, you can see the population numbers of 10 different countries and how they compare to one another. 
    · COLUMN CHARTS compare values side-by-side. You can use them quite effectively to show change over time. For example, showing how page views and user sessions time on your website is changing on a month-to-month basis. 
    * Although alike, except for the orientation, bar charts and column charts cannot always be used interchangeably. For example, a column chart may be better suited for showing negative and positive values.
    
    · PIE CHARTS show the breakdown of an entity into its sub-parts and the proportion of the sub-parts in relation to one another. Each portion of the pie represents a static value or category, and the sum of all categories is equal to hundred percent. In this example, in a marketing campaign with four marketing channels—social sites, native advertising, paid influencers, and live events—you can see the total number of leads generated per channel. 
    
    · LINE CHARTS display trends. They’re great for showing how a data value is changing in relation to a continuous variable. For example, how has the sale of your product, or multiple products, changed over time, where time is the continuous variable. Line charts can be used for understanding trends, patterns, and variations in data; also, for comparing different but related data sets with multiple series. 
    
    · DASHBOARDS organize and display reports and visualizations coming from multiple data sources into a single graphical interface. You can use dashboards to monitor daily progress or the overall health of a business function or even a specific process. Dashboards can present both operational and analytical data. For example, you could have a marketing dashboard using which you monitor your current marketing campaign for reach-outs, queries generated, and sales conversions, in real-time. As part of the same dashboard, you could also be seeing how the conversion rate of this campaign compares to the conversion rate of some of the successfully run campaigns in the past. Dashboards are a great tool to present a bird’s eye view of the complete picture while also allowing you to drill down into the next level of information for each parameter. 
    * Dashboards: are easy to comprehend by an average user make collaboration easy between teams; and allow you to generate reports on the go. Using dashboards, you can see the result of variations in data and metrics almost instantly and this can help you evaluate a situation from multiple perspectives, on the go, without having to go back to the drawing board.



## INTRODUCTION TO VISUALIZATION AND DASHBOARDING SOFTWARE ##

> In this video, we will look at some of the most commonly used data visualization software and tools. These include: Spreadsheets, Jupyter Notebook and Python libraries, R-Studio and R-Shiny, IBM Cognos Analytics, Tableau and Microsoft Power BI. Some of these are end-to-end data analytics solutions, while others are specifically for data visualization—ranging from free, open-source tools to commercially available solutions. 

- SPREADSHEETS, such as Microsoft Excel and Google Sheets, are possibly the most commonly used software to make graphical representations of data sets. Spreadsheets are easy to learn and have a ton of documentation and video tutorials available online for ready reference. 

    · EXCEL provides several chart types ranging from the basic bar, line, pie, and pivot charts, to the more advanced options such as scatter charts, trendlines, Gantt charts, waterfall charts, and combination charts (using which you can combine more than one type of charts). Excel also provides recommendations on the best visual representation for your data set. To make the charts more presentable, you can add a chart title, change colors of the elements, and add labels to data. 
    
    · GOOGLE SHEETS also offers similar chart types for visualization, though Excel does have more inbuilt formula-based options than Google Sheets. Like Excel, Google Sheets can help you choose the right visualization. All you have to do is highlight the data you wish to visualize and click the chart button and you get a list of suggested charts best suited for your data. Charts and reports automatically update, in Excel as well as in Google Sheets, as the underlying data is changed. Google Sheets is preferred over Excel, where multiple users need to collaborate. 
    

- JUPYTER NOTEBOOK is an open-source web application that provides a great way to explore data and create visualizations. You don’t have to be a Python expert to use Jupyter Notebook. 
    
- PYTHON provides a host of libraries that are used for data visualization. Let’s look at a few of those libraries.

    · MATPLOTLIB is a widely used Python data visualization library. It provides different kinds of 2D and 3D plots and the flexibility to create plots in several different ways. Using Matplotlib, you can create high-quality interactive graphs and plots with just a few lines of code. It has large community support and cross-platform support as it is an open-source tool. 
        
    · BOKEH provides interactive charts and plots and is known for delivering high-performance interactivity over large or streaming datasets. Bokeh offers flexibility for applying interaction, layouts, and different styling options to visualization. It can also transform visualizations written in some of the other Python libraries, such as Matplotlib, Seaborn, and Ggplot. 
        
    · DASH is a Python framework for creating interactive web-based visualizations. Using Dash, you can build highly interactive web applications using Python code. While knowledge of HTML and javascript is useful, but it is not a requirement. DASH is easily maintainable, cross-platform, and mobile-ready.


- Using R-STUDIO, you can create basic visualizations such as histograms, bar charts, line charts, box plots, and scatter plots; and advanced visualizations such as heat maps, mosaic maps, 3D graphs, and correlograms.

- R-SHINY is an R package that helps build interactive web apps that you can host as standalone apps on a webpage. These web apps seamlessly display R objects, such as plots and tables, and can be made live to allow access to anyone. You can also build dashboards using Shiny. The ease of working with Shiny is what popularized it among data professionals. 
        
- IBM COGNOS ANALYTICS is an end-to-end analytics solution. Some of the visualization features provided by Cognos include: Importing custom visualizations; A forecasting feature that provides time-series data modeling and forecasts based on data presented in corresponding visualizations; Recommendation for visualizations based on your data; Conditional formatting which allows you to see the distribution of your data and highlight exceptional data points, for example, highlighting high and low sales numbers over a certain threshold. COGNOS is known for its superior visualizations and overlaying data on the physical world using its geospatial capabilities. 

- TABLEAU is a software company that produces interactive data visualization products. Using tableau products, you can create interactive graphs and charts in the form of dashboards and worksheets, with drag and drop gestures. Tableau also offers the option to publish results in the form of stories. You can import R and Python scripts in Tableau and take advantage of its visualization features that are far more superior to that of other languages. Tableau’s visualization capabilities are easy and intuitive to use. Tableau is compatible with excel files, text files, relational databases, and cloud database sources such as Google Analytics and Amazon Redshift. 

- POWER BI is a cloud-based business analytics service from Microsoft that enables you to create reports and dashboards. It is a powerful and flexible tool known for its speed and efficiency, and an easy to use drag and drop interface. Power BI is compatible with multiple sources, including Excel, SQL Server, and cloud-based data repositories, which makes it an excellent choice for data professionals. Power BI provides the ability to collaborate and share customized dashboards and interactive reports securely, even on mobiles. Power BI’s dashboard consists of many visualizations on a single page that help you tell your story. These visualizations, called tiles, are pinned to the dashboard. The dashboard is interactive, which means a change in one tile affects the other. 

> When deciding which tools to use, you need to consider the ease-of-use and purpose of the visualization. In terms of the tools that are available and the visualization capabilities they offer. If you can visualize it, you can create it.
