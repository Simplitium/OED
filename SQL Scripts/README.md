# SQL Scripts

There are 3 script files to create OED DB and populate respective reference tables. They all should be run in the order they are numbered. The size of the database created is around 4GB.

## 1. Create DB and tables:
•	If you want a different name for the DB, replace all instances of OED_v1.0.1 with the name that you want (there are quite a few instances in the entire script).

•	Update your file paths – for DB and log - to where your DBs are normally saved (for log file as well!):

*C:\Program Files\Microsoft SQL Server\MSSQL12.MSSQLSERVER\MSSQL\DATA\OED_v1.0.mdf*

## 2. Populate reference tables:
•	Update database name, if you renamed OED_v1.0.1 in the first script.
 
 
## 3. Populate xPerilCodeLookup:
•	Update database name, if you renamed OED_v1.0.1 in the first script.

•	This script is slow (could be around 15 min). Parts of the code that show what’s in the tables themselves are commented out – but in case you need to look at the tables you can run those too.
