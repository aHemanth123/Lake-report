
# Dashboard of Ice Cover In the Lakes of United States

### Dashboard Link :  https://app.powerbi.com/groups/3805ea30-4d66-47db-9f49-46c08a9f4684/reports/50286549-96d2-46f8-89d7-404ca6f5144d/efea39c7e4b6945c0d05?experience=power-bi

This Dashboard helps us to gain Insights of Ice cover in the lakes 
during the Year 1973-2020 




## Problem Statement / Insights :

1. Analysis of Year wise  Average ice  cover in Lakes of United States

![Avg Value ](https://github.com/user-attachments/assets/1adfd5c9-d179-4dfd-92df-f408dddb4cd5)


2. Finding Maximum and Minimum of ice cover of each lake 
 
![min max](https://github.com/user-attachments/assets/22594a5e-340b-439a-9276-eff6837985c7)


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a   file.

- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.

- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".

- Step 4 : It was observed that in none of the columns errors & empty values were present in the dataset 

Means our data set is clean


- Step 5 : All the values are in Text format , we had converted all the data   into number format 

- Step  6: I had taken same dataset again I Unpivoted The table so that  it  is easy to observe dataset year wise in table format  all the lakes dataset 

- Step 7 : 
Dax Queries  :
- I had  created  max  of each lake given in the dataset :  
  5 lakes are given 
  1. Erie
  2. Huron
  3. Michigan
  4. Ontario
  5. Superior
  6. other Lakes 

- calculated max of  ice cover by each lake in United states
 

for creating new column following DAX expression was written;
       
        MaxErie = Max('US Lakes'[Erie]) 

        MaxHuron = Max('US Lakes'[Huron]) 

        MaxMichigan = Max('US Lakes'[Michigan])

        MaxOntario = Max('US Lakes'[Ontario])

        MaxSuperior = MAX('US Lakes'[Superior])

       
- Step 8  : Creating a Dahboard  using with Constrant colours and neat presentation.
