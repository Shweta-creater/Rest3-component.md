## REST API Testing

𝓡𝓔𝓢𝓣 𝓐𝓟𝓘 𝓣𝓮𝓼𝓽𝓲𝓷𝓰 𝓲𝓼 𝓸𝓹𝓮𝓷-𝓼𝓸𝓾𝓻𝓬𝓮 𝔀𝓮𝓫 𝓪𝓾𝓽𝓸𝓶𝓪𝓽𝓲𝓸𝓷 𝓽𝓮𝓼𝓽𝓲𝓷𝓰 𝓽𝓮𝓬𝓱𝓷𝓲𝓺𝓾𝓮 𝓽𝓱𝓪𝓽 𝓲𝓼 𝓾𝓼𝓮𝓭 𝓯𝓸𝓻 𝓽𝓮𝓼𝓽𝓲𝓷𝓰 𝓡𝓔𝓢𝓣𝓯𝓾𝓵 𝓐𝓟𝓘𝓼 𝓯𝓸𝓻 𝔀𝓮𝓫 𝓪𝓹𝓹𝓵𝓲𝓬𝓪𝓽𝓲𝓸𝓷𝓼.*   *𝓣𝓱𝓮 𝓹𝓾𝓻𝓹𝓸𝓼𝓮 𝓸𝓯 𝓻𝓮𝓼𝓽 𝓪𝓹𝓲 𝓽𝓮𝓼𝓽𝓲𝓷𝓰 𝓲𝓼 𝓽𝓸 𝓻𝓮𝓬𝓸𝓻𝓭 𝓽𝓱𝓮 𝓻𝓮𝓼𝓹𝓸𝓷𝓼𝓮 𝓸𝓯 𝓻𝓮𝓼𝓽 𝓪𝓹𝓲 𝓫𝔂 𝓼𝓮𝓷𝓭𝓲𝓷𝓰 𝓿𝓪𝓻𝓲𝓸𝓾𝓼 𝓗𝓣𝓣𝓟/𝓢 𝓻𝓮𝓺𝓾𝓮𝓼𝓽𝓼 𝓽𝓸 𝓬𝓱𝓮𝓬𝓴 𝓲𝓯 𝓻𝓮𝓼𝓽 𝓪𝓹𝓲 𝓲𝓼*   *𝔀𝓸𝓻𝓴𝓲𝓷𝓰 𝓯𝓲𝓷𝓮 𝓸𝓻 𝓷𝓸𝓽. 𝓡𝓮𝓼𝓽 𝓪𝓹𝓲 𝓽𝓮𝓼𝓽𝓲𝓷𝓰 𝓲𝓼 𝓭𝓸𝓷𝓮 𝓫𝔂 𝓖𝓔𝓣, 𝓟𝓞𝓢𝓣, 𝓟𝓤𝓣 𝓪𝓷𝓭 𝓓𝓔𝓛𝓔𝓣𝓔 𝓶𝓮𝓽𝓱𝓸𝓭𝓼.

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
  
  ### issue I have faced - when i am sending data from post method, the data is not being sent through the curl command.  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
