# SQL

There are 3 script files to create OED DB and populate respective reference tables. They all should be run in the order they are numbered.

## 1. Create DB and tables:
•	If you want a different name for the DB, replace all instances of OED_v1.0 with the name that you want (there are quite a few instances in the entire script).

•	Update your file paths – for DB and log - to where your DBs are normally saved (for log file as well!):

*C:\Program Files\Microsoft SQL Server\MSSQL14.SQLEXPRESS01\MSSQL\DATA\OED_v1.0.mdf*
 
•	The scripts are created for compatibility = 120. However, if you are using 140 compatibility (newer SQL versions), then search for XXX in the script and change compatibility = 140 and uncomment part of the code. The instructions are provided in the script.

## 2. Populate reference tables:
•	Update database name, if you renamed OED_v1.0 in the first script.
 
 
## 3. Populate xPerilCodeLookup:
•	Update database name, if you renamed OED_v1.0 in the first script.

•	This script is slow (could be around 15 min). Parts of the code that show what’s in the tables themselves are commented out – but in case you need to look at the tables you can run those too.
