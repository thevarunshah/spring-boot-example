# Spring-Boot Example
A web application template using spring boot <br>
Uses Java as the backend language and Thymeleaf to parse in HTML <br>

# How to Run
Build using Maven (https://maven.apache.org/) <br>
*runs on port 8080 by default.<br>
Run the following commands on a terminal: <br>
0) //navigate to the folder which contains pom.xml <br>
1) mvn clean <br>
2) mvn spring-boot:run <br>

# Project Structure and File Details
The <b>pom.xml</b> file contains project specifications and all the dependencies for your project. <br>
The <b>src/main/java</b> folder contains all of your Java classes (the backend). 
  - The <b>Application.java</b> file is the entry point for the spring-boot app - this class contains the main method. 
  - The <b>GreetingController.java</b> file contains all of the relevant endpoints for your app. 
    - Each endpoint has a RequestMapping annotation.
    - The Model object passed into the method is used to pass variables to your frontend. 

The <b>src/main/resources</b> folder contains all of your frontend resources. 
  - The <b>templates</b> folder contains all of your HTML pages.
    - The <b>th</b> classifier is used to parse certain thymeleaf specific HTML attributes.
    - <b>${variableName}</b> is used to refer to variables passed via the Model object.
  - A <b>static</b> folder can be added under resources for static resources such as CSS and JavaScript.
