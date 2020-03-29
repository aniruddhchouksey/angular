# angular
this has all the code for angular course that i am following

understanding angular versoning
    AagularJS(Angular 1)
    |(complete rewrite)
    Angular 2
    |
    Angular 4
    |
    Angular 9

how an angular app gets started
    - when we go to localhost:4200 the index.html file is served by the server.
    - the angular app serves the index.html file to the browser and all the js files are inserted as a scritpt in the html files.
    - then the main.ts file is executed which inturn initializes the appModule and then find all the import statements.
    - then after importing all the things the app is ready to serve the files to the user. these html files are dynamically generated.

Components
 - components are the building block of angular application 
 - each component is an html tag which define a component and all its buisness login
 - component has its html, js, css.
 - these component are created only when used.
 - component are just plane TS class which have a @Component decorator which is imported from @angular/core.
 - component decorator holds an object which defines the basic properties of the component like 
 - selector - this is a string which defines a html tag which will be used for the component. this needs to be unique.
    - if we want we can make the selector to be an attribute which can be used with a div by putting the selcector like '[app-server]'. these are called custom attributes.
    - or we can make it a class selector by specifying the selector as '.app-server' and add it using a class.
 - template - this is a string which containes the html code for the component, in case we dont want to have the html in ts file itself we can use templateUrl.
 - templateUrl - this takes the relative path to the component html file for rendering.
 - styleUrls - this is an array of relative paths to the CSS files which are going to be used in this componenet.
 - styles - this is an array of strings which can be used to define inline styles for the application.

Modules:
 - angular uses component to build web pages and uses module to bundle pieces to make features.
 - it's also just a ts class which has a @NgModule decorator which holds a object with several properties like declarations, imports, providers, bootstrap.
 - all the component needs to be registered in the module 'declaration' propery before using them in the application.

Databinding:
 - communication between TS code and HTML template.
 - string interpolation
    - we use the {{  }} to provide any ts expression which can be evaluated to a string. we can't have block expression like if else, but we can have ternary statement.