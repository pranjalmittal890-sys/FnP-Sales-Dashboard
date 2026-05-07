# FnP-Sales-Dashboard
This is a dummy dataset
This project can be transformed using Excel or PowerBI.
I will mention steps used in PowerBI, which are the similar steps that can be followed in Excel as well.
I have also added the excel power query editor version of the same

1. Get the data by connecting the folder containing all the 3 datasets in Power BI.
2. Transform the data (Do not click on 'load' or 'combine')
3. You will see the image as shown below -
   
   <img width="959" height="355" alt="image" src="https://github.com/user-attachments/assets/507b7cd8-de00-479e-827b-0349073e6fab" />
   
5. Right click on Binary hyperlink and click on 'Add as New Query' as shown below -
   
   <img width="770" height="289" alt="image" src="https://github.com/user-attachments/assets/00f8804a-5f18-4c9d-ba7f-f899fdb2e2d9" />
   
Do this step for all 3 files and rename the files as well

7. In 'customers' table, change the data type of Contact_Number from 123 - number to ABC text (as it contains numbers and signs)
8. From 'products' table, we will use Price column and add that column in orders table using Merge queries feature and using left join to join the tables based on productID column, we only need the Price column, so we will filter out the table from the column and select only Price(INR) column.
9. Now we have order date, order time and delivery date, delivery time. Using this, we will find out the difference in delivery date and order date to calculate the number of days taken to deliver the order and add a calculated column.
10. We will also add a column to extract hours and months from order date in order to analyse the purchasing trend of the customers (at what time they purchase the products and in which months are the most purchases done)
11. At last, we will calculate the total amount by multiplying the quantity with price for each order

Now we will perform the analysis and it is shared in this repo.
