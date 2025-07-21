# Used-Cars
Objective: 
1. Create a Power BI dashboard showing cars data varying with various parameters eg, Engine(CC),Mileage(kmpl),location,etc.
Steps followed overview:
1. We import raw data which we first clean and modify using python
2. We edit the columns like Mileage which has values with units together eg.Engine value - 998 CC we split the the number with str.replace("CC"," ") or str.split().str.get(0) to get the number alone then change the data type from object to float by astype(float),
   we repeat it for the columns of Power and Mileage.
3. Then we find the mean value for each of these columns and replace the null values with the mean values.
4. To display the above columns with units we create new columns eg. Mileage(kmpl) and drop the old Mileage column and repeat the same for Engine and Power.
5. To Create columns regarding Brand and Model of the car data by seperating the string under Name column through str.split().str.get(0/1).
6. Find out age of cars with the new column "Car_Age" and find the difference between the present year and the Car Year given in the data.
7. Similarly fill the null values of Price column with mean of the price.
8. Repeat the same as above with the Seats column and convert the data to integer from float .
9. Make a csv of the completed and cleaned data by to_csv and download the data.
10. Open the data in Power BI and check for any irregularities.
11. Finally create a dashbord of the data to represent various changing parameters with slicers to get an overview of the cleaned data at hand for actionable insights.
