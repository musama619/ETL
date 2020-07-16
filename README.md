# ETL

# Extract Transform Load

![download](https://user-images.githubusercontent.com/34093998/87681277-f0abc700-c797-11ea-92b9-8a12ed74b344.png)

* # Softwares 

![0](https://user-images.githubusercontent.com/34093998/87681669-55ffb800-c798-11ea-9123-c56b16b0cb31.png)
![download (1)](https://user-images.githubusercontent.com/34093998/87681207-d70a7f80-c797-11ea-8f85-e84bba4e1210.jpg)

* Microsoft® SQL Server® 2014 Express (https://www.microsoft.com/en-pk/download/details.aspx?id=42299)
* SSDT-BI (https://www.microsoft.com/en-pk/download/details.aspx?id=42313)

# Steps to Remember

1. Open SSDT for Visual Studio 2013, Create New Project and Select "Integration Service Project". Click OK
2. In the SSIS "Control Flow" Drag and Drop "Data Flow Task", rename it(if you want) then double click on it.
3. In the Data FLow Task Drag and Drop "Flat File Source" 
4. Double Click on it. A new window will appear. Click New->Browse Select your .csv file and open (Text Qualifier = ") and then Click OK
5. Next from "Other Destinations" Drag and Drop "OLE DB Destination" in the Data Flow Task.
6. Click on Flat File Source and Connect Blue line with OLE DB Destination.
7. Double Click OLE DB Destination, Click New->New and Write your Server Name which is connected in Microsoft® SQL Server® 2014 Express. Click OK.
8. Select the name of availabe tables in your database or create new. On left corner click Mapping then click OK
9. Now Click "Start". The table has been created. Refresh Database or Table in Microsoft® SQL Server® 2014 Express you will see the newly created table.
10. Right click and "See top 1000 rows" to view table data.
11. Come back to SSI and select Control Flow. Right Click and select disable option.

##### Note: If we dont disable then upon starting again by mistake will make the data duplicate in table.
