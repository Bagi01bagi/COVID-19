# COVID-19
We have taken a small dataset of Covid-19 just for your understanding purpose. You have to work on the original dataset which contains about 19000 rows. This data is available as a CSV file, downloaded it from Kaggle.  We will analyze this data using the MICROSOFT POWER BI
1 .STEP THIS DATESET 
 //   Общее количество строк Total number of lines
Total_Rows = COUNTROWS('covid_19_data')

// Непустые значения для каждого столбца Non-blank values ​​for each column
Data_count = COUNT(covid_19_data[Date])
State_count = DISTINCTCOUNT(covid_19_data[State]) 
Region_count = COUNT(covid_19_data[Region])
Confirmed_count = COUNT('covid_19_data'[Confirmed])
Deaths_count = COUNT(covid_19_data[Deaths])
Recovered_count = COUNT(covid_19_data[Recovered])

// Пустые значения для каждого столбца is null
Date_Null_Count = Total_Rows - Date_Count
State_Null_Count = Total_Rows - State_Count
Region_Null_Count = Total_Rows - Region_Count
Confirmed_Null_Count = Total_Rows - Confirmed_Count
Deaths_Null_Count = Total_Rows - Deaths_Count
Recovered_Null_Count = Total_Rows - Recovered_Count

# We can see zero values ​​in the form of column diagrams with accumulation
![Image alt](https://github.com/Bagi01bagi/COVID-19/blob/main/1%20stacked.png)

2. Все остальное я делала в отчетах 
Everything else I did in the reports
* Show the number of Confirmed, Deaths and Recovered cases in each region.
* the map of Sum of Confirmed by Region and State

![Image alt](https://github.com/Bagi01bagi/COVID-19/blob/main/tha%20map.png)

3. The second page i try to show 
   *In which Region, maximum number of Confirmed cases were recorded?
   *In which region, minimum number of Deaths cases were recorded?
   *Remove all the records where Confirmed cases is less than 10
   *Show the number of Confirmed, Deaths and Recovered cases in each region. I added slicer which helps with filters
   
![Image alt](https://github.com/Bagi01bagi/COVID-19/blob/main/3%20region.png)
4. In this step i tried to use sort
   -A) Sort the entire data wrt No. of Confirmed cases in ascending order?
   -B) Sort the entire data wrt No. of Recovered cases in descending order?

![Image alt](https://github.com/Bagi01bagi/COVID-19/blob/main/sort.png)
   
5. Finally i knew How many Confirmed, Deaths & Recovered cases where reported from India till 29 april 2020
   I showed it with table and Slicer with regions 

![Image alt](https://github.com/Bagi01bagi/COVID-19/blob/main/india.png)

   
