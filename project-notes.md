202211031018

Status: #power-bi #business-intelligence #bi-workflow
Tags: [[Power-BI]]


---
# Power BI Project


---
## Exec Summary
AW Client cares about:
- *Total Orders* by *Product Categoy*
- *Total Orders* Info by *Product Subcategory* (Revenue and Profit)
- product level performance
	- in terms of *order*
	- how frequently some products are being *returned*
	- the *revenue*
- add a slicer that **filters all data on page** based on *date interval* 
	- also add a *report wide filter* to not include year 2015 in report (even the slicer reduces to 2016-2017) because in 2015 they only sold bikes (other business)
- add Cards, Multi-row, *KPIs* (Quantitative, Numerical values) with:
	- *KPI* (*Key Performance Indicators*) show the **Value**, the **Trend** and the **Target**
		- *Total Revenue* card, with *Start of Month* **trend** and the **target** is *Prev Month Revenue* (hit the last month's revenue)
		- same for *Total Orders*
		- same for *Total Returns* (**reverse the target, low is hood**)
- text Cards (Text Values) with:
	- top product by *Total Orders*
	- top product by *Total Profit*
- Map (Simple, Filled Map, ARCGis Map):
	- *Total Sales* by *Continent* (simple map)
- [[Report View#Filter Interactions]] 
	- disable the interaction between *Timeline* and *KPIs*
	- interaction between *Category* and *Subcategory* tables (matrices) is set to highlight
- [Optional]:Create Roles ([[Report View#Managing & Viewing as Roles]]) to provide different *Territories* manager with their specific info and nothing else


---
## Product Detail
- *Total Profit* by *Start of Week* line chart
- *Total Returns* by *Start of Week* line area chart
- Simple Forecast on the *Total Profit* line with 95% confidence for 6 weeks
- Gauges with *Total Orders*, *Total Revenues* against *Targets* 
- Gauge with *Total Returns* against *Previous Month Returns*
- Card with *Product Name* and [[Report View#Drillthrough Filters]] with *Product Name*  
	- on the ***Exec Summary*** page, any product name has now the ability to drillthrough to the ***Product Detail*** page to see trends and performance for **individual products**
- A simple button to create [[Report View#Bookmarks]] from the ***Exec Summary*** to the ***Product Detail***
- Forecasting and Scenario Testing with a *What-If Parameter*
	- implement an *adjusted price* (+/- 100%) that works on *average retail price* to forecast changes in *Total Profit*


---
## Customer Detail (HW)

**1)** Add a new report page named "**Customer Detail**"

-   Add a matrix visual to show **Total Orders** and **Total Revenue** by customer full name for the top 100 customers by revenue
    
-   Sort the matrix by **Total Revenue** (_descending_) to show the top revenue-generating customers
	   
-   Add conditional formatting to show data bars on the **Total Orders** column and a background color scale on the **Total Revenue** column, and customize the style however you'd like 
    

**2)** Add a _Donut Chart_ to show **Total Orders** by **Gender** (_on the Legend_)

-   Title the chart "_Orders by Gender_", and adjust formatting to match the gauge charts on the **Customer Detail** tab 
    
-   Copy the chart and paste two more versions: one to visualize orders by **IncomeLevel**, and a second to visualize orders by **Occupation** (_chart titles_)
    
-   Update the report interactions so that _each_ donut chart (as well as the matrix) **_filters_** the other two donuts, instead of highlighting
    

**3)** Add a _Line & Clustered Column_ chart to show **Total Orders** (_as columns_) and **Total Revenue** (_as a line_), with **Start of Month** on the shared X-axis

-   Update the chart title to "_Orders & Revenue by Month_", and format the chart style however you choose
 
-   Select the matrix, and update the report interaction mode to **_filter_** the combo chart (_vs. highlighting_)
    
        
**4)** Add a _Treemap_ visual to show **Total Orders** (_values_) grouped by **Current Age** 

-   Update the chart title to "_Orders by Age_", and format the chart style however you choose
    
-   Select the matrix, and update the report interaction mode to **_filter_** the treemap (_vs. highlighting_)
    
        
**5)** Add a card to show **FullName**, and make the following updates:

-   Turn off the Category Label, update the card title to "_Top Customer_", and adjust formatting to match the donut charts
    
-   Add a Top N visual-level filter to show the #1 customer based on **Total Revenue** 
    
-   Copy and paste to create two new cards: one showing **Total Orders**, and the other showing **Total Revenue**, and update card titles to "_Customer Orders_" and "_Customer Revenue_", respectively 
 

**6)** Add a text box that says "_Executive Summary_", and insert an arrow button next to it

-   Return to the "**Exec Summary**" page, activate the bookmark tab, and add a **bookmark** named "_Exec Summary_"
    
-   Return to the "**Customer Detail**" page, and link the arrow button to the bookmark just created using the object "Action" properties 
    

---
# References

Udemy-Microsoft.Power.BI-Up.&.Running.With.Power.BI.Desktop

