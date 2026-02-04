# London Housing Data Analysis

This project analyzes London housing data, including average prices, number of houses sold, and crimes per area over time. The analysis follows a series of tasks as outlined below.

---

## Tasks / Questions

**Q1. Convert the Datatype of 'Date' column to Date-Time format.**  
- Convert the `date` column from object/string to `datetime64[ns]` for time series analysis.

**Q2. Add a new column 'year' in the dataframe, which contains years only.**  
- Extract the year from the `date` column and add it as a new column.  

**Q2.B Add a new column 'month' as 2nd column in the dataframe, which contains month only.**  
- Extract the month from the `date` column and insert it as the 2nd column in the dataframe.

**Q3. Remove the columns 'year' and 'month' from the dataframe.**  
- Drop the `year` and `month` columns to revert the dataframe to its original structure.

**Q4. Show all the records where 'No. of Crimes' is 0. And, how many such records are there?**  
- Filter the dataframe for records where `no_of_crimes == 0` and count them.

**Q5. What is the maximum & minimum 'average_price' per year in England?**  
- Group the dataframe by year for `area == 'England'` and calculate the max and min average house prices.

**Q6. What is the Maximum & Minimum No. of Crimes recorded per area?**  
- Group the dataframe by `area` and find the maximum and minimum values in `no_of_crimes`.

**Q7. Show the total count of records of each area, where average price is less than 100,000.**  
- Filter the dataframe where `average_price < 100000`, then count the number of records per area.

---

## Notes
- All date-time operations are done using pandas `to_datetime` and `.dt` accessor.  
- Columns `year` and `month` are created dynamically from the `date` column.  
- Aggregations like min, max, and counts are performed using `groupby` and aggregation functions.  
- This analysis helps to observe trends in housing prices and crime rates in London areas over time.
