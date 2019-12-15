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
a.	Server name – the name of your new SQL Server.
b.	Server admin login –  your server admin user name.
c.	Password – Use a password that u can remember
d.	Subscription – select an existing Microsoft Azure subscription you are having access to.
e.	Resource group – select an existing resource group or create a new one. For more information on resource groups you can refer to the Microsoft documentation on  Resource groups.
f.	Location – pick any location of your choice.



![](https://github.com/DhruvKinger/Rudhir-A-BDMS/blob/master/Forgithub/Screenshot%20(597).png)
