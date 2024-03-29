# Kaiburr Task 1
## Java REST API example

### Problem Statement

Implement an application in Java that provides a REST API with endpoints for searching,
creating, and deleting “task” objects. Each “task” object should contain the following properties:  
&emsp;● name (task name, string)  
&emsp;● id (task ID, string)  
&emsp;● assignee (task assignee, string)   
&emsp;● project (project name, string)  
&emsp;● startTime (task start date/time, date)  
&emsp;● special property based on the candidate (your) name. For example, if the candidate's
name is Rajesh Singh, the property name will be “rajeshSinghProperty”. The value of
this property should be set to 5 random characters from the string “RajeshSingh”. Values
for “rajeshSinghProperty” should be generated by the program only.


### Tech Stack Used
&emsp;● Java Springboot  
&emsp;● MongoDB ATLAS  
&emsp;● SpringToolSuite IDE

### Pre-requisites 
Ensure that the JDK version in your system is at least JDK 17 and above. 

### Ways to run the REST API locally on your system
&emsp;1. Use git clone https://github.com/M-JB413/KaiburrTask1.git to download the files locally and then import the folder inside Eclipse.  
&emsp;2. cd into the Tasks Directory  
&emsp;3. Create a .env file with the following key-value pairs:  
&emsp;&emsp;● MONGO_CLUSTER={Cluster ID}  
&emsp;&emsp;● MONGO_USER={User ID}  
&emsp;&emsp;● MONGO_DATABASE={Database Name}  
&emsp;&emsp;● MONGO_PASSWORD={User's Password}  
&emsp;4. Import the Tasks folder as a project using the IDE. 
&emsp;5. Wait for Maven to setup the project and once complete run the project as Spring Boot App  
NOTE - Ensure that PORT 8080 is not occupied in your system. The REST API Server runs on Port 8080

### Screenshots

#### /create - Post or Create a new Document in the database
![Create](https://github.com/M-JB413/KaiburrTask1/assets/83492132/94638e36-6a09-488c-90f5-26fc4ce685c0)


#### /get - Get all the documents from the database
![RetreiveAll](https://github.com/M-JB413/KaiburrTask1/assets/83492132/3a8a3e1d-fd3f-4826-b49c-5d6390421fca)


#### /get/name/{name} - Get documents that contain the search substring in the name field
![GetName](https://github.com/M-JB413/KaiburrTask1/assets/83492132/9e5bb326-6d6c-4f4d-9d13-427ef2d1ba58)


#### /get/assignee/{assignee} - Get documents that equal the search string in the assignee field
![GetAssignee](https://github.com/M-JB413/KaiburrTask1/assets/83492132/92780805-b588-45bc-a78b-fe7f1e4f93f7)


#### /delete/{id} - Delete the document with given ID
![Delete](https://github.com/M-JB413/KaiburrTask1/assets/83492132/cc8548b9-a550-4631-8a44-13b493e1e1ea)

