
# Competitor Sales Analysis in Power BI

This project follows the guildance from Datacamp courses to develop a complete Power BI report starting from the data integration from multiple sources, data transformation, modeling, and then visualization.





## Preparing the Data
In this part, I start exploring and integrating the dataset into Power BI and understand the challenges faced with the uncleaned data. 

Then, using Power Query Editor operations, II will clean and mash up the data to use it for reporting.

Case study scenario:
- Analyze manufacture’s sales internally
- Comparing sales against other competitors
- Comparing product performance against other competitors

1. Load all the required data.
2. Clean and explore by removing unnecessary columns. Replace null values by fill-down function. 
3. Split the values by "Columns from example" and ensure the data types are correctly formatted. 

![price](https://user-images.githubusercontent.com/105278875/205037129-07031276-e38d-4cc5-95e0-10b117cb2064.PNG)

4. Remove uncessary rows. Transpose the table to ensure correct structure.
5. Append the queries: combine both Sales tables and create a single table that analyzes sales for all countries. 
6. Have a quick exploratory analysis by suing (View - Column Profile - Column Statistics and Value Distribution)

![Capture](https://user-images.githubusercontent.com/105278875/205038573-c0ddc014-7629-4e80-9a07-a0579fce2e08.PNG) 

7. Review the last 3 years by Filter Rows.
8. Create Clustered Column Charts to determine which manufactures generate most value. 

![Revenue by manufacture](https://user-images.githubusercontent.com/105278875/205039032-da27dc2f-b099-4f87-8ae6-baf60ef93742.PNG)

9. Setting up relationship between tables1
10. Create new calculate by DAX 

Date = CALENDAR(DATE(2017,1,1), DATE(2021,12,31))

## Discovering business insights
1. Using top N list to identify major competitors. 
2. Choosing the Stacked column chart to see how the values of each manufacturer contribute to the totals. 
3. Select an appropriate visual that displays Revenue over time (Clustered Column chart). Add slicers and ensure Data labels, Target labels, and Callout value are all enabled. 
4. Add some more dimensions and create a hierarchy of Category, Segment, Product to analyze in-deep about Revenue (using Matrix visual)
5. To show the sales growth and the rate at which a product can increase the revenue from sales, using DAX calculations. Select the maxtrix visual and drag PY Sales and %Growth in values section. 
6. Apply conditional formatting rule 
- 0-40%: Red
- 41-60%: Yellow
- More than 60%: Light Blue

![part 2](https://user-images.githubusercontent.com/105278875/205265203-40a3417d-3ba1-457e-b7aa-955079e08d62.PNG)


## Creating a Data-driven story
Sintec’s marketing department has asked to keep the report design and UI in line with the company’s standard guidelines and provide with a color theme. In this project, I use Sunset theme to make the report look cleaner and more professional. 

1. Change the manufacturer slicer from drop down to list. Add the actual logos of the manufacturer into slicer. 
2. Upload customized theme. Add title and change font. 
3. Using bookmarks and Spotlights feature will highlight specific visuals and present them in a story. 
4. Apply advanced AI-based visualizations to make analyze more robust.
5. Add more functionality of drillthrough to help end users focus on a specific entity. 
6. Complete the analysis and reporting using Power BI's Analyze feature to explain the increase or decrease seen on charts. 

![f1](https://user-images.githubusercontent.com/105278875/205268368-a37ab22e-cb77-427f-8a1c-772dcfddc9ba.PNG)

![f2](https://user-images.githubusercontent.com/105278875/205268387-315432e7-08d0-4e89-be78-03189ad80bc7.PNG)


## Conclusion
1. Sintec has total market share of 38.22% in the USA. 
2. The highest growth of 18.8% in 2021 compared to last year. 
3. Artisans is generating revenue with over 50% of the market share in Germany. 
4. Sintec has 21.15% of the total market share across the globe. 