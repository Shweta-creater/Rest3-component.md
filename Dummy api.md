## REST API Testing

*REST API Testing is open-source web automation testing technique that is used for testing RESTful APIs for web applications.* 

*The purpose of rest api testing is to record the response of rest api by sending various HTTP/S requests to check if rest api is* 

*working fine or not. Rest api testing is done by GET, POST, PUT and DELETE methods.* 

*Rest stands for Representational State Transfer. It is an architectural style and an approach for communication used in the* 

*development of Web Services. REST has become a logical choice for building APIs. It enables users to connect and interact with cloud services efficiently.*

*An API or Application Programming Interface is a set of programming instructions for accessing a web-based software application.
In other words, a set of commands used by an individual program to communicate with one another directly and use each other's functions to get information.*

*For example, a Google website can have API for various functions like search, translations, calendars, etc.*

*In general API's are like below, they have server name, paths.., etc*

*http://<server name>/v1/export/Publisher/Standard_Publisher_Report?format=csv*
  
  <em>There are mainly 4 methods involve in API Testing like GET, POST, Delete, and PUT.</em> 
  
  ## GET- 
         GET method is used to extract information from the given server using a given URI. While using GET request, it should only extract data and should have no other effect on the data. 

  ## POST-
           A POST request is used to create a new entity. It can also be used to send data to the server, for example customer information, file upload, etc. using HTML forms.
  
  ##  PUT-
          Create a new entity or update an existing one.
  
  ## DELETE-
          Removes all current representations of the target resource given by a URI.
  
             
   **REST COMPONENT**  

The rest component allows to define REST endpoints (consumer) using the Rest DSL and plugin to other Camel components as the REST transport.

From Camel 2.18 onwards the rest component can also be used as a client (producer) to call REST services.

  **URI format** 

The following components support rest producer:rest://method:path[:uriTemplate]?[options]
  
  **Supported rest components**
  
  The following components support rest consumer (Rest DSL):
  
   1- camel-coap

   2- camel-netty-http

   3- camel-netty4-http

   4- camel-jetty

   5- camel-restlet

   6-camel-servlet

   7-camel-spark-rest

   8-camel-undertow

The following components support rest producer:

    1-camel-http

    2-camel-http4

    3-camel-netty4-http

    4-camel-jetty

    5-camel-restlet

    6-camel-undertow


  ## How to Test REST API

API testing requires an application to interact with API. To test an API, you require two things, 
  
   1- Testing Tool/Framework to drive the API
  
   2- Writing down your own code to test the API
  
 Rest API can be tested with tools like:

    Advanced Rest Client
    Postman-Rest Client
    Curl in Linux

  
## Code for Testing rest api  
  ![reast](https://user-images.githubusercontent.com/82276807/119935088-890ffc00-bfa4-11eb-9818-0a681b13a4e7.png)

  ## Dependency that we have used
  
  ![dependency](https://user-images.githubusercontent.com/82276807/119937346-3cc6bb00-bfa8-11eb-815a-ce0ea42e0239.png)
  
  ###  Command by which we hit our API
  
  For GET METHOD- curl -X GET http://localhost:8020/api/getdbdata
  
  For POST MEHOD - curl -d '{"name": "ram", "age":"27"}' -H "content-type:application/json" -X POST http://localhost:8010    /api/getDBData  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
