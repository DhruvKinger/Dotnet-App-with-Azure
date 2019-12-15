# Dotnet-App-with-Azure SQL Database
This describes the detailed step by step procedure to connect Dotnet application with Azure SQL Database.Steps that need to be followed are as follows:
+	Create a SQL Server
+	Deploy the database
+	Connect with Dotnet Application
# PREREQUISITES: You must use Microsoft SQL Server Management Studio 18.0 (or later)
* Task 1st  : Create a SQL Server 
You need to have a SQL Server that will host your database. If you already have a SQL Server than you can skip this step else follow the steps below :
+	Navigate to the [Azure Portal](https://azure.microsoft.com/en-gb/).

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(10).png)

+	Using Search Box present at the top in the centre, search sql server.
+	Select Sql Server.


![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/1st.png)

#                                               Or

+ You can click on ‘create a resource’ and from their you can choose sql server.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(11).png)

*	Then you have to choose SQL Databases.
*	Next you need to fill in the following information.
*  a.	Server name – the name of your new SQL Server.
*  b.	Server admin login –  your server admin user name.
*  c.	Password – Use a password that u can remember
*  d.	Subscription – select an existing Microsoft Azure subscription you are having access to.
*  e.	Resource group – select an existing resource group or create a new one. For more information on resource groups you can refer to the Microsoft documentation on  [Resource groups](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview#resource-groups).
*  f.	Location – pick any location of your choice.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(12).png)

+	Click Create.

# Note :You need to remember you server Admin login as well as password until you have not saved them in your Microsoft Sql Server Studio.

+ Once deployment is complete. You can move to list of sql Servers.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(19).png)

* Task 2nd  : Deploy your database.
* Once your SQL Server has been created, you can proceed with deploying your database to Azure SQL Database. You can do this task by going in your SSMS(SQL Server Management Studio). Follow these Steps mentioned below :
# Note : SSMS must be 18.0 or later.
+	Open your Sql Server Management Studio and Locate your database present in the local machine.
+	Right Click on the database. Select Tasks -> Deploy Database to Microsoft Azure SQL Database.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(13).png)

+	On the next Screen, click Next.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/2nd.png)

+	The next screen asks you to fill in your Azure SQL server connection details. Now here comes the role of your remembering those passwords.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(14).png)

*	When Done Click Connect.

*	If you haven’t already added a firewall rule in your Azure SQL Server  that enables communication from your local machine’s IP or range of IPs, the next screen enables you to configure one without leaving the SSMS interface. The wizard asks you to sign in with your Azure account and add a firewall rule for your IP address.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/3rd.png)

*	Next Screen will ask your database parameters. I have chosen Basic Plan and size 1 GB. You can chose of your choice.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(15).png)

+	Click Next.


![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(16).png)

+	Once Deployment is complete. Click on Close. You can find the database in Azure Portal .

+	Click on the connection strings for your database in Azure Sql Server . Copy ADO.NET connection string.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(18).png)

Task 3rd : Connection with the Application.
+	Open Visual Studio in your PC and find your Project.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(20).png)

+ Open Web Config File in your Project.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/Screenshot%20(22).png)

*	Comment out this connection string and paste connection string copied from Azure Sql Database.

![](https://github.com/DhruvKinger/Dotnet-App-with-Azure-/blob/master/Blog%20Folder/4th.png)

*	Once you have pasted that connection string. Your connection with the Azure Database is established now. Now your Dotnet Application needs Internet for any querying.

*	So, finally we have completed all our tasks. You can change the timeout for your database of your choice.










