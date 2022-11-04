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
 From the Data Schema and the filters we can see that the Factstable is filtering all other dimension tables except budget, this means that Budget is been filtered by sales person because each person is given a budget per monthly basis. 
   
  ![Screenshot (88)](https://user-images.githubusercontent.com/41531796/199352004-fe616737-4e6f-40da-b8d6-bb6214630d6a.png)

   
   
  # DATA ANALYSIS AND VISUALIZATION 

![IMG-7715](https://user-images.githubusercontent.com/41531796/199358223-4d7f90c8-0162-488b-b6e3-f09d3106e4d8.jpg)
![IMG-7716](https://user-images.githubusercontent.com/41531796/199358266-290bf8f1-5168-4637-972b-c11eb29ca396.jpg)
![IMG-7717](https://user-images.githubusercontent.com/41531796/199358299-288e5fcd-3710-412a-aa28-6133293eb257.jpg)
![IMG-7718](https://user-images.githubusercontent.com/41531796/199358324-b4108c5f-28bb-4edb-bedd-254016005ecc.jpg)



### DATA INSIGHTS
1. The Top 5 Sales Person where Carla Ferreira, Julio Lima, Gustavo Gomes,Felipe Goncalves, Leonardo and Cardoso
2. The best Month for this company is October, September, November and December so i would say generally 4th Quarter looks good
3. The Top Products that account gor most percentage of companies revenue is Wheat Flour, Oil, Yeasts, Flour, Liquor and Candy and the this insight is consistent all year and all quarter 
4. Food makes for the highest product category 
5. There are total of 22 Products and 2 Categories with the best Category been Food category
6. Their Best Year by Revenue Performance was in 2020 and it's surprising because in 2020 alot of companies tanked due to covid 19 that's quite interesting to know
7. The Sales Surpassed Budget every year. 
8. It's Noticed that the Best Supervisors are Diego Araujo, Diogo Carvalho, Sofia Ribeiro, Emily Rocha and Fernando Silva
9. I noticed that the best Salesperson has Best Supervisor i.e Carla Ferreira's Supervisor which is Diego Araujo they both happen to make a good team. Generally i noticed that Leonardo is also been supervised by Diego Araujo, so that the top and bottom five has good supervisors. 
