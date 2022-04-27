# ASP MVC GUIDE
( *quick guide on how to work with ASP.NET MVC* )

## Table of Contents

- [Introduction](#introduction)
- [Installation](#install)
- [Create Project](#Create Project)
- [Routing](#Routing)
- [Add a Route/Action](#Add a Route/Action)
- [Add a View](#Add a View)
- [Add a Model](#Add a Model)




## Introduction
ASP.NET MVC is an improvement of Windows Forms. It simplifies how websites are build. MVC here are the key terms as Visual Basic and 
C# are still the languages used to develop these applications. 
M stands for Model, simply put an entity class, eg User, V stands for View, the user interface and C stands for Controller, this is where logic
to get data from the database and display a View is put.


## Installation
ASP.NET MVC requires a few softwares to be installed for development to happen:

### Visual Studio
This is the main IDE used for ASP. It also installs all windows dependencies that are required to develop ASP applications. It comes with an additional
installer that can be used later on to install any required dependecies when needed.

### MsSQL and MsSQL Studio
Since most applicaations require a database, several organizations  choose MsSQL, Microsofts SQL Database as their database.
This is partly because it's easier to work with it when using Microsofts technologies. 
Install the database itself 'MsSQL' and then the ''MsSQL Studio' database explorer from where developers can run queries on tables, import or export data, see inserted data among other things.




## Create Project
To create a project, open Visual Studio, 
1. select Create a new project.
2. in the Create a new project dialog, select ASP.NET Core Web App (Model-View-Controller) > Next.
3. in the Configure your new project dialog, enter project name > Next
4. in the Additional information dialog, select .NET 6.0 (Long-term support) > Create

