xyz Technologies merges beautiful design with convenient services to electrify industries formerly dependent on fossil fuels. xyz’s turnkey power solutions deliver energy whenever and wherever it’s needed for reliable electrification beyond the electrical grid. With scalable clean power that moves to meet demand, xyz customers can tackle new applications and deploy new business models without the complexity of upgrading traditional energy infrastructure.

# Getting Started
xyz Web API build on top of [ASP.NET Core](https://docs.microsoft.com/aspnet/core/). platform. ASP.NET Core. is an open-source and cross-platform framework for building modern cloud based internet connected applications, such as web apps, IoT apps and mobile backends. ASP.NET Core. apps can run on .NET Core or on the full [.NET Framework](https://dotnet.microsoft.com/download/dotnet-framework/net472). 

### Prerequisite
  - .NET Core SDK
  - Code Editor ([Visual Studio](https://visualstudio.microsoft.com/downloads/) / [Visual Studio Code](https://code.visualstudio.com/download)) 
  
### Project Setup
1. Download .NET Core SDK from https://dotnet.microsoft.com/download 
2. Double click on installer and install in your system
3. Clone the source locally
  ```sh
 git clone https://github.com/xyzTech/web_core.git
 ```
 4. Trust the HTTPS development certificate:
```sh
dotnet dev-certs https --trust
```
5. Run the following commands for running application
```sh
cd xyzTech
dotnet run
```
### For developers
xyz Web API follow Repository pattern. It restricts us to work directly with the data in the application and creates new layers for database operations, business logic, and the application’s UI. 

Folder structure in xyz Web API. 

| Folders | Contains |
| ------ | ------ |
| xyz.API |  Which contains main root of API and controllers |
| xyz.Database |Which contains tables of database  |
| xyz.Entities |  Which contains ViewModel of API for response |
| xyz.Repository | Which contains CRUD operations of database |
| xyz.Services  | Which contains business logic of API  |
| xyz.Test | Which contains test cases of API   |

Under Unit testing xyz Web API used xUnit as the test library. 

### Plugins
xyz Web API is currently extended with the following plugins.

| Plugin | ReadMe |
| ------ | ------ |
| Dapper | https://github.com/StackExchange/Dapper |
| NSwag | https://github.com/RicoSuter/NSwag |
| AWS SDK | https://github.com/aws/aws-sdk-net/ |
| Braintree SDK | https://github.com/braintree/braintree_dotnet |

### For Deployment

1. Getting help for publish Asp.Net Core apps to run following command
```sh
dotnet publish -h
```
2. The following command specifies a Release build and the publishing directory
```sh
dotnet publish -c Release -o C:\FolderName
```

### For Run Tests
1. Run the tests in the web_core project:
```sh
dotnet test ~/web_core/xyzTest/xyzTest.csproj
```

# Documentation 
[xyz Core Web API](https://www.google.com)
