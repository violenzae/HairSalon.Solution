# _Hair Salon_

#### _A web application that allows the user to dynamically enter and view vendors and vendor-specific orders._

#### By _**Rachel Schieferstein**_

## Description

_This is a SQL database/C#-based web application that has an HTML UI. The user comes to a splash page which prompts them to add a stylist, or view existing sylists and clients. Then they can choose to add clients to individual stylists, and further drill down into individual client and stylist details. It uses ASP.NET MVC, shared layouts, static files, branching logic, classes, methods, HTML helpers and auto-implemented properties._

## Specifications:

| Specification | Example Input | Example Output |
| ------------- |:-------------:| -------------------:|
|User can can choose to add a new stylist with a description| "Tasha", "description"| "Tasha" is added to the stylist database with entered "description"|
|User can view all stylists|Selects "view all"|All stylists in the stylist table of the database are printed to the page|
|User can view all clients of each stylist|Clicks "Tasha"|All clients that work with "Tasha" are displayed.|
|User can edit added stylists|"Tasha" --> "Tasha B"|"Tasha" is updated to "Tasha B" in the stylist table|
|User can delete stylists|User selects "Delete" from options on "Tasha B" Details page|"Tasha B" is removed from the stylists table.|
|User can add a new client and specify which stylist it belongs to, as well as other client details.|"Barbara", "Tasha B"|"Barbara" is added to the clients table, with the id of the specified stylist in a stylist column.|
|User can view all clients|Selects "view all"|User can see all clients listed in the clients table.|
|User can edit clients|"Barbara" --> "Barb"|"Barbara" is updated to "Barb" in the restaraunt table.|
|User can delete clients|User selects "Delete"|The row with "Barb" is removed from the clients table.|

## Setup/Installation Requirements


* _Clone or download from Github Repository._
* _Install .NET Core SDK_
* _Install MySQL and start and login to a local server._
* _Recreate the database and tables by entering the following commands:_
  * CREATE DATABASE `rachel_schieferstein`;
  * CREATE TABLE `clients` (`ClientId` bigint unsigned NOT NULL AUTO_INCREMENT,
  `Name` varchar(255) DEFAULT NULL,`StylistId` int DEFAULT '0',`Service` varchar(255) DEFAULT NULL, PRIMARY KEY (`ClientId`), UNIQUE KEY `ClientId` (`ClientId`));
  *  CREATE TABLE `stylists` (`StylistId` bigint unsigned NOT NULL AUTO_INCREMENT,`Name` varchar(255) DEFAULT NULL,`Description` varchar(255) DEFAULT NULL, PRIMARY KEY (`StylistId`), UNIQUE KEY `StylistId` (`StylistId`));

* _Navigate the terminal in the "HairSalon" directory in the project, and run "dotnet restore"_
* _In the terminal in the "HairSalon" directory, type "dotnet run" and open http://localhost:5000/ in a web browser._

## Known Bugs

N/A

## Support and contact details

_If there are any questions, please contact me at violenza@gmail.com._

## Technologies Used

_This project was created using MySQL Workbench, Entity Framework 2.2.6, C#, ASP.NET MVC, Razor 2.2.0, CSS, Bootstrap 4.4.1 and HTML._

### License

*This software is licensed under the MIT license.*

Copyright (c) 2020 **_Rachel Schieferstein_**