# **📽️Cinema app📽️**


![Cinema-HD-for-Windows-PC](https://user-images.githubusercontent.com/96648890/190856735-14ba2155-ce2a-4efa-8629-28988d83aea5.jpg)

<!-- ABOUT THE PROJECT -->
## **📢Project Description**

A simple application that simulates a cinema's ticket-reservation system. It contents only with backend part.
Manage cinema by adding new movies, movie sessions, adding cinema halls. With registering new user the shopping cart linked to user will be created. After login as user add movie sessions to shopping cart and create orders to purchase tickets.



## 💻Implementation details

Project based on 2-layer architecture:

- Application layer (services)
- Data access layer (DAO)

## ⚡Project configuration

1. Clone this project to your IDE as Maven project.
2. Check a pom.xml file if any errors are occurred - fix them.
3. Open MySql. It can be local or remote database. Create schema.
4. To configure connection to database open hibernate.cfg.xml
(src/main/resources/hibernate.cfg.xml)
5. Edit these fields according to your data: 

````
<property name="connection.url"><jdbc:mysql://<URL_TO_DATABASE>:<PORT_NUMBER>/<DATABASE_NAME>?serverTimezone=UTC></property>
<property name="connection.username"><DATABASE_USERNAME></property>
<property name="connection.password"><DATABASE_PASSWORD></property>
````  
   
  where:
- <URL_TO_DATABASE> - URL to Database (for local database: localhost)
- <PORT_NUMBER> - port number of database (for local database: 3306)
- <DATABASE_NAME> - name of database(for local database: cinema_app)
- <DATABASE_USERNAME> - username to get permission to read and write to database
- <DATABASE_PASSWORD> - password for <DATABASE_USERNAME> user

## 🧧Application functionality

1. Registration/authentication
2. Add/get movie;
3. Add/get cinema hall;
4. Add/get/get all by date movie sessions;
5. Add session to shopping cart;
6. Complete order after adding sessions to shopping cart;
7. Get order history for user

## 🔥Application technologies used

- JDK 11
- Maven
- MySQL
- Hibernate
- HQL

## 📊Diagram of DB tables relations

![Hibernate_Cinema_Uml](https://user-images.githubusercontent.com/96648890/190859151-a9cdc3b6-e28a-4b56-93ba-65b1c2017515.png)
