
# LANGUAGES FOR DATA PROFESSIONALS #

## OVERVIEW ##

A data analyst's ecosystem includes the infrastructure, software, tools, frameworks, and processes used to gather, clean, analyze, mine, and visualize data. Data can be categorized as:

- Structured: Data that follows a rigid format and can be organized neatly into rows and columns. Typically in databases and spreadsheets. 
- Semi-structured data: A mix of data that has consistent characteristics and data that doesn’t conform to a rigid structure. For example, an email has the name of the sender and recipient (structured), but also has the contents of the email (unstructured). 
- Unstructured data: Data that is complex, and mostly qualitative information that is impossible to reduce to rows and columns. For example, photos, videos, text files, PDFs, and social media content. 

    The type of data drives the kind of data repositories that the data can be collected and stored in, and also the tools that can be used to query or process the data. Data also comes in a wide-ranging variety of file formats being collected from a variety of data sources, ranging from relational and non-relational databases, to APIs, web services, data streams, social platforms, and sensor devices. This brings us to data repositories: A term that includes databases, data warehouses, data marts, data lakes, and big data stores. The type, format, and sources of data influence the type of data repositories that you can use to collect, store, clean, analyze, and mine the data for analysis. If you’re working with big data, for example, you will need big data warehouses, that allow you to store and process large-volume high-velocity data and also frameworks that allow you to perform complex analytics in real-time on big data. The ecosystem also includes languages that can be classified as query languages, programming languages, and shell and scripting languages. From querying and manipulating data with SQL to developing data applications with Python, and writing shell scripts for repetitive operational tasks, these are important components in a data analyst’s workbench. Automated tools, frameworks, and processes for all stages of the analytics process are part of the Data Analysts ecosystem. From tools used for gathering, extracting, transforming, and loading data into data repositories, to tools for data wrangling, data cleaning, data mining, analysis, and data visualization — it's a very diverse and rich ecosystem. Spreadsheets, Jupyter Notebooks, and IBM Cognos are just a few examples.


## TYPES OF DATA ##

- DATA is unorganized information that is processed to make it meaningful. 
- Data comprises of facts, observations, perceptions, numbers, characters, symbols, and images that can be interpreted to derive meaning. 

    - Structured data has a well-defined structure or adheres to a specified data model, can be stored in well-defined schemas such as databases, and in many cases can be represented in a tabular manner with rows and columns. Structured data is objective facts and numbers that can be collected, exported, stored, and organized in typical databases. Some of the sources of structured data could include: SQL Databases and Online Transaction Processing (or OLTP) Systems that focus on business transactions, Spreadsheets such as Excel and Google Spreadsheets, Online forms, Sensors such as Global Positioning Systems (or GPS) and Radio Frequency Identification (or RFID) tags; and Network and Web server logs. You can typically store structured data in relational or SQL databases. You can also easily examine structured data with standard data analysis methods and tools. 

    - Semi-structured data is data that has some organizational properties but lacks a fixed or rigid schema. It cannot be stored in the form of rows and columns as in databases. It contains tags and elements, or metadata, which is used to group data and organize it in a hierarchy. Some of the sources of semi-structured data could include: E-mails, XML, and other markup languages, Binary executables, TCP/IP packets, Zipped files, Integration of data from different sources. XML and JSON allow users to define tags and attributes to store data in a hierarchical form and are used widely to store and exchange semi-structured data. 
    
    - Unstructured data is data that does not have an easily identifiable structure and, therefore, cannot be organized in a mainstream relational database in the form of rows and columns. It does not follow any particular format, sequence, semantics, or rules. It can deal with the heterogeneity of sources and has a variety of business intelligence and analytics applications. Some of the sources of unstructured data could include: Web pages, Social media feeds, Images in varied file formats (such as JPEG, GIF, and PNG), video and audio files, documents and PDF files, PowerPoint presentations, media logs and surveys. Unstructured data can be stored in files and documents (such as a Word doc) for manual analysis or in NoSQL databases that have their own analysis tools for examining this type of data. 
    
>> To summarize, structured data is data that is well organized in formats that can be stored in databases and lends itself to standard data analysis methods and tools; Semi-structured data is data that is somewhat organized and relies on meta tags for grouping and hierarchy; and Unstructured data is data that is not conventionally organized in the form of rows and columns in a particular format.


## TYPES OF FILE FORMATS ##

The most common standard file formats include:

    - DELIMITED TEXT FILES: Are text files used to store data as text in which each line, or row, has values separated by a delimiter; where a delimiter is a sequence of one or more characters for specifying the boundary between independent entities or values. Any character can be used to separate the values, but most common delimiters are the comma, tab, colon, vertical bar, and space. Delimited files allow field values of any length and are considered a standard format for providing straightforward information schema. They can be processed by almost all existing applications. Delimiters also represent one of various means to specify boundaries in a data stream.
        · CSV (Comma-Separated Values) and TSV (Tab-Separated Values) are the most commonly used file types in this category. 
        · When literal commas are present in text data and therefore cannot be used as delimiters, TSVs serve as an alternative to CSV format. Tab stops are infrequent in running text. Each row, or horizontal line, in the text file has a set of values separated by the delimiter, and represents a record. The first row works as a column header, where each column can have a different type of data. For example, a column can be of date type, while another can be a string or integer type data. 
    
    - XLSX (Microsoft Excel Open XML Spreadsheet): Is a Microsoft Excel Open XML file format that falls under the spreadsheet file format. It is an XML-based file format created by Microsoft. In an .XLSX, also known as a workbook, there can be multiple worksheets. And each worksheet is organized into rows and columns, at the intersection of which is the cell. Each cell contains data. XLSX uses the open file format, which means it is generally accessible to most other applications. It can use and save all functions available in Excel and is also known to be one of the more secure file formats as it cannot save malicious code. 
    
    - XML (Extensible Markup Language): Is a markup language with set rules for encoding data. The XML file format is both readable by humans and machines. It is a self-descriptive language designed for sending information over the internet. XML is similar to HTML in some respects, but also has differences; for example, an .XML does not use predefined tags like .HTML does. XML is platform independent and programming language independent and therefore simplifies data sharing between various systems. 
    
    - PDF (Portable Document Format): Is a file format developed by Adobe to present documents independent of application software, hardware, and operating systems, which means it can be viewed the same way on any device. This format is frequently used in legal and financial documents and can also be used to fill in data such as for forms. 
    
    - JSON (JavaScript Object Notation): Is a text-based open standard designed for transmitting structured data over the web. The file format is a language-independent data format that can be read in any programming language. JSON is easy to use, is compatible with a wide range of browsers, and is considered as one of the best tools for sharing data of any size and type, even audio and video. That is one reason, many APIs and Web Services return data as JSON.


## SOURCES OF DATA ##

Some common sources are: Relational Databases, Flat files and XML Datasets, APIs and Web Services, Web Scraping, Data Streams, and Feeds.

Typically, organizations have internal applications to support them in managing their day to day business activities, customer transactions, human resource activities, and their workflows. These systems use relational databases such as SQL Server, Oracle, MySQL, and IBM DB2, to store data in a structured way. Data stored in databases and data warehouses can be used as a source for analysis. For example, data from a retail transactions system can be used to analyze sales in different regions, and data from a customer relationship management system can be used for making sales projections. External to the organization, there are other publicly and privately available datasets. For example, government organizations releasing demographic and economic datasets on an ongoing basis. Then there are companies that sell specific data, for example, Point-of-Sale data or Financial data, or Weather data, which businesses can use to define strategy, predict demand, and make decisions related to distribution or marketing promotions, among other things. Such data sets are typically made available as flat files, spreadsheet files, or XML documents. 

Flat files, store data in plain text format, with one record or row per line, and each value separated by delimiters such as commas, semi-colons or tabs. Data in a flat file maps to a single table, unlike relational databases that contain multiple tables. One of the most common flat file format is CSV in which values are separated by commas. Spreadsheet files are a special type of flat files, that also organize data in a tabular format – rows and columns. But a spreadsheet can contain multiple worksheets, and each worksheet can map to a different table. Although data in spreadsheets is in plain text, the files can be stored in custom formats and include additional information such as formatting, formulas, etc. Microsoft Excel, which stores data in .XLS or .XLSX format is probably the most common spreadsheet. Others include Google sheets, Apple Numbers, and LibreOffice. XML files, contain data values that are identified or marked up using tags. While data in flat files is “flat” or maps to a single table, XML files can support more complex data structures, such as hierarchical. Some common uses of XML include data from online surveys, bank statements, and other unstructured data sets.

Many data providers and websites provide APIs, or Application Program Interfaces, and Web Services, which multiple users or applications can interact with and obtain data for processing or analysis. APIs and Web Services typically listen for incoming requests, which can be in the form of web requests from users or network requests from applications and return data in plain text, XML, HTML, JSON, or media files.

    CASE STUDY: Let’s look at some popular examples of APIs being used as a data source for data analytics: The use of Twitter and Facebook APIs to source data from tweets and posts for performing tasks such as opinion mining or sentiment analysis, which is to summarize the amount of appreciation and criticism on a given subject, such as policies of a government, a product, a service, or customer satisfaction in general. Stock Market APIs used for pulling data such as share and commodity prices, earnings per share, and historical prices, for trading and analysis. Data Lookup and Validation APIs, which can be very useful for Data Analysts for cleaning and preparing data, as well as for co-relating data—for example, to check which city or state a postal or zip code belongs to. APIs are also used for pulling data from database sources, within and external to the organization. Web scraping is used to extract relevant data from unstructured sources. Also known as screen scraping, web harvesting, and web data extraction, web scraping makes it possible to download specific data from web pages based on defined parameters. Web scrapers can, among other things, extract text, contact information, images, videos, product items, and much more from a website. Some popular uses of web scraping include: collecting product details from retailers, manufacturers, and eCommerce websites to provide price comparisons, generating sales leads through public data sources, extracting data from posts and authors on various forums and communities, and collecting training and testing datasets for machine learning models. Some of the popular web scraping tools include BeautifulSoup, Scrapy, Pandas, and Selenium. Data streams are another widely used source for aggregating constant streams of data flowing from sources such as instruments, IoT devices and applications, GPS data from cars, computer programs, websites, and social media posts. This data is generally timestamped and also geo-tagged for geographical identification. Some of the data streams and ways in which they can be leveraged include: stock and market tickers for financial trading, retail transaction streams for predicting demand and supply chain management, surveillance and video feeds for threat detection, social media feeds for sentiment analysis, sensor data feeds for monitoring industrial or farming machinery, web click feeds for monitoring web performance and improving design, and real-time flight events for rebooking and rescheduling. Some popular applications used to process data streams include Apache Kafka, Apache Spark Streaming, and Apache Storm. RSS (or Really Simple Syndication) feeds, are another popular data source. These are typically used for capturing updated data from online forums and news sites where data is refreshed on an ongoing basis. Using a feed reader, which is an interface that converts RSS text files into a stream of updated data, updates are streamed to user devices.


## LANGUAGES ##

These can be categorized as – query languages, programming languages, and shell scripting. 
- Query languages are designed for accessing and manipulating data in a database; for example: SQL.
- Programming languages are designed for developing applications and controlling application behavior; for example: Python, R, and Java.
- Shell and Scripting languages, such as Unix/Linux Shell, and PowerShell, are ideal for repetitive and time-consuming operational tasks.

- SQL (Structured Query Language): Is a querying language designed for accessing and manipulating information from, mostly, though not exclusively, relational databases. Using SQL, we can write a set of instructions to perform operations such as Insert, update, and delete records in a database; Create new databases, tables, and views; and Write stored procedures—which means you can write a set of instructions and call them for later use. Here are some advantages of using SQL:
    · SQL is portable and can be used independent of the platform. It can be used for querying data in a wide variety of databases and data repositories, although each vendor may have some variations and special extensions. 
    · It has a simple syntax that is similar to the English language. Its syntax allows developers to write programs with fewer lines than some of the other programming languages using basic keywords such as select, insert, into, and update. 
    · It can retrieve large amounts of data quickly and efficiently. It runs on an interpreter system, which means code can be executed as soon as it is written, making prototyping quick and easy. 
    · SQL is one of the most popular querying language. Due to its large user community and the sheer volume of documentation accumulated over the years, it continues to provide a uniform platform, worldwide, to all its users. 
    
- PYTHON: Is a widely-used open-source, general-purpose, high-level programming language. Its syntax allows programmers to express their concepts in fewer lines of code, as compared to some of the older languages. Python is perceived as one of the easiest languages to learn and has a large developer community. Because of its focus on simplicity and readability, and a low learning curve, it’s an ideal tool for beginning programmers. It is great for performing high-computational tasks in vast amounts of data, which can otherwise be extremely time-consuming and cumbersome. Python provides libraries like Numpy and Pandas, which eases this task by the use of parallel processing. It has inbuilt functions for almost all of the frequently used concepts. Python supports multiple programming paradigms, such as object-oriented, imperative, functional, and procedural, making it suitable for a wide variety of use cases. 
Now let’s look at some of the reasons that make Python one of the fastest-growing programming languages in the world today: 
    · It is easy to learn: With Python, you have the advantage of using fewer lines of code to accomplish tasks compared to other languages. 
    · It is open-source: Python is free and uses a community-based model for development. 
    · It runs on Windows and Linux environments and can be ported to multiple platforms. 
    · It has widespread community support with plenty of useful analytics libraries available. 
    · It has several open-source libraries for data manipulation, data visualization, statistics, and mathematics, to name just a few. 
    · Its vast array of libraries and functionalities also include: Pandas for data cleaning and analysis, Numpy and Scipy, for statistical analysis, Beautifulsoup and Scrapy for web scraping, Matplotlib and Seaborn to visually represent data in the form of bar graphs, histogram, and pie-charts, Opencv for image processing.

- R : Is an open-source programming language and environment for data analysis, data visualization, machine learning, and statistics. Widely used for developing statistical software and performing data analytics, it is especially known for its ability to create compelling visualizations, giving it an edge over some of the other languages in this space. Some of the key benefits of R include the following: 
    · It is an open-source platform-independent programming language.
    · It can be paired with many programming languages, including Python.
    · It is highly extensible, which means developers can continue to add functionalities by defining new functions.
    · It facilitates the handling of structured as well as unstructured data which means it has a more comprehensive data capability.
    · It has libraries such as Ggplot2 and Plotly that offer aesthetic graphical plots to its users. You can make reports with the data and scripts embedded in them; also, interactive web apps that allow users to play with the results and the data.
    · It is dominant among other programming languages for developing statistical tools. 
    
- JAVA: Is an object-oriented, class-based, and platform-independent programming language originally developed by Sun Microsystems. It is among the top-ranked programming languages used today. Java is used in a number of processes all through data analytics, including cleaning data, importing and exporting data, statistical analysis, and data visualization. In fact, most of the popular frameworks and tools used for big data are typically written in Java, such as Hadoop, Hive, and Spark. It is perfectly suited for speed-critical projects.

- A UNIX / LINUX SHELL: Is a computer program written for the UNIX shell. It is a series of UNIX commands written in a plain text file to accomplish a specific task. Writing a shell script is fast and easy. It is most useful for repetitive tasks that may be time-consuming to execute by typing one line at a time. Typical operations performed by shell scripts include: file manipulation, program execution, system administration tasks such as disk backups and evaluating system logs, installation scripts for complex programs, executing routine backups, running batches, PowerShell is a cross-platform automation tool and configuration framework by Microsoft that is optimized for working with structured data formats, such as JSON, CSV, XML, and REST APIs, websites, and office applications. It consists of a command-line shell and scripting language. PowerShell is object-based, which makes it possible to filter, sort, measure, group, compare, and many more actions on objects as they pass through a data pipeline. It is also a good tool for data mining, building GUIs, and creating charts, dashboards, and interactive reports.



# DATA REPOSITORIES & BIG DATA PLATFORMS #

### SUMMARY & HIGHLIGHTS ###

In this lesson, you have learned the following information: 

A Data Repository is a general term that refers to data that has been collected, organized, and isolated so that it can be used for reporting, analytics, and also for archival purposes.  The different types of Data Repositories include: 

    · Databases, which can be relational or non-relational, each following a set of organizational principles, the types of data they can store, and the tools that can be used to query, organize, and retrieve data.

    · Data Warehouses, that consolidate incoming data into one comprehensive storehouse.  

    · Data Marts, that are essentially sub-sections of a data warehouse, built to isolate data for a particular business function or use case. 

    · Data Lakes, that serve as storage repositories for large amounts of structured, semi-structured, and unstructured data in their native format. 

    · Big Data Stores, that provide distributed computational and storage infrastructure to store, scale, and process very large data sets.


ETL, or Extract Transform and Load, Process is an automated process that converts raw data into analysis-ready data by:

    · Extracting data from source locations.
    · Transforming raw data by cleaning, enriching, standardizing, and validating it.
    · Loading the processed data into a destination system or data repository.

Data Pipeline, sometimes used interchangeably with ETL, encompasses the entire journey of moving data from the source to a destination data lake or application, using the ETL process.  

Big Data refers to the vast amounts of data that is being produced each moment of every day, by people, tools, and machines. The sheer velocity, volume, and variety of data challenge the tools and systems used for conventional data. These challenges led to the emergence of processing tools and platforms designed specifically for Big Data, such as Apache Hadoop, Apache Hive, and Apache Spark.



## OVERVIEW ##

A data repository is a general term used to refer to data that has been collected, organized, and isolated so that it can be used for business operations or mined for reporting and data analysis. It can be a small or large database infrastructure with one or more databases that collect, manage, and store data sets. Such as databases, data warehouses, and big data stores.

- DATABASES: 
    · Is a collection of data, or information, designed for the input, storage, search and retrieval, and modification of data.
    · A Database Management System, or DBMS, is a set of programs that creates and maintains the database. Even though a database and DBMS mean different things the terms are often used interchangeably.
    · It allows you to store, modify, and extract information from the database using a function called querying. 
    · Several factors influence the choice of database, such as the data type and structure, querying mechanisms, latency requirements, transaction speeds, and intended use of the data. It’s important to mention two main types:

     * Relational databases, also referred to as RDBMSes, build on the organizational principles of flat files, with data organized into a tabular format with rows and columns following a well-defined structure and schema. However, unlike flat files, RDBMSes are optimized for data operations and querying involving many tables and much larger data volumes. Structured Query Language, or SQL, is the standard querying language for relational databases.

     * Non-relational databases, also known as NoSQL, or “Not Only SQL”. Them emerged in response to the volume, diversity, and speed at which data is being generated today, mainly influenced by advances in cloud computing, the Internet of Things, and social media proliferation. Built for speed, flexibility, and scale, non-relational databases made it possible to store data in a schema-less or free-form fashion. NoSQL is widely used for processing BIG DATA. A data warehouse works as a central repository that merges information coming from disparate sources and consolidates it through the extract, transform, and load process, also known as the ETL process, into one comprehensive database for analytics and business intelligence. At a very high-level, the ETL process helps you to extract data from different data sources, transform the data into a clean and usable state, and load the data into the enterprise’s data repository. 
     
    · Related to Data Warehouses are the concepts of Data Marts and Data Lakes. Both of them have historically been relational, since much of the traditional enterprise data has resided in RDBMSes. However, with the emergence of NoSQL technologies and new sources of data, non-relational data repositories are also now being used for Data Warehousing. 

    · Another category are Big Data Stores, that include distributed computational and storage infrastructure to store, scale, and process very large data sets. Overall, data repositories help to isolate data and make reporting and analytics more efficient and credible while also serving as a data archive.



## RDBMS ##

- RELATIONAL DATABASE: Is a collection of data organized into a table structure, where the tables can be linked, or related, based on data common to each. Tables are made of rows and columns, where rows are the “records”, and the columns the “attributes”. 

    · Let’s take the example of a customer table that maintains data about each customer in a company. The columns, or attributes, in the customer table are the Company ID, Company Name, Company Address, and Company Primary Phone; and Each row is a customer record. Now let’s understand what we mean by tables being linked, or related, based on data common to each. Along with the customer table, the company also maintains transaction tables that contain data describing multiple individual transactions pertaining to each customer. The columns for the transaction table might include the Transaction Date, Customer ID, Transaction Amount, and Payment Method. The customer table and the transaction tables can be related based on the common Customer ID field. You can query the customer table to produce reports such as a customer statement that consolidates all transactions in a given period. 
    
- This capability of relating tables based on common data enables you to retrieve an entirely new table from data in one or more tables with a single query. It also allows you to understand the relationships among all available data and gain new insights for making better decisions. 

- Relational databases use structured query language, or SQL, for querying data. Them build on the organizational principles of flat files such as spreadsheets, with data organized into rows and columns following a well-defined structure and schema. But this is where the similarity ends. Relational databases, by design, are ideal for the optimized storage, retrieval, and processing of data for large volumes of data, unlike spreadsheets that have a limited number of rows and columns. 

- Each table in a relational database has a unique set of rows and columns and relationships can be defined between tables, which minimizes data redundancy. Moreover, you can restrict database fields to specific data types and values, which minimizes irregularities and leads to greater consistency and data integrity. 

- Them use SQL for querying data, which gives you the advantage of processing millions of records and retrieving large amounts of data in a matter of seconds. Moreover, the security architecture of relational databases provides controlled access to data and also ensures that the standards and policies for governing data can be enforced. 

- Them range from small desktop systems to massive cloud-based systems. They can be either: 
    · Open-source and internally supported, open-source with commercial support, or commercial closed-source systems. IBM DB2, Microsoft SQL Server, MySQL, Oracle Database, and PostgreSQL are some of the popular relational databases. 
    · Cloud-based relational databases, also referred to as Database-as-a-Service: are gaining wide use as they have access to the limitless compute and storage capabilities offered by the cloud. Some of the popular cloud relational databases include Amazon Relational Database Service (RDS), Google Cloud SQL, IBM DB2 on Cloud, Oracle Cloud, and SQL Azure. 

- RDBMS is a mature and well-documented technology, making it easy to learn and find qualified talent. One of the most significant advantages of the relational database approach is its ability to create meaningful information by joining tables. 
Some of its other advantages include: 
    · Flexibility: Using SQL, you can add new columns, add new tables, rename relations, and make other changes while the database is running and queries are happening. 
    · Reduced redundancy: Relational databases minimize data redundancy. For example, the information of a customer appears in a single entry in the customer table, and the transaction table pertaining to the customer stores a link to the customer table. 
    · Ease of backup and disaster recovery: Relational databases offer easy export and import options, making backup and restore easy. Exports can happen while the database is running, making restore on failure easy. Cloud-based relational databases do continuous mirroring, which means the loss of data on restore can be measured in seconds or less. 
    · ACID-compliance: ACID stands for Atomicity, Consistency, Isolation, and Durability. And ACID compliance implies that the data in the database remains accurate and consistent despite failures, and database transactions are processed reliably. 
    
USE CASES:

· Online Transaction Processing: OLTP applications are focused on transaction-oriented tasks that run at high rates. Relational databases are well suited for OLTP applications because they can accommodate a large number of users; they support the ability to insert, update, or delete small amounts of data; and they also support frequent queries and updates as well as fast response times. 

· Data warehouses: In a data warehousing environment, relational databases can be optimized for online analytical processing (or OLAP), where historical data is analyzed for business intelligence. 

· IoT solutions: Internet of Things (IoT) solutions require speed as well as the ability to collect and process data from edge devices, which need a lightweight database solution. This brings us to the limitations of RDBMS: RDBMS does not work well with semi-structured and unstructured data and is, therefore, not suitable for extensive analytics on such data. For migration between two RDBMSs, schemas and type of data need to be identical between the source and destination tables. Relational databases have a limit on the length of data fields, which means if you try to enter more information into a field than it can accommodate, the information will not be stored. 

> " Despite the limitations and the evolution of data in these times of big data, cloud computing, IoT devices, and social media, RDBMS continues to be the predominant technology for working with structured data. "



## NoSQL ##

- NoSQL, which stands for “not only SQL,” or sometimes “non SQL”: is a non-relational database design that provides flexible schemas for the storage and retrieval of data. 

- NoSQL databases have existed for many years but have only recently become more popular in the era of cloud, big data, and high-volume web and mobile applications. They are chosen today for their attributes around scale, performance, and ease of use. It's important to emphasize that the "No" in "NoSQL" is an abbreviation for "not only" and not the actual word "No." 

- NoSQL databases are built for specific data models and have flexible schemas that allow programmers to create and manage modern applications. They do not use a traditional row/column/table database design with fixed schemas, and typically not use the structured query language (or SQL) to query data, although some may support SQL or SQL-like interfaces. NoSQL allows data to be stored in a schema-less or free-form fashion. Any data, be It structured, semi-structured, or unstructured, can be stored in any record. 

- Based on the model being used for storing data, there are four common types of NoSQL databases. Key-value store, document-based, column-based, and graph-based. 

    · Key-value store. Data in a key-value database is stored as a collection of key-value pairs. The key represents an attribute of the data and is a unique identifier. Both keys and values can be anything from simple integers or strings to complex JSON documents. Key-value stores are great for storing user session data and user preferences, making real-time recommendations and targeted advertising, and in-memory data caching. However, if you want to be able to query the data on specific data value, need relationships between data values, or need to have multiple unique keys, a key-value store may not be the best fit. Redis, Memcached, and DynamoDB are some well-known examples in this category. 
    
    · Document-based: Document databases store each record and its associated data within a single document. They enable flexible indexing, powerful ad hoc queries, and analytics over collections of documents. Document databases are preferable for eCommerce platforms, medical records storage, CRM platforms, and analytics platforms. However, if you’re looking to run complex search queries and multi-operation transactions, a document-based database may not be the best option for you. MongoDB, DocumentDB, CouchDB, and Cloudant are some of the popular document-based databases.

    · Column-based: Column-based models store data in cells grouped as columns of data instead of rows. A logical grouping of columns, that is, columns that are usually accessed together, is called a column family. For example, a customer’s name and profile information will most likely be accessed together but not their purchase history. So, customer name and profile information data can be grouped into a column family. Since column databases store all cells corresponding to a column as a continuous disk entry, accessing and searching the data becomes very fast. Column databases can be great for systems that require heavy write requests, storing time-series data, weather data, and IoT data. But if you need to use complex queries or change your querying patterns frequently, this may not be the best option for you. The most popular column databases are Cassandra and HBase. 
    
    · Graph-based: Graph-based databases use a graphical model to represent and store data. They are particularly useful for visualizing, analyzing, and finding connections between different pieces of data. The circles are nodes, and they contain the data. The arrows represent relationships. Graph databases are an excellent choice for working with connected data, which is data that contains lots of interconnected relationships. Graph databases are great for social networks, real-time product recommendations, network diagrams, fraud detection, and access management. But if you want to process high volumes of transactions, it may not be the best choice for you, because graph databases are not optimized for large-volume analytics queries. Neo4J and CosmosDB are some of the more popular graph databases. 


- NoSQL was created in response to the limitations of traditional relational database technology. The primary advantage of NoSQL is its ability to handle large volumes of structured, semi-structured, and unstructured data. Some of its other advantages include: 
    · The ability to run as distributed systems scaled across multiple data centers, which enables them to take advantage of cloud computing infrastructure; 
    · An efficient and cost-effective scale-out architecture that provides additional capacity and performance with the addition of new nodes; and 
    · Simpler design, better control over availability, and improved scalability that enables you to be more agile, more flexible, and to iterate more quickly. 
    
> To summarize the key differences between relational and non-relational databases: RDBMS schemas rigidly define how all data inserted into the database must be typed and composed, whereas NoSQL databases can be schema-agnostic, allowing unstructured and semi-structured data to be stored and manipulated. Maintaining high-end, commercial relational database management systems is expensive whereas NoSQL databases are specifically designed for low-cost commodity hardware. Relational databases, unlike most NoSQL, support ACID-compliance, which ensures reliability of transactions and crash recovery. RDBMS is a mature and well-documented technology, which means the risks are more or less perceivable as compared to NoSQL, which is a relatively newer technology. Nonetheless, NoSQL databases are here to stay, and are increasingly being used for mission critical applications.



## DATA MARTS, DATA LAKES, ETL, DATA PIPELINES ##

> Earlier in the course, we examined databases, data warehouses, and big data stores. Now we’ll go a little deeper in our exploration of data warehouses, data marts, and data lakes; and also learn about the ETL process and data pipelines. 

- A DATA WAREHOUSE works like a multi-purpose storage for different use cases. By the time the data comes into the warehouse, it has already been modeled and structured for a specific purpose, meaning it is analysis ready. As an organization, you would opt for a data warehouse when you have massive amounts of data from your operational systems that needs to be readily available for reporting and analysis. Them serve as the single source of truth—storing current and historical data that has been cleansed, conformed, and categorized. 

- A data warehouse is a multi-purpose enabler of operational and performance analytics. A DATA MART is a sub-section of the data warehouse, built specifically for a particular business function, purpose, or community of users. The idea is to provide stakeholders data that is most relevant to them, when they need it. For example, the sales or finance teams accessing data for their quarterly reporting and projections. Since a data mart offers analytical capabilities for a restricted area of the data warehouse, it offers isolated security and isolated performance. The most important role of a data mart is business-specific reporting and analytics. 

- A DATA LAKE is a storage repository that can store large amounts of structured, semi-structured, and unstructured data in their native format, classified and tagged with metadata. So, while a data warehouse stores data processed for a specific need, a data lake is a pool of raw data where each data element is given a unique identifier and is tagged with metatags for further use. You would opt for a data lake if you generate, or have access to, large volumes of data on an ongoing basis, but don’t want to be restricted to specific or pre-defined use cases. Unlike data warehouses, a data lake would retain all source data, without any exclusions. And the data could include all types of data sources and types. Data lakes are sometimes also used as a staging area of a data warehouse. The most important role of a data lake is in predictive and advanced analytics. 

- Now we come to the process that is at the heart of gaining value from data: the Extract, Transform, and Load process, or ETL.

    · ETL is how raw data is converted into analysis-ready data. It is an automated process in which you gather raw data from identified sources, extract the information that aligns with your reporting and analysis needs, clean, standardize, and transform that data into a format that is usable in the context of your organization; and load it into a data repository. While ETL is a generic process, the actual job can be very different in usage, utility, and complexity.

    · EXTRACT is the step where data from source locations is collected for transformation. Data extraction could be through: 
        * Batch processing: meaning source data, is moved in large chunks from the source to the target system at scheduled intervals. Tools for batch processing include Stitch and Blendo. 
        * Stream processing, which means source data is pulled in real-time from the source and transformed while it is in transit and before it is loaded into the data repository. Tools for stream processing include Apache Samza, Apache Storm, and Apache Kafka. 
        
    · TRANSFORM involves the execution of rules and functions that converts raw data into data that can be used for analysis. For example, making date formats and units of measurement consistent across all sourced data, removing duplicate data, filtering out data that you do not need, enriching data, for example, splitting full name to first, middle, and last names, establishing key relationships across tables, applying business rules and data validations. 
    
    · LOAD is the step where processed data is transported to a destination system or data repository. It could be: 
        * Initial loading, that is, populating all the data in the repository, 
        * Incremental loading, that is, applying ongoing updates and modifications as needed periodically; or 
        * Full refresh, that is, erasing contents of one or more tables and reloading with fresh data. 
    Load verification, which includes data checks for missing or null values, server performance, and monitoring load failures, are important parts of this process step. It is vital to keep an eye on load failures and ensure the right recovery mechanisms are in place. 

  
- It’s common to see the terms ETL and data pipelines used interchangeably. And although both move data from source to destination, DATA PIPELINE is a broader term that encompasses the entire journey of moving data from one system to another, of which ETL is a subset. Data pipelines can be architected for batch processing, for streaming data, and a combination of batch and streaming data. In the case of streaming data, data processing or transformation, happens in a continuous flow. This is particularly useful for data that needs constant updating, such as data from a sensor monitoring traffic. A data pipeline is a high performing system that supports both long-running batch queries and smaller interactive queries. The destination for a data pipeline is typically a data lake, although the data may also be loaded to different target destinations, such as another application or a visualization tool. The most popular among available solutions being Apache Beam and DataFlow.



## FOUNDATIONS OF BIG DATA ##

> In this digital world, everyone leaves a trace. From our travel habits to our workouts and entertainment, the increasing number of internet connected devices that we interact with on a daily basis record vast amounts of data about us there's even a name for it Big Data.

- BIG DATA: refers to the dynamic, large, and disparate volumes of data being created by people, tools, and machines. 

- It requires new, innovative and scalable technology to collect, host, and analytically process the vast amount of data gathered in order to drive real-time business insights that relate to consumers, risk, profit, performance, productivity management, and enhanced shareholder value. There is no one definition of big data but there are certain elements that are common across the different definitions, such as velocity, volume, variety, veracity, and value. These are the V's of big data:

    · Velocity is the speed at which data accumulates. Data is being generated extremely fast in a process that never stops. Near or real-time streaming, local, and cloud-based technologies can process information very quickly. 

    · Volume is the scale of the data or the increase in the amount of data stored. Drivers of volume are the increase in data sources, higher resolution sensors, and scalable infrastructure. 

    · Variety is the diversity of the data. Structured data fits neatly into rows and columns in relational databases, while unstructured data is not organized in a predefined way like tweets, blog posts, pictures, numbers, and video. Variety also reflects that data comes from different sources; machines, people, and processes, both internal and external to organizations. Drivers are mobile technologies social media, wearable technologies, geo technologies video, and many, many more. 

    · Veracity is the quality and origin of data and its conformity to facts and accuracy. Attributes include consistency, completeness, integrity, and ambiguity. Drivers include cost and the need for traceability. With the large amount of data available, the debate rages on about the accuracy of data in the digital age. Is the information real or is it false? 
    
    · Value is our ability and need to turn data into value. Value isn't just profit. It may have medical or social benefits, as well as customer, employee or personal satisfaction. The main reason that people invest time to understand big data is to derive value from it. 
    
    
- USE CASES: Let's look at some examples of the V's in action. 
    · Velocity: Every 60 seconds, hours of footage are uploaded to YouTube, which is generating data. Think about how quickly data accumulates over hours, days, and years. 
    · Volume: The world population is approximately 7 billion people and the vast majority are now using digital devices. Mobile phones, desktop and laptop computers, wearable devices, and so on. These devices all generate, capture, and store data approximately 2.5 quintillion bytes every day. That's the equivalent of 10 million blu-ray DVDs. 
    · Variety: Let's think about the different types of data. Text, pictures, film, sound, health data from wearable devices, and many different types of data from devices connected to the internet of things. 
    · Veracity. Eighty percent of data is considered to be unstructured and we must devise ways to produce reliable and accurate insights. The data must be categorized, analyzed, and visualized.
    

> Data scientists, today, derive insights from big data and cope with the challenges that these massive data sets present. The scale of the data being collected means that it's not feasible to use conventional data analysis tools, however, alternative tools that leverage distributed computing power can overcome this problem. TOOLS such as Apache Spark, Hadoop, and its ecosystem provides ways to extract, load, analyze, and process the data across distributed compute resources, providing new insights and knowledge. This gives organizations more ways to connect with their customers and enrich the services they offer.


## BIG DATA PROCESSING TOOLS ##

- The Big Data processing technologies provide ways to work with large sets of structured, semi-structured, and unstructured data so that VALUE can be derived from big data. 

We are going to talk about three open source technologies and the role they play in big data analytics: 

> HADOPP is a collection of tools that provides distributed storage and processing of big data. HIVE is a data warehouse for data query and analysis built on top of Hadoop. SPARK is a distributed data analytics framework designed to perform complex data analytics in real-time.


- APACHE HADOOP:  a java-based open-source framework, allows distributed storage and processing of large datasets across clusters of computers. In Hadoop distributed system, a node is a single computer, and a collection of nodes forms a cluster. It can scale up from a single node to any number of nodes, each offering local storage and computation. Hadoop provides a reliable, scalable, and cost-effective solution for storing data with no format requirements. Using Hadoop, you can: 
    · Incorporate emerging data formats, such as streaming audio, video, social media sentiment, and clickstream data, along with structured, semi-structured, and unstructured data not traditionally used in a data warehouse. 
    · Provide real-time, self-service access for all stakeholders. 
    · Optimize and streamline costs in your enterprise data warehouse by consolidating data across the organization and moving “cold” data, that is, data that is not in frequent use, to a Hadoop-based system. 
    
One of the four main components of Hadoop is Hadoop Distributed File System, or HDFS, which is a storage system for big data that runs on multiple commodity hardware connected through a network. HDFS provides scalable and reliable big data storage by partitioning files over multiple nodes. It splits large files across multiple computers, allowing parallel access to them. Computations can, therefore, run in parallel on each node where data is stored. It also replicates file blocks on different nodes to prevent data loss, making it fault-tolerant. 
    Let’s understand this through an EXAMPLE: Consider a file that includes phone numbers for everyone in the United States; the numbers for people with last name starting with A might be stored on server 1, B on server 2, and so on. With Hadoop, pieces of this phonebook would be stored across the cluster. To reconstruct the entire phonebook, your program would need the blocks from every server in the cluster. HDFS also replicates these smaller pieces onto two additional servers by default, ensuring availability when a server fails. In addition to higher availability, this offers multiple benefits. It allows the Hadoop cluster to break up work into smaller chunks and run those jobs on all servers in the cluster for better scalability. Finally, you gain the benefit of data locality, which is the process of moving the computation closer to the node on which the data resides. 
    
This is critical when working with large data sets because it minimizes network congestion and increases throughput. Some of the other benefits that come from using HDFS include: 
    · Fast recovery from hardware failures, because HDFS is built to detect faults and automatically recover. 
    · Access to streaming data, because HDFS supports high data throughput rates. 
    · Accommodation of large data sets, because HDFS can scale to hundreds of nodes, or computers, in a single cluster. 
    · Portability, because HDFS is portable across multiple hardware platforms and compatible with a variety of underlying operating systems. 


- APACHE HIVE: is an open-source data warehouse software for reading, writing, and managing large data set files that are stored directly in either HDFS or other data storage systems such as Apache HBase. Hadoop is intended for long sequential scans and, because Hive is based on Hadoop, queries have very high latency—which means Hive is less appropriate for applications that need very fast response times. Hive is not suitable for transaction processing that typically involves a high percentage of write operations. Hive is better suited for data warehousing tasks such as ETL, reporting, and data analysis and includes tools that enable easy access to data via SQL. 


- APACHE SPARKS: a general-purpose data processing engine designed to extract and process large volumes of data for a wide range of applications, including Interactive Analytics, Streams Processing, Machine Learning, Data Integration, and ETL. It takes advantage of in-memory processing to significantly increase the speed of computations and spilling to disk only when memory is constrained. Spark has interfaces for major programming languages, including Java, Scala, Python, R, and SQL. It can run using its standalone clustering technology as well as on top of other infrastructures such as Hadoop. And it can access data in a large variety of data sources, including HDFS and Hive, making it highly versatile. The ability to process streaming data fast and perform complex analytics in real-time is the key use case for Apache Spark.

