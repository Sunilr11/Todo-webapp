---
topic: ASP.NET and SQL Database sample for Azure App Service
languages:
  - aspx-csharp
products:
  - Azure App Service
  - Azure Web Apps
  - Azure SQL DataBases
---

# ASP.NET and SQL Database sample for Azure App Service

This is a sample application that you can use to follow along with the tutorial at 
[Create an ASP.NET app in Azure with SQL Database](https://docs.microsoft.com/en-us/azure/app-service-web/app-service-web-tutorial-dotnet-sqldatabase/). 

# Azure SQl DataBase

For connecting SQL DB with App service, the connection string need to be created in Azur eApp service 

Eg:  Data Source=tcp:<Servername>,1433;Initial Catalog=<databasename>;User Id=<username>@<servername>;Password=<password>
     Data Source=tcp:server.database.windows.net,1433;Initial Catalog=dbname;User Id=demouser@server;Password=******

Note: While creation of connection string in app service "Name" should be given correctly. In our case
      name = MyDbConnection
      value = Data Source=tcp:<Servername>,1433;Initial Catalog=<databasename>;User Id=<username>@<servername>;Password=<password>
      type = SQLAzure
  
  You can find the name in repo under **Models/mydatabasecontext.cs**
## License

See [LICENSE](LICENSE).

## Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
  
