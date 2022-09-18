# Azure-Projects- Multi-stage pipeline using YAML file

This project will focus on how to use CI/CD Pipelines as Code with YAML for Azure Pipelines. 

This will cover, creating the application infrastructure on the cloud with Azure SQL, Azure Service Plan, Azure SQL Server and configure firewall rule to allow Azure Web App to communicate with Azure SQL Server.

Also, how to create a new YAML pipeline from Azure DevOps pipelines template for ASP.NET which include tasks in YAML that restore all the NuGet packages, build the ASP.NET application and running unit test, create Web.Zip of the app and store that on Azure Artifacts then pick this package and deploy it to the Web App and SQL Server on Azure.

Using YAML (Yet Another Markup Language). This allows us to access pipeline features as but with a markup file that can be managed like any other source control file. YAML build definitions can be added to a project by simply adding their source file to the root of the repository. Azure DevOps also provides default templates for popular project types, as well as a YAML designer to simplify the process of defining build and release tasks.

*****************************************************************************

* First we need to create SQL server, Azure webapp and Resource manager. We can also create this with the help of predefined template in azure portal.

* Firewall settings to be made in Azure webapp to access the SQL server.

* In Azure devops portal, under pipelines select asp.net project(Predefined for .net application)

* Build and Test steps are already there in the readymade yaml file

* We need to add steps to create deployment

* Tasks added to create deployment
     - After the build and test stage, need to add "publish artifact" stage
     - Followed by the task add "Download build artifacts"
     - Then add "azure app service deploy" task
     
* Once the pipeline ran successful then update the webapp connection string name . Need to take the the connection string name form src/webconfig

* Now the application got deployed to azure webapp and the data will be loaded to azure sql server aswell

     

