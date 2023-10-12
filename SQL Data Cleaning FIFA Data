# Data-Cleaning-in-SQL-FIFA-Data #

/*Cleaning Data in Mysql Queries*/

Use portfolio_project;
SELECT * FROM fifa_data;

--------------------------------------------------
/* show the top 10 rows of the match_details table */

select * 
from fifa_data 
limit 10;

---------------------------------------------------------
/* Remove Duplicated rows */
/* First check which rows are duplicated using ID column */

select ID, count(ID) as cnt 
from Fifa_data group by ID Having cnt>1;

select DISTINCT *
from Fifa_Data;

/* creating a table with non duplicated rows */
CREATE TABLE non_dup_data 
SELECT Distinct * 
FROM Fifa_Data;

select * from non_dup_data limit 10;

select * from non_dup_data;

/* delete the original table */
drop table Fifa_Data;

-------------------------------------------------------------------------------
/* Alter the non duplicated table name to the original table name*/

Alter Table Non_Dup_Data Rename Fifa_Data;


Select * from Fifa_data;

Select ID, Count(ID) as cnt
from Fifa_Data
Group by ID
Having cnt > 1

-----------------------------------------------------------------------------
/* showing the Scorer name and how many goals they have scored 
then store that data into another table called scoring */

select scorer, count(ID) as goals
from Fifa_data
group by Scorer;

CREATE TABLE IF NOT EXISTS scoring 
select Scorer, count(*) as Goals 
from Fifa_data group by Scorer;

------------------------------------------------------------------------
/* Check scoring table. Show the scorer with the most goals first*/
select * 
from scoring
order by Goals DESC;


select Scorer, count(*) as Goals 
from Fifa_Data group by Scorer;






