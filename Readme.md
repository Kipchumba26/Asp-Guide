# ASP MVC GUIDE
( *quick guide on how to work with ASP.NET MVC* )

## Table of Contents

- [Introduction](#introduction)
- [Installation](#install)
- [Create](#Create Project)
- [Routing](#Routing)
- [Routes/Actions](#Add Route/Action)
- [View](#Add View)
- [Model](#Add Model)




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


## Routing
Routing is the mapping of urls to application handlers and views that resolve what should be done when a user visits a url.
In ASP.NET, routing is based in controllers and actions. Controllers live on the controllers folder. Actions are methods in controllers that return views, json, html, xml or any other accepted formats.
Actions must have a corresponsing view in ASP.NET MVC Razor Pages. If you have a controller named TestController and inside it a function called Check, the app will have a route domain/Test/Check. 'domain'
in this case can be http://localhost:$PORT or https://localhost:$PORT or a custom domain if the application has been deployed.

In this current application, we have a controller called HomeController and inside it a function called About. This means there is a route domain/Home/About.
This is how ASP.NET MVC does its routing.


## Routes/Actions
An action acts as part of a url, in the case of Home/About, About is an action. It is
also a function that can have code that acts on data and returns a view. This view can
be JSON, html, xml or any accepted format.
Here is a simple example

```
        public ActionResult About()
        {
            return View();
        }
```

ActionResult here indicates the return type JSON, html, xml. 

```
return View();
```
Above line indicates that an html view is being returned. ASP searches for a view with
same name as the action/function in a folder named as the controller that contains the
action.

If About is in HomeController.cs, the html file is searched in Home folder and has to
be named About.cshtml or About.html or About.aspx.