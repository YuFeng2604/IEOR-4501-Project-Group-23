IEOR4501 Project Group 23
================================

General Information
-------------------
Our team is made up of two group members, Andy Chen and Yu Feng. In our IEOR4501 final project, we are asked to use a dataset published by NYC to make analyses and answer the desired questions. So we create this repository to put our work, which includes the following:
1. A Jupyter notebook called `Top10.ipynb` with our analysis of top 10 incident types
2. A Jupyter notebook called `Parking.ipynb` with our analysis of parking incidents
3. README file describing the contents of our work and our group members

Dataset
-----------------------
New York City publishes a dataset consisting of calls to the 311 phone number for non-emergency services. Each call to 311 has a number of datapoints tracked and aggregated. The data we work with is from this dataset, which is stored inside a CSV file (around 1.5GB).

What Has Been Implemented
-----------------------
In the first Jupyter notebook called `Top10.ipynb`, we read the csv file and convert the `Unique Key` column to the index of our Pandas DataFrame. Secondly, we fix the zip codes after observing that "10030" is incorrectly coded as "12345". Then we analyze what the top 10 causes of calls to 311 are in our chosen ZIP code 10027, and calculate how many total incidents of each of these 10 types there have been in the year 2020. More than that, we verify the data type, index names, and values of `top10` at the last part of "Data Analysis".

In a second Jupyter notebook called `Parking.ipynb`, we want to analyze whether illegal parking incidents are a larger fraction of total 311 incidents in ZIP code 10027 than they are in general. Specifically, we compute the total number of parking incidents in ZIP 10027, which is assigned to variable `parking_cu`, and the total number of all incidents, which is assigned to variable `total_cu`. Simultaneously, assign a variable `parking_nyc`, which stands for the number of parking incidents across all ZIP codes, and a variable `total_nyc` for the total number of all incidents. Finally, our answer is in the form of a single bool called `higher_parking_proportion`, which is `False` because our ZIP 10027 contains a lower proportion of parking incidents than the global value.

Team Members of Project Group 23
--------------------------------
[Andy Chen]   
ac4952   
andy.chen@columbia.edu   
   
[Yu Feng]   
yf2604   
yf2604@columbia.edu
