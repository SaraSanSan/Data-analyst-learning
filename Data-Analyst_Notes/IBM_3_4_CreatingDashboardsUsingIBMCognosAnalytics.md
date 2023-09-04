
# CREATING VISUALIZATIONS AND DASHBOARDS WITH COGNOS ANALYTICS #

# CREATING DASHBOARDS USING IBM COGNOS ANALYTICS #

### SUMMARY ###

In this lesson you have learned:

- How to register and navigate around Cognos Analytics.

- How to use Cognos Analytics to create a simple dashboard.

- About the value of Cognos Analytics and its advanced capabilities, such as creating calculations and leveraging navigation paths.


## Cognos Analytics: INTRODUCTION & HOW TO SIGN UP ##

> In this video, we're going to cover a couple of things. The first is a quick overview of what Cognos Analytics is and we're going to show you how to sign up for the trial. 

- Cognos Analytics is a multifaceted tool allowing you perform both mode 1 and mode 2 type of analysis, all in one product. 

    · It contains a number of different tools, such as the ability to model your data, explore your data, create compelling, advanced analytics visualizations like our key driver analysis, displaying natural language generated based off of your data, and create reports which are specific and tailored to your individual users, either through filters or through the ability to create bursts. 

    · We also have the ability to create fantastic dashboards, which will be the main focus of this particular course. 
    

- Now to sign up for the trial, we're going to go to the IBM.BIZ/TRY_COGNOS. If you already have an account, you can login here and you'll simply have to fill out part of this form. If you don't, then we'll go ahead fill out this form quickly, and the key one to take note of is to select a Data Center which is close to you in your particular geography. Now the system is being spun up for us and we can go ahead and actually launch this directly from this workflow. Now that you're in, you can go ahead and either manage your subscription through this button, or alternatively, you can always re-access the system through this URL. 

> In the next video, we'll take you through a little bit around how to navigate and use Cognos and its dashboard capabilities.



## NAVIGATING IN Cognos Analytics ##

> In this particular video we'll cover of how we can upload spreadsheets, channel navigation, in Cognos Analytics, how to start a new dashboard, using dashboard templates as well as navigating within the Cognos Analytics Dashboard environment.

- There are two main navigation areas for Cognos Analytics. Along the left-hand side, as well as along the top. These will change and update based on the area you're in the product. 

- Now for today, while Cognos can connect to a number of databases, we're going to start with simply uploading an Excel file. We can do this in one of two ways. We come to the New, select Upload files, and navigate to find the file in question. Alternatively, what we can do is we can drag and drop the file onto our main landing page here and have it take us directly into the experience that we're looking to do in our case here, dashboard. 

- Now you'll notice that this says that uploaded content will land in my content, which is up there on the left-hand navigation. Whether you do it from here or through the plus and upload, it'll still land in the same place. Once in my content, it can be taken, moved around into a shared area within team content. 

- As the file uploads here, you'll notice that we see something that says "Analyzing." This allows us to interrogate the data, get an understanding of what's in the data in order to be able to help make some better assumptions and decisions for you as we look to build out content. 

- The first thing we'll do is we go to build a dashboard, is to select a template. You'll see a number here, and based on what you're trying to achieve, how many visualizations and what types, you may want to select something specific. In this case, I'll choose one that has four and one larger space.

- Once we're in the dashboard, we'll notice that the pane with our uploaded file column headers is displayed. There's a few other things that we want to highlight here in terms of navigation to help you with the experience here in Cognos Analytics. Our second pin down here allows you to pin different visualizations for reuse in other dashboards across the system. We'll come back to our assistant in a future video. But this allows you to ask questions in natural language and have the system tell you a little bit about your data as well as provide some visualizations. Next system here is our view of all the different visualizations we support in the dashboard, as well as the ability to upload your own custom visualization should we not have one that meets your needs. The final one here, is our additional widgets, whether that's text, images, video, hyperlinks or any of the shapes that are viewed here. 

> In the next video, we'll dive a little bit deeper into how specifically to create dashboards.



## CREATING A SIMPLE DASHBOARD in Cognos  ##

> In this video, we'll cover off creating simple dashboards and Cognos analytics. We'll cover a variety of different methods for creating a visualization. Whether it's through our automatic generation, manually populating slots, or using our system. We will also cover off how you can filter within a Cognos Analytics dashboard. 

- As I mentioned, as the data was uploaded, we took a look at the data and tried to understand what types of data were included, and that's denoted by the icon in front of each of these elements. Now in the case of order ID, we actually want to switch this up and change it. Change the properties from a measure to an identifier. 

- With that done, let's go ahead and start to create some visualizations. It's simply grab for my tree and drag it onto the canvas. 
    · Now in this case, if I drop on top of the box, what it'll do is it'll fill the space available as denoted by the template.
    · Next, look at the number of orders that we've by counting the number of order IDs that we have. Now in this case, it determined the best visualization for an identifier to be a list. We can go ahead and take a look at what other recommended visualizations. In this case, there aren't any, but we know we want to turn this into a summary so we can just go and manually select it. 
    · Next up, let's look at the quantity ordered and we'll finally finished with the average sale. In this case, I'll drag Sales onto the canvas, but what I'll do is I'll change our summarization from sum to average. 
    · So just like that, I now have a few KPIs to be able to monitor and track. 

- The other way we can search create visualizations is by selecting the specific visualization we want and dragging it onto the canvas. 
    · In this case, I'm interested in looking at our sales across the world based on countries. In this case, I can find country. Alternatively, if I have a lot of data, I can simply start to type at the top. I'll see country comes to the surface. As we said, we wanted to take a look at sales.
    · In this case, we look specifically at country, but as you can see, we can go further down in terms of latitude and longitude. Now with this, I can manually drag and drop to make this as big or as small as I want, and you'll see that we show percentages of how much real estate it's actually taking it out. Of course, each of our visualizations has a number of properties. We won't get into those in too much detail. But if there's something that you're looking to do, take a look at the properties and it's likely there. 
    
- The final way that will show creating visualizations is through our assistant. Now in this case, I may have an idea of what I want to look at or I may not. 
    · If I don't, I can simply ask it to suggest questions. This will offer up some insight that I may not have been thinking about. In this case, we'll keep it simple. We'll just look at which product line has the top sales. With a click, I'm now presented with the visualization as well as alternatives based on that particular visualization. If I'm happy with a view, I can simply drag and drop this onto my canvas, and it now becomes a visualization alongside the others, I can continue to resize this.

- Now, all of our dashboard design are meant to be interactive. 
    · In this case, if I were interested in seeing the rest of my dashboard through the specific lines of classic cars, I can click on "Classic Cars" and you'll see that all my visualizations are now updating specifically with the filter of classic cars. Now this is one way that I can do it, and I can do it multiple clicks. Or alternatively, I can take that particular field and drop it in. If I were perhaps interested in a particular status, I could drag this into the all tabs or if I just want to be specific to this tab in here. Now with this, I'll be able to choose one or many. In this case, maybe we want to take a look at how much we have in the on-hold status. With that, we'll see again, all of these have been updated to reflect to simply the on-hold. It looks like from a world-wide view, we only have holds in a couple of countries which is positive. 
    
> In the next video, we'll delve deeper into a few of the more advanced capabilities of the dashboard.



## ADVANCED CAPABILITIES in Cognos Analytics Dashboards  ##

> In this video we're going to cover a few of the more advanced capabilities in Cognos Analytics Dashboards. Cover how to create calculations. How to leverage navigation paths. How to do excludes from visualizations, as well as how to set top bottom on a visualization.

- Much like Excel our dashboard can create CALCULATIONS. We list out a number of different options here that you can take a look at or alternatively you can simply start typing and will offer up suggestions. 

    · In this case, we're interested in looking at our MSRP, minus the price that we sell each unit for, to give us a margin calculation.
    · Now this calculation is treated exactly the same as any of our other fields that we have in here. So in this case let's select our margin, and we'll look at product line and bring that in. 
    

- In this case, we can see the trains is not doing very well. It's actually a negative margin for us. Now we may want to drill into this a little bit more. So we can create what we call NAVIGATION PATHS. 
    · In this case I can choose any field from my data to be able to drill up and down on. In this case we want to start with product line, and probably want to see customers and ultimately if there are specific orders.

- Now I can right-click on trains. I can start to drill down. In this case, I can see that we have a few offenders who are in the negatives when we look at this particular field. So if we go ahead and look at something like many gifts. Again, we can drill down a little bit further to see that while they have one which is positive the other ones are in the negatives. Let's take another look at something a little bit different. So we look at sales, by status, and by product line.

- Now in this case were still filtered on trains so we may want to go back. Navigate up. In this case, we're still filtered on just trains. So let's unclick that to get back to our initial starting point. In this case, we can see that are shipped is really dramatically having an impact on this. So we can go ahead and we can choose to exclude our shipped items. Now we get a much better view of everything else that's going on for the other statuses. 

- Another thing that we could do is if we have a large number of data points in this case, perhaps customer sales, customer name and sales, we may want to FILTER DOWN on only our most important ones. In this case I can come to sales right-click and I can ask it to show us a top X number. In this case, by default we have 10. Now we can see these are our top 10 customers. 


- And one last one just for fun. We can actually create INFOGRAPHICS on the fly. In this case if I've got sales, I can take any one of my shapes here, perhaps a piggy bank, drop it on top and just like that we've now created an infographic.
