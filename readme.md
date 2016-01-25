# Intro to the MEAN Stack

## Background

* Frameworks allow us to be `full-stack` developers.
* We can:
  - define the database tables
  - develop server-side code:
     * database integration
     * business logic
     * consume external APIs
     * provide a RESTful API
     * security
     * notifications / server push
  - develop client-side code:
     * HTML       - structure
     * CSS        - styling
     * JavaScript - client side events, updates, validations, integration with APIs

* Trends
  - Moving more of the application logic away from the server and into the front end.
  - Think of it as coding the back end in the front end.
  - Some of the more popular JavaScript frameworks doing this are:
      * AngularJS
      * Backbone
      * Ember

* This is not really new (though it is new to Web App Development)
  - dump terminals and `time-sharing` of mainframes
  - desktop apps
  - SaaS and cloud computing
  - Cloud data with Local computation

### Server Side Rendering vs. Client Side Rendering

* Server-side rendering: HTML page is generated and `rendered` on the server
* Client-side rendering: HTML page is served from server as a `template` and fully rendered in the browser
  - sets the stage for dynamic updates to the DOM via JavaScript
  - AJAX
  - GMail, Google Maps

### Rails

* Leans heavily on server-side rendering
* Some client-side rendering can be "sprinkled in".
* Most user actions (mouse clicks) hit the server.

### Client Side Rendering via AngularJS, etc.

* Provides rich support for client-side rendering
* Sees server as a simple RESTful API with security and persistence:
  - HTTP GET, PUT, POST, DELETE
  - JSON data

We *can* use AngularJS with Rails, but it seems a bit overkill:

* both provide MVC
* both do rendering (templates)
* both provide routing

## Motivation to use MEAN

* JavaScript throughout all layers
  - Browser
  - RESTful API (JSON)
  - Server (NodeJS)
  - Database (MongoDB uses BSON = Binary JSON)
* Better Support for Client-side Rendering
  - The Rails Asset Pipeline gets in the way
  - Rails MVC seems like overkill: default is that every RESTful endpoint has a View
* Improved performance and scalability due to *fast* asynchronous I/O
* MongoDB is easier to use than RDBMS
* JSON throughout the integration layers
* AngularJS is a rich client-side MVC SPA Framework that makes DOM manipulation easy

## Comparison of Rails and MEAN Stack


|        Feature          |          Rails                |              MEAN              |
|:-----------------------:|:-----------------------------:|:------------------------------:|
| Database                | usually RDBMS                 | MongoDB                        |
| Server Language         | Ruby                          | JavaScript via NodeJS          |
| Server Framework        | Rails                         | Express, Hapi, others          |
| ORM / DB Integration    | Active Record                 | Mongoose                       |
| Package Manager         | Bundler                       | npm                            |
| Client/Server Interface | HTML or RESTful API with JSON | RESTful API with JSON          |
| Client Language         | JavaScript                    | JavaScript                     |
| Client Presentation     | HTML / CSS                    | HTML / CSS                     |
| Rendering               | Server                        | Client                         |
| Client Updates          | Favors server rendering       | Favors Partial Updates (AJAX)  |


## Introducing the MEAN Stack

### MongoDB

* A NoSQL database
* A document database
* Stores Binary JSON (BSON)
* Easy to get up and running

### NodeJS

* A JavaScript runtime environment on the server
* Uses Google's V8 JavaScript engine
* Contains a built-in HTTP server library

### ExpressJS

* Server-side MVC for NodeJS
* Much more lightweight than Rails

### AngularJS

* A full-featured client-side MVC Framework
* Works well for SPA applications
* Makes DOM manipulation via AJAX calls easy
* Offers 2-way data-binding to simplify the HTML/JS interaction
