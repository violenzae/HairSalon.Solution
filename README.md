# _Hair Salon_

#### _A web application that allows the user to dynamically enter and view vendors and vendor-specific orders._

#### By _**Rachel Schieferstein**_

## Description

_This is a SQL database/C#-based web application that has an HTML UI. The user comes to a splash page which prompts them to add a stylist, or view existing sylists and clients. Then they can choose to add clients to individual stylists, and further drill down into individual client and stylist details. It uses ASP.NET MVC, shared layouts, static files, branching logic, classes, methods, HTML helpers and auto-implemented properties._

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