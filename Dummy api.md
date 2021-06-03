<img src="https://ezeiatech.com/wp-content/uploads/2019/05/apache-camel-interview-questions.jpg">

<h1 align="center"> 𝐂𝐚𝐦𝐞𝐥 𝐑𝐞𝐬𝐭𝐥𝐞𝐭 𝐜𝐨𝐦𝐩𝐨𝐧𝐞𝐧𝐭<h1>



# 𝐑𝐄𝐒𝐓 𝐀𝐏𝐈 𝐓𝐞𝐬𝐭𝐢𝐧𝐠

*Rest stands for Representational State Transfer. It is an architectural style and an approach for communication used in the* 

*development of Web Services. REST has become a logical choice for building APIs. It enables users to connect and interact with cloud services efficiently.*

*An API or Application Programming Interface is a set of programming instructions for accessing a web-based software application.
In other words, a set of commands used by an individual program to communicate with one another directly and use each other's functions to get information.*

*For example, a Google website can have API for various functions like search, translations, calendars, etc.*

*In general API's are like below, they have server name, paths.., etc*

*http://<server name>/v1/export/Publisher/Standard_Publisher_Report?format=csv*
  
  <em>There are mainly 4 methods involve in API Testing like GET, POST, Delete, and PUT.</em> 
  
  ### 𝐆𝐄𝐓
         GET method is used to extract information from the given server using a given URI. While using GET request, it should only extract data and should have no other effect on the data. 

  ### 𝐏𝐎𝐒𝐓
           A POST request is used to create a new entity. It can also be used to send data to the server, for example customer information, file upload, etc. using HTML forms.
  
  ### 𝐏𝐔𝐓
          Create a new entity or update an existing one.
  
  ### 𝐃𝐄𝐋𝐄𝐓𝐄
          Removes all current representations of the target resource given by a URI.
  
  <br>
  <details close="close"> 
  <summary><b>Code Pic</b></summary>   
 <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119935088-890ffc00-bfa4-11eb-9818-0a681b13a4e7.png"></p>
  </details>
  
 1️⃣- In above code I have used get method in first route get method is used to extract information from the given server using a given URI. While using GET request, It should only extract data and should have no other effect on the data. 
  
 2️⃣-In second route I have used post method.A POST request is used to create a new entity. It can also be used to send data to the server, for example customer information, file upload, etc. using HTML forms.
  
  3️⃣-We can use multiple route IDs in a CamelContext project.But it should be noted that the name of each route ID should be different.
  
 4️⃣: -<from uri="restlet:http://localhost:8020/api/getdbdata In this line we will use Restlet component and here we will give the path of our get API
    


  <details close="close"> 
  <summary><b>𝐃𝐞𝐩𝐞𝐧𝐝𝐞𝐧𝐲 𝐰𝐡𝐢𝐜𝐡 𝐰𝐞 𝐡𝐚𝐯𝐞 𝐮𝐬𝐞𝐝</b></summary>   
  
 <p align ="center"><img src= "https://user-images.githubusercontent.com/82276807/119937346-3cc6bb00-bfa8-11eb-815a-ce0ea42e0239.png"></p>
When we send multiple requests at the same time through curl command then  </details>
  
   <details>
   <summary><b>𝐂𝐨𝐦𝐦𝐚𝐧𝐝 𝐛𝐲 𝐰𝐡𝐢𝐜𝐡 𝐰𝐞 𝐡𝐢𝐭 𝐨𝐮𝐫 𝐀𝐏𝐈</b></summary>
  
  For GET METHOD- curl -X GET http://localhost:8020/api/getdbdata
  
  For POST MEHOD - curl -d '{"name": "ram", "age":"27"}' -H "content-type:application/json" -X POST http://localhost:8010    /api/getDBData  
   </details>

  
    
  <details close="close"> 
  <summary><b>𝐈𝐬𝐬𝐮𝐞 𝐰𝐞 𝐡𝐚𝐯𝐞 𝐟𝐚𝐜𝐞𝐝</b></summary>  
    
 <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/120450508-2062be00-c3ae-11eb-9990-daf4e68c3c63.png"></p>   
  </details>
  
  1-When I was sending data from post method via the curl command.the data was not being sent and the restlet operation failing at         that time.
   
   2- When we send multiple requests at the same time through curl command then we come to this issue.
 

  <details>
    <summary><b>𝐑𝐞𝐟𝐞𝐫𝐞𝐧𝐜𝐞 𝐨𝐟 𝐬𝐢𝐭𝐞𝐬 𝐰𝐞 𝐡𝐚𝐯𝐞 𝐮𝐬𝐞𝐝 </b></summary>
  
  https://camel.apache.org/components/2.x/restlet-component.html
     </details>
  
  <br>
  <details close="close"> 
  <summary><b>𝐎𝐮𝐭𝐩𝐮𝐭 𝐰𝐡𝐞𝐧 𝐰𝐞 𝐬𝐞𝐧𝐝 𝐝𝐚𝐭𝐚 𝐟𝐫𝐨𝐦 𝐩𝐨𝐬𝐭 𝐦𝐞𝐭𝐡𝐨𝐝 𝐮𝐬𝐢𝐧𝐠 𝐝𝐮𝐦𝐦𝐲 𝐀𝐏𝐈 𝐯𝐢𝐚 𝐜𝐮𝐫𝐥 𝐜𝐨𝐦𝐦𝐚𝐧𝐝</b></summary> 
  
  
  <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119963539-d6509580-bfc5-11eb-8f95-b435dd1d996b.png"></p>
  </details>
  
 
  <br>
  <details close="close"> 
  <summary><b>𝐎𝐮𝐭𝐩𝐮𝐭 𝐰𝐡𝐞𝐧 𝐰𝐞 𝐞𝐱𝐭𝐫𝐚𝐜𝐭 𝐝𝐚𝐭𝐚 𝐟𝐫𝐨𝐦 𝐠𝐞𝐭 𝐦𝐞𝐭𝐡𝐨𝐝 𝐮𝐬𝐢𝐧𝐠 𝐝𝐮𝐦𝐦𝐲 𝐀𝐏𝐈 𝐯𝐢𝐚 𝐜𝐮𝐫𝐥 𝐜𝐨𝐦𝐦𝐚𝐧𝐝</b></summary> 
  
  <p align ="center"><img src="https://user-images.githubusercontent.com/82276807/119965082-8246b080-bfc7-11eb-9415-c9976c000fc8.png"></p>
      </details>


  
  
  
  
  
  
  
  
  
  
  
