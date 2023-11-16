# Live360-Orlando-2023

These files were used for the demonstrations of my sessions at Live 360 in Orlando on November 16, 2023.

The file Getting Your Story Straight.pbix (https://github.com/data-inspirations/VSLive2023Vegas/blob/main/Getting%20Your%20Story%20Straight.pbix) contains examples of different styles of visualizations that I discussed in the session titled Getting Your Story Straight with Data Visualizations. No additional setup is required. All data required for the demonstration has been imported into the PBIX file and does not require a refresh to view and interact with the visualizations.

The file Sales and Marketing file (https://github.com/data-inspirations/VSLive2023Vegas/blob/main/Sales%20and%20Marketing%20Story.pbix) originally came from Microsoft and created by Obvience, but I can no longer find the original link from which I downloaded it. It provides examples of how you might structure a data story in Power BI. 

The file Customer Analysis Final.pbix (https://github.com/data-inspirations/VSLive2023Vegas/blob/main/Customer%20Analysis%20Final.pbix) contains examples of visualizations used to demonstration basic analytical concepts in Power BI as I discussed in the session titled Making the Leap from Reporting to Data Analysis. If you're not interested in the R visualizations, you can ignore the setup instructions below and Power BI will not render those pages of the report.  To view the R visualizations, you need to have a local installation of R. In my demonstration, I used R Services in Microsoft SQL Server 2019 and my environment setup is described below.

# My environment

Power BI Desktop
Download from https://www.microsoft.com/en-us/download/details.aspx?id=58494

Open the Customer Analysis Final.pbix file. You should be able to use the file without connecting to SQL Server as long as you don’t try to refresh the file or execute the R script. 

To update the file to connect to your own SQL Server instance:
Click Transform Data on the Home tab of the ribbon.
Click Data Source Settings on the Home tab of the ribbon in Power Query Editor. 
With AdventureWorksDW selected, click the Change Source button.
Change the server and database settings to match your environment if you have a SQL Server with AdventureWorks DW installed (see below).
To refresh the R visuals, you will need an installation of R on your computer and you need to configure the home directory by opening Options and Settings from the File menu, selecting Options, and then R Scripting. Configure the home directory by selecting it in the Detected R Home Directories drop-down list, or keep Other selected and manually set the path to the directory.
 
If you open the demonstration PBIX file, you will be prompted if you want to enable scripts. This is due to the presence of R visuals in the file. 
 
SQL Server 2019 with R Services 
Download from https://www.microsoft.com/en-us/download/details.aspx?id=100809
Install R Services as described here: https://docs.microsoft.com/en-us/sql/machine-learning/install/sql-machine-learning-services-windows-install?view=sql-server-ver15

SQL Server Management Studio
Download from Download SQL Server Management Studio (SSMS) - https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16&redirectedfrom=MSDN

A link to the backup file and instructions to install AdvenureWorkdsDW from a backup are on this page (https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms) in addition to “restore a database backup” instructions. Be sure to get the AdventureWorksDW20xx.bak file. I believe I used the 2014 version, but any version should be fine. The main difference would be in the date range used for sales. 









