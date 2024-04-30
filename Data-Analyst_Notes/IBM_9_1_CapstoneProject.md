
# CAPSTONE PROJECT #

## INTRODUCTION ##

### WELCOME / SYLLABUS

Congratulations on making it this far!
Successfully completing this Capstone project will earn you the Data Analyst Professional
Certificate.
This Capstone provides you a practical hands on experience to demonstrate all of the skills
you have picked up so far in this Professional Certificate program.
As part of the capstone project, you will take on the role of a Data Analyst with a
global IT and Business Services firm.
In this role, you will be analyzing several datasets to help identify trends for emerging
technologies.
In Module 1 you will collect data for the technology skills that are in demand from
various sources including:
Job postings, blog posts, surveys.
In Module 2, you will take the collected data and prepare it for analysis by using data
wrangling techniques like:
Finding duplicates, removing duplicates, finding missing values, and inputting missing values.
You’ll continue to module 3 and apply statistical techniques to analyze the data and identify
insights and trends like:
What are the top programming languages that are in demand?
What are the top database skills that are in demand?
What are the most popular IDEs?
And
Demographic data like gender and age distribution of developers.
In module 4, you’ll focus on choosing an appropriate visualization based on the data
you want to present using charts, plots, and histograms to help reveal your findings and
trends.
In module 5, you will employ Cognos to create interactive dashboards to help you analyze
and present the data dynamically.
In the final module, you will use your storytelling skills to provide a narrative and present
the findings of your analysis.
You will be provided with a presentation template to begin the process and to help you create
a compelling story and present your findings.
Each module includes a short quiz to test your knowledge.
You will be evaluated based on the quizzes in each module.
The dashboard and the storytelling presentation you create that will be reviewed and graded
by your peers.
To begin, I recommend taking a few minutes to explore the course site.
Review the material we’ll cover each week and preview the assignments you’ll need
to complete to pass the course.
Click “Discussions” to see forums where you can discuss the course material with fellow
learners and course team.
If you have questions about course content, please post them in the forums to get help
from others in the course community.
For technical problems with the Coursera platform, visit the Learner Help Center.
We are excited to have you join us and hope you enjoy the course.
Good luck and let’s get started! 


### THE PROJECT

You have recently been hired as a Data Analyst by a global IT and business consulting services firm that is known for their expertise in IT solutions and their team of highly experienced IT consultants.  In order to keep pace with changing technologies and remain competitive, your organization regularly analyzes data to help identify future skill requirements. 

As a Data Analyst, you will be assisting with this initiative and have been tasked with collecting data from various sources and identifying trends for this year's report on emerging skills. 

Your first task is to collect the top programming skills that are most in demand from various sources including: Job postings, Training portals and Surveys.

Once you have collected enough data, you will begin analyzing the data and identify insights and trends that may include the following: What are the top programming languages in demand? What are the top database skills in demand? What are the popular IDEs?

You will begin by scraping internet web sites and accessing APIs to collect data in various formats like .csv files, excel sheets, and databases.   

Once this is completed, you will make that data ready for analysis using data wrangling techniques. 

When the data is ready you will then want to apply statistical techniques to analyze the data.  Then bring all of your information together by using  IBM Cognos Analytics to create your dashboard. And finally, show off your storytelling skills by sharing your findings in a presentation.

You will be evaluated using quizzes in each module as well as the final project presentation.



## DATA COLLECTION ##

Data Collection is the first step in solving any analysis problem and can be collected in many formats and from many sources. In the first module of the Capstone, we will collect data by scraping the internet and using web APIs.

Learning Objectives:

    - Work with data in different formats.
    - Collect data from various sources.

### COLLECTING DATA USING APIs

In the coming future data will increasingly be shared using Application Programming Interfaces (APIs).

An API is hosted on the public internet or a private network. APIs provide anytime access to the latest data.

Your assignment is to get the number of job openings using the GitHub Jobs API for technologies like: Java, Python, MySQL, C++, C#

GitHub Jobs API allows anyone to query for the jobs based upon:
- Technology like Python, MySQL
- City like New York, Bangalore

Here are the technical details to access the API.

The GitHub Jobs API allows you to search, and view jobs with JSON over HTTP.

To get the JSON representation of any search result or job listing, append .json to the URL you’d use on the HTML GitHub Jobs site.

For example, below url will search for Python jobs near New York:

https://jobs.github.com/positions?description=python&location=new+york

To get the JSON representation of those jobs, just use positions.json:

https://jobs.github.com/positions.json?description=python&location=new+york

---

PAGINATION

The API also supports pagination. /positions.json, for example, will only return 50 positions at a time. You can paginate results by adding a page parameter to your queries.

Pagination starts by default at 0.

EXAMPLES

https://jobs.github.com/positions.json?description=ruby&page=1

https://jobs.github.com/positions.json?page=1&search=code

---

GET /positions.json

Search for jobs by term, location, full time vs part time, or any combination of the three. All parameters are optional.

PARAMETERS

    description — A search term, such as “ruby” or “java”. This parameter is aliased to search.
    location — A city name, zip code, or other location search term.
    lat — A specific latitude. If used, you must also send long and must not send location.
    long — A specific longitude. If used, you must also send lat and must not send location.
    full_time — If you want to limit results to full time positions set this parameter to ‘true’.

EXAMPLES

https://jobs.github.com/positions.json?description=python&full_time=true&location=sf

https://jobs.github.com/positions.json?search=node

https://jobs.github.com/positions.json?lat=37.3229978&long=-122.0321823

---

GET /positions/ID.json

Retrieve the JSON representation of a single job posting.

PARAMETERS

    markdown — Set to ‘true’ to get the description and how_to_apply fields as Markdown.

EXAMPLES

https://jobs.github.com/positions/21516.json

https://jobs.github.com/positions/21516.json?markdown=true


### COLLECTING DATA USING WEBSCRAPING

### EXPLORING DATA

Stack Overflow, a popular website for developers, conducted an online survey of software professionals across the world. The survey data was later open sourced by Stack Overflow. The actual data set has around 90,000 responses.

The dataset you are going to use in this assignment comes from the following source: https://stackoverflow.blog/2019/04/09/the-2019-stack-overflow-developer-survey-results-are-in/ under a ODbL: Open Database License.

You will be given a subset of the original data set in this capstone project. You will explore, analyze, and visualize this dataset and present your analysis.

Note: This randomised subset contains around 1/10th of the original data set. Any conclusions you draw after analyzing this subset may not reflect the real world scenario.


## DATA WRANGLING ##

In this module, you will be focusing on the cleaning of your dataset with various techniques. With these techniques you will be identifying duplicate rows, finding missing values, and normalizing the data.

Learning Objectives:

    - Identify duplicate values in the dataset.
    - Remove duplicate values from the dataset.
    - Identify missing values in the dataset.
    - Determine the missing values in the dataset.
    - Normalize data in the dataset.

ASSINGMENT OVERVIEW,

Data Wrangling or Munging is a process in which we clean up the data set and make it ready for data analysis. In this assignment you will perform the following tasks:

    - Identify duplicate rows in the data frame.
    - Remove duplicate rows from the dataframe.
    - Find the number of missing values for all columns.
    - Find the value counts for the column "Employment".
    - Normalize the data using two existing columns.  

### FINDING MISSING VALUES

### DETERMINE MISSING VALUES

### FINDING DUPLICATES

### REMOVING DUPLICATES

### NORMALIZING DATA



## EXPLORATORY DATA ANALYSIS ##

In this module, begin working with the cleaned dataset from the previous module. You will now begin to analyze the dataset to find the distribution of data, presence of outliers and the correlation between different columns.

Learning Objectives:

    - Examine the distribution of data in the dataset.
    - Identify the outliers in the dataset.
    - Remove outliers from the dataset.
    - Recognize the correlation between features in the dataset.


ASSIGNMENT OVERVIEW,

After cleaning the dataset, your next step is the analysis. In this stage you will become more familiar with the data set and it will start to take shape. In this assignment you will:

    - Plot a distribution curve, and histogram.
    - Find the median, and outliers of particular columns.
    - Compute the Inter Quartile Range.
    - Find out the upper and lower bounds, and find correlations between numerical columns.
    - Create a new dataframe.

### DISTRIBUTION

### OUTLIERS

### CORRELATION



## DATA VISUALIZATION ##

In module 4 of the Capstone, you will be required to create visualizations using the developer survey data. The visualizations you create should highlight the distribution of data, relationships between data, the composition of data, and comparison of data.

Learning Objectives:

    - Visualize distribution of data.
    - Visualize the relationship between two features.
    - Visualize composition of data.
    - Display the comparison of data series using line and stacked bar charts.


ASSINGMENT OVERVIEW,

In this assignment you will now show off your visualization skills by working with the Stack Overflow Developer Survey 2019 dataset. In this assignment you will:

    - Create a histogram to show the distribution of data.

    - Create different plots such as a scatter, bubble or boxplot.

    - Create a pie chart, bar chart, and stacked chart to show medians and counts.

### VISUALIZING DISTRIBUTION OF DATA

### RELATIONSHIP

### COMPOSITION

### COMPARISON



## DASHBOARD CREATION ##

In this module, you will create a dashboard using IBM Cognos Analytics. This platform will give you the ability to create various charts while assembling a dashboard that is appealing and easy to understand. Your dashboard will contain your data analysis, which should be intuitive and allow for the drill-down of data.

Learning Objectives:

    - Utilize the features in IBM Cognos to improve your charts.
    - Demonstrate the use of correct chart types to use to visualize data.
    - Create a dashboard that helps visualize the key points of the survey dataset.

### DASHBOARDS

ASSIGNMENT OVERVIEW,

In this assignment you will continue working with the Stack Overflow Developer Survey 2019 data to create a dashboard. In this dashboard you will create the following:

A Current Technology Usage tab containing:
    - Top 10 Languages
    - Top 10 Databases
    - Platforms
    - Top 10 WebFrames

A Future Technology Trends tab containing:
    - Top 10 Languages desired for the next year
    - Top 10 Databases desired for the next year
    - Desired platforms for the next year
    - Top 10 WebFrames desired for the next year

A Demographics tab containing:
    - Respondent classified by gender
    - Respondent count for countries
    - Respondent count by age
    - Respondent count by gender and classified by education level



## PRESENTATION OF FINDINGS ##

You have analyzed the data in the previous modules, and now it is time to demonstrate your storytelling skills. In this module, you will create a compelling story that helps to clarify your analysis in an easy-to-understand presentation.

Learning Objectives:

    - Create a compelling story of the analysis
    - Present your findings using visualizations
    - Present your analysis

### HOW TO PRESENT YOUR FINDINGS

### Elements Of A Successful Data Findings Report

While finding and cleaning data is an important first step in data analysis, a concept can
be lost if you are not able to organize and represent the findings effectively to your
audience.
In this video, you will learn how to represent your findings by focusing on specific elements
to create a successful data findings report.
After the data has been collected, cleaned, and organized the work of interpretation begins.
You are now able to obtain a complete view of the data and hopefully, answer the questions
that were formed before starting the analysis.
Now, you typically begin to compose a findings report that explains what was learned.
Depending on the stakeholders and how they receive the information, your report could
vary in form.
This could include a paper style report, a slideshow presentation, or maybe even both.
The findings report is a crucial part of data analysis, as it conveys what was discovered.
When beginning this process, the collected data and information may seem a little overwhelming.
The best way to get through this block is to begin by creating an outline.
By completing an outline, you can then get a complete picture and begin to write in a
precise but simple manner.
While there are many different formats for creating a data-driven presentation, we have
created a simple outline that is easy to follow yet effective.
When creating your outline always remember to structure it towards your audience and
create a presentation that is appropriate for your situation.
You first begin with your cover page.
This beginning section will have the title of your presentation, your name, and then
the date.
The next section in your outline will be an executive summary and then the table of contents.
The table of contents will contain the sections and subsections of your report in order to
give your audience an overview of the contents.
This also enables readers to go directly to a specific section that may be more important
to them.
Continue your presentation with the introduction, methodology, results, discussion, conclusion,
and finally the appendix.
Please note the depth and length for each element may vary depending on the audience
and format of report.
The first step in creating your report is properly creating an executive summary.
This summary will briefly explain the details of the project and should be considered a
stand-alone document.
This information is taken from the main points of your report and while it is acceptable
to repeat information, no new information is presented.
The next section, after the table of contents, is the introduction.
The introduction explains the nature of the analysis, states the problem, and gives the
questions that were to be answered by performing the analysis.
The next section is methodology.
Methodology explains the data sources that were used in the analysis and outlines the
plan for the collected data.
For example, was the cluster or regression method used to analyze the data?
Next, we have the results section.
This section goes into the detail of the data collection, how it was organized, and how
it was analyzed.
This portion would also contain the charts and graphs that would substantiate the results
and call attention to the more complex or crucial findings.
By providing this interpretation of data, you are able to give a detailed explanation
to the audience and how it relates to the problem that was stated in the introduction.
Next is the discussion of the report findings and implications.
For this section you would begin to engage the audience with a discussion of your implications
that were drawn from the research.
For example, let’s say you were conducting research for top programming languages for
college graduates.
Would you find they need to learn multiple languages to remain competitive in the job
market, or would one language always reign supreme?
We have now reached the conclusion of the report findings.
This final section should reiterate the problem given in the introduction and gives an overall
summary of the findings.
It would also state the outcome of the analysis and if any other steps would be taken in the
future.
Lastly, we have the appendix.
This section would contain information that really didn’t fit in the main body of the
report, but you deemed it was still important enough to include.
This type of information could include locations where the raw data was collected or other
details such as resources, acknowledgements or references.
In this video, we learned about the important elements in creating a successful data findings
report.
In the next video, we will learn the best practices when presenting your findings. 


### Best Practices For Presenting Your Findings

Okay, you’ve spent weeks, maybe months, studying the data and the time has come to report your
findings.
The questions have been answered, and you feel good about the story.
How will you speak to your audience so they leave with the intended message?
In this video, learn how to present your findings in a way that will engage and keep the attention
of your audience.
Delivering data-driven presentations may seem easy, but there are a few important factors
to remember in accurately conveying your message.
Make sure charts and graphs are not too small and are clearly labeled,
Use the data only as supporting evidence,
Share only one point from each chart or graph, and
Eliminate data that does not support the key message.
Have you ever sat through a presentation and the information being presented was difficult
to read or understand?
While this may seem apparent, small charts and labels can be easily overlooked.
Make sure to test the visualizations by sitting at different distances, similar to your audience,
and if the data cannot be seen clearly then maybe a redesign should be considered.
When preparing the report, you may feel the only way to explain the findings is to pack
the slides with data.
While this may seem sensible as a data analyst, your audience will probably not appreciate
the intricacies of the data and just see a pile of numbers.
To resolve this issue, begin by forming the key messages that need to be conveyed to the
audience and build the story around these messages.
After forming the outline, go back and insert the data to support your findings.
By not relying heavily on the data and using this method to create the presentation, you
will create a story that is engaging and interesting to your audience.
Presenting your data using charts and graphs is the best way to get your message across
to the audience, however, if you are supplying too much information it can be confusing.
For example, looking at this pie chart, can you decipher what the key message is, and
what the presenter is trying to convey?
In the example, the chart has so much information it is hard to determine what point the presenter
is trying to make and what the focus should be for the audience.
By sticking with one idea and not summarizing multiple points into one visualization, you
are able to accurately convey the idea to the audience and avoid any confusion.
Data analysts can spend months researching data, however, some items that seem interesting
to the analyst may not be relevant to the project.
Trying to explain every little detail to your audience and not recognizing irrelevant data
could damage the key message.
By eliminating this unnecessary data and highlighting only data points that support your key ideas,
you will keep the presentation clear and concise.
In this video, we learned about creating a data-driven presentation that will keep the
audience engaged and how to deliver a clear and concise message. 


### Structure Of A Report

Before starting the analysis, think about the structure of the report. Will it be a brief report of five or fewer pages, or will it be a longer document running more than 100 pages in length? The structure of the report depends on the length of the document. A brief report is more to the point and presents a summary of key findings. A detailed report incrementally builds the argument and contains details about other relevant works, research methodology, data sources, and intermediate findings along with the main results.

I have reviewed reports by leading consultants including Deloitte and McKinsey. I found that the length of the reports varied depending largely on the purpose of the report. Brief reports were drafted as commentaries on current trends and developments that attracted public or media attention. Detailed and comprehensive reports offered a critical review of the subject matter with extensive data analysis and commentary. Often, detailed reports collected new data or interviewed industry experts to answer the research questions.

Even if you expect the report to be brief, sporting five or fewer pages, I recommend that the deliverable follow a prescribed format including the cover page, table of contents, executive summary, detailed contents, acknowledgments, references, and appendices (if needed).

I often find the cover page to be missing in documents. It is not the inexperience of undergraduate students that is reflected in submissions that usually miss the cover page. In fact, doctoral candidates also require an explicit reminder to include an informative cover page. I hasten to mention that the business world sleuths are hardly any better. Just search the Internet for reports and you will find plenty of reports from reputed firms that are missing the cover page.

At a minimum, the cover page should include the title of the report, names of authors, their affiliations, and contacts, the name of the institutional publisher (if any), and the date of publication. I have seen numerous reports missing the date of publication, making it impossible to cite them without the year and month of publication. Also, from a business point of view, authors should make it easier for the reader to reach out to them. Having contact details at the front makes the task easier.

"A table of contents (ToC)" is like a map needed for a trip never taken before. You need to have a sense of the journey before embarking on it. A map provides a visual proxy for the actual travel with details about the landmarks that you will pass by in your trip. The ToC with main headings and lists of tables and figures offers a glimpse of what lies ahead in the document. Never shy away from including a ToC, especially if your document, excluding cover page, table of contents, and references, is five or more pages in length.

Even for a short document, I recommend an "abstract" or an "executive summary". Nothing is more powerful than explaining the crux of your arguments in three paragraphs or less. Of course, for larger documents running a few hundred pages, the executive summary could be longer.

An "introductory section" is always helpful in setting up the problem for the reader who might be new to the topic and who might need to be gently introduced to the subject matter before being immersed in intricate details. A good follow-up to the introductory section is a review of available relevant research on the subject matter. The length of the literature review section depends upon how contested the subject matter is. In instances where the vast majority of researchers have concluded in one direction, the literature review could be brief with citations for only the most influential authors on the subject. On the other hand, if the arguments are more nuanced with caveats aplenty, then you must cite the relevant research to offer adequate context before you embark on your analysis. You might use the literature review to highlight gaps in the existing knowledge, which your analysis will try to fill. This is where you formally introduce your research questions and hypothesis.

In the "methodology" section, you introduce the research methods and data sources you used for the analysis. If you have collected new data, explain the data collection exercise in some detail. You will refer to the literature review to bolster your choice for variables, data, and methods and how they will help you answer your research questions.

The results section is where you present your empirical findings. Starting with descriptive statistics (see Chapter 4, "Serving Tables") and illustrative graphics (see Chapter S, "Graphic Details" for plots and Chapter 10, "Spatial Data Analytics" for maps), you will move toward formally testing your hypothesis (see Chapter 6, "Hypothetically Speaking").

In case you need to run statistical models, you might turn to regression models (see Chapter 7, "Why Tall Parents Don't Have Even Taller Children") or categorical analysis (see Chapters 8, "To Be or Not to Be" and 2., "Categorically Speaking About Categorical Data"). If you are working with time-series data, you can turn to Chapter 11, Doing Serious Time with Time Series. You can also report results from other empirical techniques that fall under the general rubric of data mining (see Chapter 12, "Data Mining for Gold"). Note that many reports in the business sector present results in a more palatable fashion by holding back the statistical details and relying on illustrative graphics to summarize the results.

The results section is followed by the discussion section, where you craft your main arguments by building on the results you have presented earlier.

The "discussion section" is where you rely on the power of narrative to enable numbers to communicate your thesis to your readers. You refer the reader to the research question and the knowledge gaps you identified earlier. You highlight how your findings provide the ultimate missing piece to the puzzle.

Of course, not all analytics return a smoking gun. At times, more frequently than I would like to acknowledge, the results provide only a partial answer to the question and that, too, with a long list of caveats.

In the "conclusion" section, you generalize your specific findings and take on a rather marketing approach to promote your findings so that the reader does not remain stuck in the caveats that you have voluntarily outlined earlier. You might also identify future possible developments in research and applications that could result from your research.

What remains is housekeeping, including a list of references, the acknowledgment section (acknowledging the support of those who have enabled your work is always good), and "appendices", if needed.
Have You Done Your Job as a Writer?

As a data scientist, you are expected to do thorough analysis with the appropriate data, deploying the appropriate tools. As a writer, you are responsible for communicating your findings to the readers. Transport Policy, a leading research publication in transportation planning, offers a checklist for authors interested in publishing with the journal. The checklist is a series of questions authors are expected to consider before submitting their manuscripts to the journal. I believe the checklist is useful for budding data scientists and, therefore, I have reproduced it verbatim for their benefit.

    Have you told readers, at the outset, what they might gain by reading your paper?

    Have you made the aim of your work clear?

    Have you explained the significance of your contribution?

    Have you set your work in the appropriate context by giving sufficient background (including a complete set of relevant references) to your work?

    Have you addressed the question of practicality and usefulness?

    Have you identified future developments that might result from your work?

    Have you structured your paper in a clear and logical fashion?


### Basic PowerPoint

### FINAL PRESENTATION

For your final assignment you will create a presentation based on the analysis of your data conducted in previous modules. Your presentation will develop into a story of your analysis that should be compelling and easy to understand. A PowerPoint template has been provided to get you started however you are free to add additional slides, charts and tables.

0. Download the Microsoft PowerPoint presentation template from the link below: 

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DA0321EN-SkillsNetwork/labs/module%206/Lab%20-%20Getting%20Started%20with%20PowerPoint%20for%20the%20Web/Final-capstone-story-template.pptx

Note: If you do not have a desktop version then follow the instructions from the previous lab to get access to PowerPoint online.

1. Complete the slides with relevant details (You are free to add additional slides, charts, tables).

2. Add any additional unused charts or tables to the appendix that you think are relevant to your analysis.

3. Convert your final presentation into .pdf format.

4. As part of your grade for the final assignment, you will be asked to upload your presentation for peer review.

5. You will also need to review the final presentation for at least one other peer and grade them before your final grade will be available.


The main grading criteria will be:

    Have you uploaded the template presentation in pdf format?

    Have you filled up the Title slide with relevant information?

    Have you filled up the Executive Summary slide?

    Have you filled up the Methodology slide?

    Have you used the correct visualizations?

    Have you included the screenshots of the dashboard you created in Module 5?

    Have you titled the charts correctly?

    Have you filled up the findings & implications?

    Have you used the appendix slide to include data collected from other sources?

    Have you used your creativity to improve the presentation beyond the template?

    Have you given any value additions?

    Have you displayed any innovative ideas?

You will not be judged on:

    Your English language, including spelling or grammatical mistakes.

    The content of any text or image(s) or where a link is hyperlinked to.
