
# CREATING VISUALIZATIONS AND DASHBOARDS WITH SPREADSHEETS #

# CREATING DASHBOARDS USING SPREADSHEETS #

### SUMMARY ###

In this lesson you have learned:

- The role of dashboarding and why it is an important skill as a data analyst.

- How to setup and configure a simple dashboard in Excel.

- The importance of dashboards in telling a data-driven story.


## INTRODUCTION TO DASHBOARDING ##

> In this video we will have a brief introduction to dashboards, including what they are, what they consist of, why they can be a useful component in a data analyst’s toolkit, and an essential skill in a data analyst’s skillset. 

- The term ‘dashboard’ comes from the automotive industry where car designers have put the most important gauges and other display information, such as engine oil temperature, current speed, current RPM, amount of fuel left, and so on, in a handy graphical display that is easy for the driver to view and understand. Originally these displays were analog, but many are now digital and use varying forms of visualization, including digital meters and mini graphs. You can take that same idea and apply it to a dashboard in a data analysis application; designers of these types of dashboard want to put key business information in one place, in the form of graphical displays, to make it easier for the viewer to understand them.

- Dashboards can take this a step further by also  allowing the user to interact with the dashboard and modify exactly what information they see by using tools supplied on the dashboard. Users of a dashboard therefore not only get a consolidated visualization of their business   data and key performance indicators (or KPIs), but also get a controllable self-service business intelligence (BI) interface through the use of filters, which enable them to control precisely what information they see. 

- Dashboards are typically created in a data analysis application by using multiple pivot tables and charts, visualizations such as Map Charts and Sparklines, and filtering tools such as Slicers and Timelines. These pivot tables and charts could be created from a single data  source or from multiple data sources. 

- When you use dashboards in your data analysis application, you get the following benefits: They offer insights into your key data; They can alert you to patterns and trends in your data; They provide an interactive experience for the user, allowing them to filter what data they see; They are updated dynamically as the source data changes; They provide a centralized and consolidated view of business data.

- A dashboard can be a very useful tool in areas of the business such as fiscal forecasting and reporting, project management, executive reporting, human resources, customer service, helpdesk issue tracking, healthcare monitoring, call center analytics, social media marketing, and many more. 

- For a budding data analyst, dashboards can be a vital skill to add their arsenal, as the majority of employers see the dashboarding skill as a ‘must have’ rather than a ‘nice to have’.

- If you can show that you have the skills to create accomplished and spectacular, interactive, yet easy to view and use dashboards,  whether in a spreadsheet application such as Microsoft Excel or Google Sheets or using a more advanced data analysis and visualization   application such as Bokeh or Dash in Python, RStudio’s Shiny, Tableau, or IBM Cognos Analytics, then that will greatly help in your future career as a data analyst.

> In this video, we had a brief introduction to dashboards, including what they are, what they consist of, why they can be a useful component in a data analyst’s toolkit, and an essential skill in a data analyst’s skillset. In the next videos, we will learn how to create a simple dashboard using a spreadsheet application.



## INTERVIEW: Using Dashboards to Present Data Results ##

> In the first part of this video, we will listen to several data professionals discuss how dashboards can help when presenting data results.

- Can you tell us how dashboards can help you when presenting data results? 

- One thing I particularly love with data are dashboards. They take the fluff out and they show you the most important things that you want to see, often in real time, and you can make them as pretty as you want. I've seen some dashboards that are frankly an eyesore because of trying to cramp so much data into one dashboard. It's important to be specific and be succinct in what it is that you're looking for so that you can avoid those things. A lot of the times the dashboards are great for executives or business owners on the go who are maybe looking at dashboards from a mobile device and they don't really have the space or the capacity on a mobile device to look at so much data. 

- Dashboards can really be highly effective in the short amount of time as long as you understand the deliverables and what it is that you're stakeholder wants to see and what's important to them for purposes of making decisions. The reason why presenting the information in a way that is palatable to your audience is important is because you want to make sure that people are getting value out of what you're doing. A lot of times I think that's why data analysts in general get a bad reputation because people still think we're just number crunchers. I think the bigger problem is we haven't done as good of a job as we could to really explain the numbers and so that's where PowerPoint presentations with graphs, we love graphs, key performance indicators maybe that prick out the information in a different way and highlight what's most important, that will help. Also just making sure that you're reading the room. If you were in a meeting and everybody's eyes are glazed over because you're talking numbers, maybe you need to ask them, "What information are you looking for? What is most important to you?" So that when you go back and you create your next dashboard or create your next report, you can highlight things that are important to your audience because we always need to be reading the room. 

- We need to make sure that we are showing our value, helping people to understand, educating them so that they can bring up their knowledge-base and so that starts to help the fear dissipate. The fear of the numbers starts to go away if we would just show them what the numbers actually mean. We can do that not just by throwing numbers at them so they'll get overwhelmed, but by helping them to see it graphically and with dashboards and KPIs, and other ways just to bring it to them and make it real to them. Dashboards in a spreadsheet is an indicator for action. Just like on your car dashboard, if you see a low fuel light, that means you need to put gas in your car. A dashboard in a spreadsheet should be just that simple. It should tell the person what they need to focus on immediately or any indication that things need to change because it's either going up in the wrong direction or it's going down. But don't put information that's nice to know on a dashboard. It's on a need to know basis especially if you want to get action. 


> In the second part of this video, we will listen to a data professional discuss how Cognos Analytics can help you create outstanding visualization dashboards for presenting data results. 

- Can you tell us how you use Cognos Analytics to create visualization dashboards for presenting data results? 

- IBM Cognos Analytics can really help you create a better visualization and dashboards in a number of different ways. Starting off we have our templates, allowing you to quickly select from a template and simply drag and drop your visualizations into the slides to help you create something that's visually compelling effectively and easily. We also have what we call our visualization recommender. If you grab a couple fields, drag them onto the canvas, we'll recommend a visualization. If you don't like the one we recommend right off the bat, then you do have the ability to go in and start to select some different visualizations from our recommendations. On top of this, we also have started to infuse AI into the offering. In this, you can start to have the system actually generate an entire dashboard for you. You can have a conversation with our assistant, ask it questions, and once you're focused in on the particular area that you're interested in, simply say, "Generate dashboard." At that point you'll get a beautiful dashboard created, laid out nicely that you can search and use as your starting point for further discussions and help you really understand the data that's in your system. A couple of things that we want to highlight, one is the advanced analytic capabilities. Whether this is through our visualizations like our key driver analysis or through our AI infused forecasting. The last thing would be the ability to share your visualizations and your dashboards in just a few clicks. Whether that's sharing it in the system through a link, whether it's pushing it to email or even pushing it into a Slack channel where you can start to have a discussion there.



## CREATING A SIMPLE DASHBOARD USING EXCEL ##


> Now that we've learned about the basics of dashboards and why they are an essential tool for a data analyst, in this video we'll look at how to set up and configure a relatively simple dashboard in Excel, which will help us to tell a story about our data. 

- Before creating our first dashboard we would have first collected and organized the data then verified that the data in our worksheet was clean error-free and did not contain any blank rows or columns and then we would have formatted it as a table. 

- Next, we would have created some pivot tables to help us analyze our data and we would have performed some sorting and filtering on the data in our pivot tables to highlight the key aspects of our data analysis. 

- Lastly, we would have created various data visualizations such as charts, maps, and slicers to help us tell a story about our data findings. 

    · In this example, Car Sales Workbook we've already gone through those processes of collecting, cleaning, analyzing, and visualizing our data and we are now at the point where we can combine that data analysis and those visualizations in a digital dashboard that will help us present our key data findings to stakeholders. 
    
    · The first thing we need to do is create a new worksheet to host our dashboard and give it a name, then drag it to the end of the tabs list in the workbook. As we've already created several visualizations we can use those to populate our dashboard.

    · So, if we look at some of the other worksheet tabs these contain various visualizations which we've been working on throughout this course. We can just use some of them by copying a few charts and other visualizations from there to our dashboard. We'll copy this pie chart from this worksheet and paste it to our dashboard then we'll grab a copy of this 3D column chart and paste that too.

    · We'll also copy the 3D area chart from the other pivot chart sheet to our dashboard.

    · We'll grab the tree map chart and copy that to our dashboard too.

    · Let's copy the scatter plot chart too.

    · We'll also copy the histogram and copy that to our dashboard worksheet, and let's take a copy of the map chart visualization too.

    · Let's also copy the Sparkline's visualization to our new dashboard worksheet.

    · Lastly, let's go back to the line pie bar worksheet and select both the line chart and the bar charts and copy them both to the dashboard worksheet. 
    
    · Okay, so now we have a lot of different visualizations on our dashboard. We can make things look a little better by resizing some of the visualization objects and moving them around a bit. So we've now resized some of the visualizations and move things around, and then we could zoom out to see all the visualizations on screen. But if we remember what we heard from some of the subject matter experts during the expert viewpoints video, sometimes less is more and one or two of the experts mentioned that if we provide and display too much information, the key points can sometimes get lost. So, we should create a copy of this dashboard on another worksheet and then thin down the amount of visualizations and maybe make them more focused to highlight one or two of the more important views we want to convey.

    · To do that, we'll first make a copy of the dashboard worksheet and move it to the end of the worksheets tabs. On the copy dashboard 2 worksheet we'll now delete a few superfluous charts.

    · Let's first remove the tree map because that is giving us almost the same information as the pie chart. Then we can remove the 3D column chart because that has essentially the same data as the 3D area chart. And let's also lose the scatter plot histogram and the Sparklines because they aren't really key to our message.

    · Let's copy the slicer from the line pie bar worksheet to our dashboard to give us some interactivity.

    · Now let's zoom back out and do some arranging and resizing to these visualizations to make the dashboard look a little sharper. So, now we've rearranged and resized the visualizations to make the dashboard look a little leaner and tidier. 
    
    · We should also make some style and color changes to give our dashboard a more consistent look and feel. We'll apply the same style to all the chart elements. So, we'll apply a dark gray style and monochromatic green colors to the 3D area chart, and the line chart, and the pie chart, and the bar chart and the map chart. And we can recolor the slicer too to fit in with our color scheme.

    · Now things look a lot better and more professional and the last thing we should do is remove some of the Excel interface elements and other bits of unnecessary screen clutter to give us a nice clean looking dashboard. We can remove screen clutters such as grid lines, the formula bar, and headings. And we can collapse the ribbon too, and that should do it. 
    
    · Now when we either present this dashboard or email it to a key stakeholder it includes some interactivity via the slicer and also via the filterable pivot chart. If we use the slicer to select several Ford car models, all three charts that are related to that data, get updated at the same time.

    · We can modify filters in the 3D area chart to display only Ford cars instead of Chevrolets.

    · And if we switch to the pivot chart 1 worksheet we can see that the original data has also been updated with this new filter.

    · And when we make changes to the original source data, such as increasing the value of unit sales of cars in Australia, the map chart visualization in this worksheet updates and the Australia turns dark blue. But also, the map chart visualization in the dashboard gets updated too. So we can see that Australia is now dark green on this map chart. All of this shows how live and interactive the data in our dashboard is. Creating a clean, focused, and interactive dashboard can be a major asset when trying to tell a story about data. 
    

> In this video we learned how to set up and configure a relatively simple dashboard in excel, which will help us to tell a story about our data. In the next video we will get an introduction to IBM Cognos Analytics Data Analysis and Visualization Business Intelligence Platform.
