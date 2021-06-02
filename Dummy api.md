<img src="https://ezeiatech.com/wp-content/uploads/2019/05/apache-camel-interview-questions.jpg">

<h1 align="center">Camel Restlet component <h1>



# REST API Testing

*Rest stands for Representational State Transfer. It is an architectural style and an approach for communication used in the* 

*development of Web Services. REST has become a logical choice for building APIs. It enables users to connect and interact with cloud services efficiently.*

*An API or Application Programming Interface is a set of programming instructions for accessing a web-based software application.
In other words, a set of commands used by an individual program to communicate with one another directly and use each other's functions to get information.*

*For example, a Google website can have API for various functions like search, translations, calendars, etc.*

*In general API's are like below, they have server name, paths.., etc*

*http://<server name>/v1/export/Publisher/Standard_Publisher_Report?format=csv*
  
  <em>There are mainly 4 methods involve in API Testing like GET, POST, Delete, and PUT.</em> 
  
  ### GET- 
         GET method is used to extract information from the given server using a given URI. While using GET request, it should only extract data and should have no other effect on the data. 

  ### POST-
           A POST request is used to create a new entity. It can also be used to send data to the server, for example customer information, file upload, etc. using HTML forms.
  
  ### PUT-
          Create a new entity or update an existing one.
  
  ### DELETE-
          Removes all current representations of the target resource given by a URI.
  
  <br>
  <details close="close"> 
  <summary><b>Code Pic</b></summary>   
 <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119935088-890ffc00-bfa4-11eb-9818-0a681b13a4e7.png"></p>
  </details>
  
 1- In above code I have used get method in first route get method is used to extract information from the given server using a given URI. While using GET request, It should only extract data and should have no other effect on the data. 
  
 2-In second route I have used post method.A POST request is used to create a new entity. It can also be used to send data to the server, for example customer information, file upload, etc. using HTML forms.
  
  
  
  


  <details close="close"> 
  <summary><b>Dependeny which I have used</b></summary>   
  
 <p align ="center"><img src= "https://user-images.githubusercontent.com/82276807/119937346-3cc6bb00-bfa8-11eb-815a-ce0ea42e0239.png"></p>
  </details>
  
  ###  Command by which we hit our API
  
  For GET METHOD- curl -X GET http://localhost:8020/api/getdbdata
  
  For POST MEHOD - curl -d '{"name": "ram", "age":"27"}' -H "content-type:application/json" -X POST http://localhost:8010    /api/getDBData  


  
     
    <details>
       <summary><b>Issue I have faced</b></summary>
 <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/120450508-2062be00-c3ae-11eb-9990-daf4e68c3c63.png"></p>   
  </details>
  
 1- When I was sending data from post method via the curl command.the data was not being sent and the restlet operation failing at       that time.
 

  <details>
    <summary> Reference of sites I have used </summary>
  https://www.guru99.com/testing-rest-api-manually.html
  
  https://camel.apache.org/components/2.x/restlet-component.html
     </details>
  
  
  <br>
  <br>
   <details close="close"> 
  <summary><b><Output when we send data from post method using dummy API via curl command/b></summary></b></summary>
  
  <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119963539-d6509580-bfc5-11eb-8f95-b435dd1d996b.png"></p>
  </details>
  
 
  
 <details> 
   <summary><b><Ouput when we extract data from get method using dummy API via curl command</b></summary> 
  <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119965082-8246b080-bfc7-11eb-9415-c9976c000fc8.png"></p>
      </details>


  
  
  
  
  
  
  
  
  
  
  
