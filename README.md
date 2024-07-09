# Sale_Data_MeriSkill_internship_project
Sql Query used in cleaning the Dataset


```--the database where the dataset is stored
use [YEMIFATODU2db]

--to select Dataset from Database
select * from
[dbo].[Sale_Data]


--to check for NULL values

select *
from
  Sale_Data
WHERE column1 IS NULL
   OR Order_ID IS NULL
   OR Product  IS NULL
   OR Quantity_Ordered IS NULL
   OR Price_Each IS NULL
   OR Purchase_Address IS NULL
   OR column8 IS NULL
   OR Sales IS NULL
   OR City IS NULL
   OR HOur IS NULL;


 -- updating NULL value column

UPDATE Sale_Data
SET Quantity_Ordered = 1
WHERE Quantity_Ordered IS NULL


--Renaming the columns appropriately

EXEC sp_rename '[dbo].[Sale_Data].column1', 'Index_no', 'COLUMN';
EXEC sp_rename '[dbo].[Sale_Data].column8', 'Months', 'COLUMN';


--Dropping unwanted columns

ALTER TABLE [dbo].[Sale_Data]
DROP COLUMN Index_no;


--creating additional columns for splitting date and time only

 ALTER TABLE [dbo].[Sale_Data]
ADD Date_Only DATE,
    Time_Only VARCHAR(12);


--Populating the table with values from Order_date

UPDATE Sale_Data
SET Date_Only = CAST(Order_Date AS DATE),
    Time_Only = LEFT(CONVERT(VARCHAR, Order_Date, 121), 12);

	UPDATE Sale_Data
SET Date_Only = CAST(Order_Date AS DATE),
    Time_Only = FORMAT(Order_Date, 'HH:mm:ss');

--droping the Order_Date column from the table

ALTER TABLE Sale_Data
DROP COLUMN Order_Date;

--final check for the dataset

select * from
Sale_Data```

