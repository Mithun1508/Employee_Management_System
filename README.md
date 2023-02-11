# Employee-Management-System 
![7debfbba-7670-4801-9d4f-fad70f0f4666](https://user-images.githubusercontent.com/93249038/215545052-88e9a412-7608-42e8-ba66-ab7af23aafe2.gif)

Employee management using spring mvc, spring data jpa, ehcache, jsp, javascript and apache tomcat.

Description: It's an employee management system, exposed to users as both web and rest service, with which users can perform basic crud operations and also search employees filtered using fields. This code can be used to understand how spring modules can be used to create an web application with client to backend and vice versa dataflow.

   Application to manage Employee Information. HR application to store all the employee information in a single place. This includes different modules like Employee Personal Information, Immigration information, Timsheet information, Payroll information etc.,


 This repository consists of Java Program for Employee Management System. In this repository I have created a TUI program for Employee Management System which consists of 4 different operation.

(1) Adding User

(2) Removing User

(3) Updating User

(4) Viewing details of User

The Program is completely based on OOPs concept.

## Technologies Used:

1 Persistence - Spring data jpa with hibernate, c3po for conection pooling, mysql.

2 Spring mvc - It provides model-view-controller architecture and ready components that can be used to develop flexible and loosely coupled web applications and also expose rest services.

3 Caching - ehcache

4 Web Technologies - jsp, javascript

5 Server - Apache Tomcat

6 Logging - slf4j, logback-classic

7 Eclipse Neon 4.6.0

8 MySQL Workbench

9 Postman for Chrome: Version 4.10.5

## Build Configuration: clean package Run Configuration: tomcat:run -Dmaven.tomcat.port=8081

## How To Run:

Create required database. Either use employee_database.sql or create them manually or change hibernate.hbm2ddl.auto property in application-config to create and again change it back to validate after first run.

Change the database properties in jdbc.properties according to your mysql.

# HOW TO RUN THIS PROJECT?# ###FROM THE IDE:###

Open the project in an IDE like Eclipse.

You can run the DBScript provided in MySQL to create database and tables with basic values. (Creating database is necessary since hibernate- update option is used : "spring.jpa.hibernate.ddl-auto = update")

In case you do not want to run file, you can change the line "spring.jpa.hibernate.ddl-auto = update" to "spring.jpa.hibernate.ddl-auto = create-drop" in src/main/resources/application.properties file.

Check your database connection in src/main/resources/application.properties file and change if needed.

Go to com.employee.management

Right Click on class Application.

Hit "Run As Java Application" in the IDE.

Check if localhost server has started.

Open Postman client service on Google chrome.

Hit url : "http://localhost:8080/employees" and url : "http://localhost:8080/departments"

Accordingly select the request method and the url as follows: Department: GET - "http://localhost:8080/departments" - gets list of all departments GET - "http://localhost:8080/departments/{id}" - gets department with selected id POST - "http://localhost:8080/departments" - inserts into department PUT - "http://localhost:8080/departments/{id}" - updates departments with selected id DELETE - "http://localhost:8080/departments" - deletes all departments DELETE - "http://localhost:8080/departments/{id}" - deletes departments with selected id PATCH - "http://localhost:8080/departments/{id}" - patches/updates departments with selected id

Employee: GET - "http://localhost:8080/employees" - gets list of all employees GET - "http://localhost:8080/employees/{id}" - gets employees with selected id POST - "http://localhost:8080/employees" - inserts into employees PUT - "http://localhost:8080/employees/{id}" - updates employees with selected id DELETE - "http://localhost:8080/employees" - deletes all employees DELETE - "http://localhost:8080/employees/{id}" - deletes employees with selected id PATCH - "http://localhost:8080/employees/{id}" - patches/updates employees with selected id

# ASSUMPTIONS#

DATABASE and TABLES are created in MySQL

DepartmentID is a foreign key in Employee table.

Make sure department table is populated with the department you refer for in employee.

While inserting employee detail through postman service: give a department id for department. Eg: { "employeeID": 2, "firstName": "Tim", "lastName": "Cook", "department": 3 }

# DESIGN DISCUSSION#

The employee table has a department id foreign key.

Department table needs to have a value existing to be referred by the employee table.

Get mapping will fetch the results, Post mapping will insert results, Put mapping and Patch mapping will update results, Delete mapping will delete results.

You will need to create database if not, change in the application.properties file.

Ease of extending the program

You can add useraccount table and assign username and password details for the employee.

You can also create a system account who handles all the creation and deleting of employee and department.




## TOPICS COVERED IN THIS PROJECT:

 ## 1) Used protocols : HTTP,UDP,TCP, Client-sever 
   
 ## 2) How caching Working underneath the code 

 ## 3) Database used : MYSQL 
 
 ## 4) Tomcat installed in Machine, POSTMAN, ECLIPSE 
 
 ## 5) JSP & Thymeleaf - fRONTEND PART
 
 ## 6) SERVLET - BACKEND
 
 ## 7) JDBC CONNECT THE DATABASE WITH java class
 
 ## 8) Hibernate (ORM) CONFIGURATIONS CRUD 
 


![Screenshot_2023-02-11-19-05-56-42_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262811-04843ba3-8655-445a-96f7-1749ad387c79.jpg)
![Screenshot_2023-02-11-19-06-15-90_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262823-30c86d73-fa56-4247-a087-f80f1463b4ff.jpg)


![Screenshot_2023-02-11-19-08-49-59_f9ee0578fe1cc94de7482bd41accb329 (1)](https://user-images.githubusercontent.com/93249038/218262627-99737d83-fb96-42d7-a97b-9bba31a33756.jpg)
![Screenshot_2023-02-11-19-09-09-72_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262634-ab5df624-07ee-440c-8403-e843ac1535b4.jpg)
![Screenshot_2023-02-11-19-09-42-55_f9ee0578fe1cc94de7482bd41accb329 (1)](https://user-images.githubusercontent.com/93249038/218262640-ac7e1c66-95cc-4919-9aef-282de30c5e73.jpg)
![Screenshot_2023-02-11-19-09-42-55_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262650-7ab0dcd7-77e8-4a4d-9319-0a599b263e6c.jpg)
![Screenshot_2023-02-11-19-10-51-48_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262655-156271cd-cc21-457d-b72b-d1bf52f41a89.jpg)
![Screenshot_2023-02-11-19-11-36-26_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262668-1872471b-be31-43a7-8c2e-c5dc07a22aa6.jpg)
![Screenshot_2023-02-11-19-11-57-93_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262681-66b9b3c5-8be3-47b6-a73f-2e14a1dd57e8.jpg)
![Screenshot_2023-02-11-19-13-12-63_f9ee0578fe1cc94de7482bd41accb329](https://user-images.githubusercontent.com/93249038/218262764-811e8abc-6cb4-4484-8356-a425d5214fea.jpg)

# SOFTWARE DOWNLOAD REFERENCES:

https://code.visualstudio.com/

https://www.oracle.com/in/java/technologies/downloads/

https://docs.oracle.com/en/java/

https://netbeans.apache.org/download/nb123/nb123.html

https://www.apachefriends.org/download.html

https://dev.mysql.com/downloads/connector/j/


