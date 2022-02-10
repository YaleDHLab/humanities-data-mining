# Introduction to Data Visualization with Tableau Public

## Overview
[Tableau Public](https://public.tableau.com/en-us/s/) is a free visualization suite for creating interactive data visualizations online. With a single click, you can move between different chart types and see which works better for the data and questions at hand.   

While Tableau runs locally, it saves publicly—meaning your data becomes public. For data with privacy restrictions, you should use Tableau Desktop, which runs on and saves to your local machine. [Students](https://www.tableau.com/academic/students?utm_campaign_id=2019176&utm_campaign=Prospecting-PROD-ALL-ALL-ALL-ALL&utm_medium=Paid+Search&utm_source=Google+Search&utm_language=EN&utm_country=USCA&kw=tableau%20for%20students&adgroup=CTX-Brand-Student-E&adused=RSA&matchtype=e&placement=&gclid=EAIaIQobChMI4uyd9faW6gIVkYbACh2MZgwNEAAYASAAEgIG6PD_BwE&gclsrc=aw.ds) and [educators](https://www.tableau.com/academic/teaching?utm_campaign_id=2019176&utm_campaign=Prospecting-CORE-ALL-ALL-ALL-ALL&utm_medium=Paid+Search&utm_source=Google+Search&utm_language=EN&utm_country=USCA&kw=%2Btableau%20for%20%2Bteachers&adgroup=CTX-Brand-Teaching-B&adused=ETA&matchtype=b&placement=&gclid=EAIaIQobChMIp5Spi_eW6gIVycDACh2PAQkjEAAYASAAEgLwKvD_BwE&gclsrc=aw.ds) can sign up for free yearly licenses to Tableau Desktop.

## Example Project: Internet Users by Country
To practice working in Tableau Public, download this [dataset of internet users per 100 people](https://raw.githubusercontent.com/YaleDHLab/humanities-data-mining/master/workshop-materials/tableau-workshop/data/internet-users.csv) by selecting "File" and "Save Page As..." Make sure that the file format saves as a comma separated value (CSV) file. This dataset was published by Tableau Public in 2018, but was originally published on [Knoema](https://knoema.com/WBINU2018/internet-users-per-100-people). The spreadsheet includes three variables or columns ("Country," "Internet users per 100 people," "Year") and 1,764 records or rows.

As a sample research scenario, let's imagine that someone just handed us this data. To get a better feel for its quality and what questions we might ask of it, we can create a few exploratory visualizations in Tableau Public. [A completed copy](https://public.tableau.com/app/profile/peter.leonard6457/viz/YData2022InternetUsers/dashboard#1) of the Tableau workbook we're about to create can be found on Tableau Public.

### Set Up
1. [Download, install, and then open Tableau Public](https://public.tableau.com/en-us/s/).
2. Under "Connect" in the left-hand column, click on "Text file" and select the `internet-users.csv` file. This will load a preview of the dataset, which lets us see how Tableau is interpreting our data.
3. Review Tableau's interpretation of our data. The symbol at the top of the header represents what data type it thinks each column contains:
- Abc = string (text) data,
- Globe = geospatial data, 
- Calendar = temporal data, 
- Hashtag = numeric data, 
- T|F = Boolean (true or false) data. 
 
For our dataset, we need to change the "Year" column from a numeric value to a date. To do so, click on the hash symbol above "Year" and select "Date." You should notice that all of our years now also have a month and day prefixed to them; by default, Tableau treats dates as month-day-year, so it adds a generic 1/1/ to the beginning of our year.

4. To begin working with our data, click on the grey "Sheet 1" rectangle toward the bottom left-hand corner of the application. This will create our first Tableau worksheet, a blank space for generating visualizations.

![Button for New Worksheet](https://github.com/YaleDHLab/humanities-data-mining/blob/master/workshop-materials/tableau-workshop/image/tableauNewWorksheet.png)

#### Interface Interactions 
Double-clicking or dragging any dimension or measure over to the "Columns" and "Rows" sections near the middle-top of the sheet will give you the opportunity to examine the data more closely. You can use the back arrow at the top left to undo actions.  
- "Pages," "Filters," and "Marks" are where you will drag dimensions and measures in order to filter the data.
- The "Show Me" button on the top right can be clicked on and off. When clicked on, it shows you different visualizations you can toggle between, along with what kinds of data you need in order to generate them. Toggle "Show Me" off for now since it takes up screen real estate and will hide our filter settings (once we create a filter).

### Starting Questions
With this dataset, we can see how internet adoption has changed by country over time. Before we start looking closely at the numbers, what are your preliminary guesses as to which 5 countries had the most internet users per 100 people in 1990? What about in 2015? Let's see if the data matches our expectations!

### Bar Chart: Internet Adoption
1. Drag "Country" to "Rows."
2. Drag "Internet users per 100 people" (not the measure Tableau generated, which is just counting the number of rows in our spreadsheet) to "Columns."
3. Sort data from most to least by clicking the icon with the three stacked rectangles and downward arrow (it's located in our toolbar at the top of the sheet). 
4. Question: if our dataset is internet users per 100 people, then why does Iceland show 708.8 users?
<details><summary>Answer</summary>
<p>
Tableau is summing all values that correspond with an "Iceland" row, regardless of whether they record is for a different date. To see internet users per 100 people, we need to add a year filter.
</p>
</details>
5. Create the year filter by dragging "Year" to the "Filters" card. 
- Select "Years" in the resulting pop-up box.
- Click the "All" box.
- Click "Ok." It will look like nothing happened.
- To set the filter, click on the dropdown by "YEAR(Year)," and select "Show Filter." This will show the filter settings in the right-hand column (you may have to click off "Show Me" to see it).
- In the right-hand column, click the dropdown by "YEAR(Year)," and select "Single Value (list)" to filter one year at a time.</br>
6. We can now answer our starting questions. Which 5 countries had the most internet users per 100 people in 1990? Which 5 countries had the most in 2015?
<details><summary>Answer</summary>
<p>
In 1990, the United States, Norway, Switzerland, Australia, and Sweden had the most internet users per 100 people. By 2015, the top 5 changed to: Iceland, Luxembourg, Andorra, Norway, and Liechtenstein. Only Norway appears in the top 5 twice!
</p>
</details>
7. If we want to focus only the top countries in terms of internet adoption, we can add a country filter by dragging "Country" to the "Filters" card. This time, select the countries of interest. If we'd like to compare greatest number of users in 1990 to 2015, we should select: the United States, Norway, Switzerland, Australia, Sweden, Iceland, Luxembourg, Andorra, and Liechtenstein. You can choose whichever countries are of interest to you!
8. Give a title to the chart by double clicking on the current "Sheet 1" title and inserting "Internet Users per 100 People." You can also change the styling, if you want a different typeface or font.Click "Apply" to see what the title will look like. When you're finished, click "Ok."
9. Change the "Sheet 1" name in the lower left-hand corner by double clicking on it and renaming it "bar chart."

### Line Graph: Change over Time
1. Start a new sheet by clicking the icon next to our current sheet.
2. Double click on "Year" (this should add it to the "Columns" section)
3. Double click on "Internet users" (this should add it to the "Rows" section)
4. Drag "Country" to the "Color" mark - note the warning cautioning against the use of color for more than 20 records. To see what happens, click "Add all members." While the resulting line graph shows an overall increase in the number of users, it's difficult to track individual changes and differentiate colors. Click the back arrow in the top-left corner to undo.
5. Drag "Country" to the "Color" mark again, but this time, click "Filter and then add." Choose countries of interest (you might choose the same countries from the bar chart or new ones you want to highlight). To ensure colors can be easily distinguished, don't choose over 10 countries.
6. Change line colors by clicking on the dropdown next to "Country" in the right-hand column. Select a palette from the dropdown, or double click on the color next to an individual country's name to change it. When you have colors you like, click "Assign Palette" to see what they look like on the graph. Then click "Ok." 
7. Give the graph the title: "Internet Users over Time."
8. Change the "y axis" label by double clicking on it and then typing "Year" in the "Axis Titles" field.
9. Rename the sheet to "line graph."

### Map: Internet Users by Country
1. Start a new sheet.
2. Double-click on the "Country" pill, which will automatically generate a map.
3. Click to turn on "Show Me" and select the second map, which we will use to generate a choropleth map.
4. Notice that not all countries are filled in on the map. Click on "3 unknown" in the lower right-hand corner of the map to give Tableau a mapping between country names as they appear in our dataset, and country names that Tableau knows. 
- Dem. People's Rep. Korea to North Korea,
- Dem. Rep. Congo to Democratic Republic of Congo,
- Korea to South Korea.
5. Drag "Internet users" over the "Color" mark, which will shade each country according to the number of internet users—by default, Tableau will again aggregate this count.
6. To filter by year while also adding animation to the map, drag "Year" to "Pages" (instead of "Filter").
7. Let's give the map a title. Delete sheet name (but keep "Page Name") and add: "Internet Users per 100 People in:" before the "Page Name", which will automatically fill in the title with whatever year is selected.
8. Rename the sheet to "map."

### Data Dashboard: Combine Visualizations Together
1. Start a data dashboard by clicking on the icon next to the sheet icon.
2. Adjust the size of the dashboard by clicking on the dropdown under "Size" in the left-hand column. This enables you to re-size for the device(s) your designing for. To have the dashboard take up the size of the screen you're using, click the size dropdown and then click the dropdown by "Range" and select "Automatic."
3. Double click on the sheet names in the left-hand column to add them to the dashboard (I would start with the map). You can also drag and drop. Practice re-arranging them on the dashboard.
4. To make the dashboard even more dynamic and informative, let's add a component that links out to the Wikipedia page for whichever country a user selects.
- Drag a "Web Page" object onto the dashboard and click "Ok" without adding a URL. 
- On the dropdown box for the web page object, click "Add URL Action."
- In the name field, type: "Go to Wikipedia page for" and then click the triangle button at the end of the line and select "Country."
- For "Run action on," choose "Hover."
- For URL, add: "https://en.wikipedia.org/wiki/" and then click on the triangle button and select "Country."
- Click "Test Link" to see if it's working.
- Click "Ok" and "Ok" again to add the action.
- Hover on any data point in the dashboard, and the Wikipedia page should automatically update to reflect the country that's selected. ![Dashboard View](https://github.com/YaleDHLab/humanities-data-mining/blob/master/workshop-materials/tableau-workshop/image/tableauDashboard.png)

### Save Your Work
To save your Tableau workbook, you have to create a free Tableau account. When you click save, you will be prompted to log in and save your workbook to Tableau's server, where it will be visible on Tableau Public. Users can interact with your workbook on Tableau Public, or they could download, add to, or otherwise edit it.

## Bonus

### Animated Bar Chart: Internet Adoption Revisited
1. Let's learn a bit more about animations in Tableau so that we can create more dynamic graphs. Start creating a new sheet.
2. In our bar chart, we highlighted the countries with the highest number of internet users. If we want to dynamically watching the country order change over time, we have to set up a rank field. To do so, right-click near the bottom of the "Tables" column and select: "Create Calculated Field."
3. For the title of the Calculate Field, type "Rank". The syntax for a rank calculation is: ```RANK_UNIQUE(sum([Internet users per 100 people]))``` If you Google Tableau and the kind of task you're looking to perform, you'll find tutorials with many different types of calculations you can create. Once you've added the calculation for rank, click "Ok."
4. Drag the new "Rank" measure to "Rows."
5. Add "Country" to the "Detail" mark.
6. Go back to the "Rank" pill in "Rows" and change the data from "Continuous" to "Discrete."
7. Drag "Internet users" to "Columns."
8. Go back to the "Rank" pill in "Rows" and choose "Computer Using" -> "Country."
9. Drag "Year" into the "Pages" section, which will activate the animation.
10. To add country instead of ranking as the label: go to "Rank" and deselect "Show Header." Next, drag "Country" over the "Label" mark. To stylize the label, click on the "Label" mark - from here, you can change the "Label Appearance" (type, font) and "Alignment" (where the label appears).
11. To add a color scheme, drag "Internet Users" over the "Color" mark. You can more precisely adjust the colors by clicking on the dropdown beside "Internet Users" in the right-hand column.
12. Don't forget to add a title!

## Next Steps, Cautions, & Additional Tips
* To learn about joining multiple datasets, creating data stories, running calculations, and managing a Tableau server, watch Tableau's free [online training videos](https://www.tableau.com/learn/training/20201).
* Word of caution: Tableau frequently has updates available, but they're not always backwards compatible. For that reason, you might not want to update to the newest version while you're in the middle of a project.
* For additional practice and open datasets, check out [#MakeoverMonday](https://www.makeovermonday.co.uk/). Every week, Tableau shares a dataset and starter visualization, and challenges participants to remake it. You can find the results and share your own remakes on [Twitter](https://twitter.com/hashtag/makeovermonday?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Ehashtag). Better yet, if you see a makeover visualization you like, try downloading the workbook from Tableau Public to see how it was made!
