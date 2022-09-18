# Azure-Projects- Multi-stage pipeline using YAML file

This project will focus on how to use CI/CD Pipelines as Code with YAML for Azure Pipelines. 

This will cover, creating the application infrastructure on the cloud with Azure SQL, Azure Service Plan, Azure SQL Server and configure firewall rule to allow Azure Web App to communicate with Azure SQL Server.

Also, how to create a new YAML pipeline from Azure DevOps pipelines template for ASP.NET which include tasks in YAML that restore all the NuGet packages, build the ASP.NET application and running unit test, create Web.Zip of the app and store that on Azure Artifacts then pick this package and deploy it to the Web App and SQL Server on Azure.

Using YAML (Yet Another Markup Language). This allows us to access pipeline features as but with a markup file that can be managed like any other source control file. YAML build definitions can be added to a project by simply adding their source file to the root of the repository. Azure DevOps also provides default templates for popular project types, as well as a YAML designer to simplify the process of defining build and release tasks.
