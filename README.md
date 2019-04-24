# SqlNexus-PowerBI-Templates
Power BI Templates for SQL Nexus

## Prerequisites
* Power BI Desktop (latest version - download from http://aka.ms/powerbi)
* pssdiag capture imported into a SQL Nexus DB (https://github.com/Microsoft/SqlNexus)


## Performance Reports
1.	For Performance Data (DMV queries & Perfmon counters)
2.	Open **SQL Nexus - Performance Reports.pbit** and provide the necessary parameter values
  *	**Server Name**: SQL Server containing the populated Nexus database
  *	**Database Name**: Name of Nexus database
  *	**Round To Minutes**: Used for summarizing data. 
    * For short captures, use 0 for no summarization
    * For long captures (e.g. 24 hours) a 5 minute summarization is a good starting point.
  *	**Start Date** & **End Date**: Use to limit the range of time for data loaded from the Nexus database. Useful when you have a long capture where you want to focus on a short range of time (used in combination with Round To Minutes)

## ReadTrace Reports
1.	Used when Trace/xEvent data was included in the pssdiag capture
2.	Open **SQL Nexus - ReadTrace Reports.pbit** and provide the necessary parameter values
  *	**Server Name**: SQL Server containing the populated Nexus database
  *	**Database Name**: Name of Nexus database
