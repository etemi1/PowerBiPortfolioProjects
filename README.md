# PowerBiPortfolioProjects
Data Modelling, Data Analysis, Data Visualization are the Skills displayed in this Project
This is a Sales vs Budget Analysis.
 In this Project i performed a data Analysis for the purpose of presenting my Insights to my Stakeholders.
 
 
 ABOUT DATASET:
 This Dataset contains 4 data with different structures Namely SalesData, Budget, Product and photos respectively
Here is a screenshot of what the data contains
 
 
 
![Screenshot (35)](https://user-images.githubusercontent.com/41531796/197608535-7e2f68c8-ed5c-412f-bb51-8261586fbfd3.png)
![Screenshot (36)](https://user-images.githubusercontent.com/41531796/197608937-74670d3b-bd14-4a3d-9c3d-beec94fe6760.png)
![Screenshot (37)](https://user-images.githubusercontent.com/41531796/197609061-feea297c-9ffd-4a73-8d0e-53c70cf9f958.png)
![Screenshot (38)](https://user-images.githubusercontent.com/41531796/197609138-19f511af-a5eb-4bc6-9b62-172d275fdb46.png)

PROCESS:
Data EXploration: I Explored the data with Excel, to get an idea of the kind of entities in the data i am working with the columns, the measures and dimension

DATA CLEANING & NORMILIZATION: I imported all 4 files into Power BI and started data Cleaning Process. Power Bi seperated the Photos into two tables so making all the tables 5.
The data Cleaning Process Started with duplicating the Sales table so that i can model the data at the same time. My reason for duplicating the Data is so ican  have a dimension table called Salesperson. I removed every other ccolumn not relating to Sales Person, removed duplicates and performed an Inner join so that i can merge the extra table that contained EACH SalesPerson Image in URL Form with Sales Table. Sales Person column add forms like SP 105 so to make it consistent with the Sales Table, i splitted the column so i can have 105 standing Alone.
  By now i have two clean tables
  Next i duplicated the Table again to form a  Dates Table, after that i went to the Product Table and removed the ProductID Name since  there was already a column with that information. I Performed another Inner join with the Photos Table to extract Product URL. I changed data types to necessary data types, added a custom Column for Profit 

