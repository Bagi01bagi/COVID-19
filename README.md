# COVID-19
We have taken a small dataset of Covid-19 just for your understanding purpose. You have to work on the original dataset which contains about 19000 rows. This data is available as a CSV file, downloaded it from Kaggle.  We will analyze this data using the MICROSOFT POWER BI
1 .STEP THIS DATESET 
2. //   Общее количество строк Total number of lines
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
![Image alt](https://github.com/{username}/{repository}/raw/{branch}/{path}/image.png)
