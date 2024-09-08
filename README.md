
# Dashboard of Ice Cover In the Lakes of The United States

### Dashboard Link :  https://app.powerbi.com/groups/3805ea30-4d66-47db-9f49-46c08a9f4684/reports/50286549-96d2-46f8-89d7-404ca6f5144d/efea39c7e4b6945c0d05?experience=power-bi

This Dashboard helps us to gain Insights of Ice cover in the lakes 
during the Years 1973-2020 




## Problem Statement / Insights :

1. Analysis of Year wise  Average ice  cover in Lakes of the United States

![Avg Value ](https://github.com/user-attachments/assets/1adfd5c9-d179-4dfd-92df-f408dddb4cd5)


2. Finding the Maximum and Minimum of ice cover of each lake 
 
![min max](https://github.com/user-attachments/assets/22594a5e-340b-439a-9276-eff6837985c7)


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a   file.

- Step 2 : Open the power query editor & in the view tab under the Data preview section, and check the "column distribution", "column quality" & "column profile" options.

- Step 3 : Also since by default, the profile will be opened only for 1000 rows you need to select "column profiling based on entire dataset".

- Step 4 : It was observed that in none of the columns errors & empty values were present in the dataset 

This means our data set is clean


- Step 5 : All the values are in Text format, we converted all the data   into number format 

- Step  6: I took the same dataset again I Unpivoted The table so that  it  is easy to observe dataset year-wise in table format  all the lake's dataset 

- Step 7 : 
Dax Queries  :
- I created  max  value ice cover  of each lake given in the dataset :  
  5 lakes are given 
  1. Erie
  2. Huron
  3. Michigan
  4. Ontario
  5. Superior
  6. other Lakes 

- calculated max of  ice cover by each lake in the United States
 

for creating a new column following the DAX expression was written;
       
        MaxErie = Max('US Lakes'[Erie]) 

        MaxHuron = Max('US Lakes'[Huron]) 

        MaxMichigan = Max('US Lakes'[Michigan])

        MaxOntario = Max('US Lakes'[Ontario])

        MaxSuperior = MAX('US Lakes'[Superior])

       
- Step 8  : Create a Dashboard  using Constant colors and a neat presentation.
