![image](https://github.com/user-attachments/assets/bd971b19-6630-49ba-9ac4-9037c9dee0c0)# TodosApi - Provides enpoints to manage ToDo Tasks from UI

Tech Stack:
  - Dotnet 8
  - EntityFramewok core - Code First Approach
  - c#
  - Sql SERVER EXPRESS
  - XUnit

* The Application is cors enabled
* Unit Tests Added for Task Controller and Services.

Api Project Structure:

* Controllers:
- Account Controller - Authentication/Authorisation/JWT Token (used asp.net Identity)
- TaskList Controller - Manage Todo Tasks (Get/Add/Update/Delete)

* MiddleWare:
- Global error handling Middleware

* Repository : To Manage Data and tasklists (Pattern :Repository Pattern for object relational Mapping to Sql)

* Services: To Manage TaskLists

* Mappers - Auto Mapper to map dtos and data models

****Pre Requistes:****

* Dot Framework 8,
* EntityFramework Core,
* Visual STUDIO 2022,
* Sql Server Express

==================================**How to Run Api**========================================
 The WebAPi will run on port: 5115

 To run Api:

**Change connectionstring accordingly in AppSettings.json**
 example:
   "ConnectionStrings": {
    "Default": "Server=ServerName;Database=todo;user id=***;PWD=***;Trusted_Connection=True;MultipleActiveResultSets=true;TrustServerCertificate=true"
  },

**Build the Application**
* Build Application 
* After build application Succeded.

**Run below in Tools Nuget Package Manager Console

- Add-Migration "init"

- database-update

  Asp.net Identty tables aand ToDo table wil be created in Sql Server

  Two roles [Admin,User] will be added as part of migration

Api will be up and running on Port
http://localhost:5115/swagger/index.html
 

Unit Tests Can be run from Explorer:

![image](https://github.com/user-attachments/assets/e460b186-b1ae-4bc5-afaa-bd7871391b37)

