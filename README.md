# PowerBiPortfolioProjects
Data Modelling, Data Analysis, Data Visualization are the Skills displayed in this Project
This is a Sales vs Budget Analysis.
 In this Project i performed a data Analysis for the purpose of presenting my Insights to my Stakeholders.
 
 
# ABOUT DATASET:
 This Dataset contains 4 data with different structures Namely SalesData, Budget, Product and photos respectively
 Sale
Here is a screenshot of what the data contains
 
 
 
![Screenshot (35)](https://user-images.githubusercontent.com/41531796/197608535-7e2f68c8-ed5c-412f-bb51-8261586fbfd3.png)
![Screenshot (36)](https://user-images.githubusercontent.com/41531796/197608937-74670d3b-bd14-4a3d-9c3d-beec94fe6760.png)
![Screenshot (37)](https://user-images.githubusercontent.com/41531796/197609061-feea297c-9ffd-4a73-8d0e-53c70cf9f958.png)
![Screenshot (38)](https://user-images.githubusercontent.com/41531796/197609138-19f511af-a5eb-4bc6-9b62-172d275fdb46.png)

# PROCESS:
Data EXploration: I Explored the data with Excel, to get an idea of the kind of entities in the data i am working with the columns, the measures and dimension, After that i used the filters option in Excle to get an idea of where to start my data cleaning from

# DATA CLEANING & NORMILIZATION:
 I imported all 4 files into Power BI and started data Cleaning Process. Power Bi seperated the Photos into two tables so making all the tables 5.
The data Cleaning Process Started with renaming the Sales table as FactSales and duplicating the table so that i can model the data at the same time. My reason for duplicating the Data on FactSales Table is to create a dimension table for SalesPerson.  I removed every other column not relating to Sales Person, removed duplicates and performed an Inner join so that i can merge the extra table that contained EACH SalesPerson Image in URL Form with FactSales Table.
 Sales Person ID column had forms like 'SP 105' so to make it consistent with the FactSales Table, i splitted the column so i can have 105 standing Alone.
  By now i have two clean tables. 
  Next i duplicated the Table again to form a  Dates Table, i better way would been to use an Advance date dimesion query which would give a many to one but i tried using this method, for some reason was getting blanks, So after that i went to the Product Table and removed the ProductID Name since  there was already a column with that information. I Performed another Inner join with the Photos Table to extract Product image URL. I changed data types when necessary , added a custom Column for Profit.
 I Cleaned the Final Table, Budget. The Budget Table was where i found the real challenge, but with the help of Pivot tool in Power Bi, i was able to use filters to remove blanks and unpivoted the columns so it turned 3. 
 # DATA MODELLING:
  I tried to make all relationships Many to One with Sales Filtering Salesperson table, Date and Product and SalesPerson table was filtering Budget. 
   Here is a screen grab of the Model afterwards
   ![Screenshot (30)](https://user-images.githubusercontent.com/41531796/197616608-a1427404-1459-404c-adc9-d9b8ca0ff44e.png)
   
   
   
  # DATA ANALYSIS AND VISUALIZATION 
   ![Screenshot (33)](https://user-images.githubusercontent.com/41531796/197617348-72c8f668-73b0-4049-a6c6-20958a727e2c.png)

![Screenshot (31)](https://user-images.githubusercontent.com/41531796/197617465-f6cb6582-6861-4c55-a6c6-593e69238ecf.png)
![Screenshot (34)](https://user-images.githubusercontent.com/41531796/197617501-b84f5af4-5437-49d3-b7ad-33bdb471def6.png)
![Screenshot (32)](https://user-images.githubusercontent.com/41531796/197617535-97e67ec1-69af-49b8-882f-e4fb3c2a5fa5.png)

# QUESTIONS ASKED: 
1. What was the Monthly Sales Trend from 2019 to 2021. 
2. Did the Salesperson meet their Target?
3. Who were the TOP 5 SalesPerson?
4. What 3 products Sells the most?
5. Which Manager had the best performance?
6. Which Supervisor had the best Performance in 2020?
7. What Products are best Sold by each SalesPerson?

