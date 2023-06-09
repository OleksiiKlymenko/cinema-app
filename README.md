# Movie Ticket App
______________________
### Description
This project allow you to manage your own cinema. Here we have two 
roles ADMIN and USER, each of these roles has own features, use following 
endpoints to try all functionality. In this app you can register new User as User or Admin. 
If you login as a User you can get all available movies, cinema halls and movie session. Add ticket to movie session in your cart 
and buy tickets in the shopping cart. If you are Admin you can create movies, cinema halls, movie session and find user by email.


### List of endpoints
- `POST: /register` - to register new user (USER Role by default)
- `GET: /cinema-halls`  - for USER and ADMIN
- `POST: /cinema-halls` - for ADMIN
- `GET: /movies` - for USER and ADMIN
- `POST: /movies` - for ADMIN
- `GET: /movie-sessions/available` - for USER and ADMIN
- `POST: /movie-sessions` - for ADMIN
- `PUT,DELETE: /movie-sessions/{id}` - for ADMIN
- `PUT: /shopping-carts/movie-sessions` - for USER
- `GET: /shopping-carts/by-user` - for USER
- `POST: /orders/complete` - for USER
- `GET: /orders` - for USER
- `GET: /users/by-email` - for ADMIN

### Structure
___

- `src/main/java/cinema` - Here you can find all packages which contains all logic of this app. The project has 3-Tier Architecture
- `src/main/resources/db.properties` - configuration file for connecting to data base


### Used Technologies
___

- Java `17`
- Apache Maven `3.3.2`
- Apache Tomcat `9.0.75`
- MySQL `8.0.22`
- Spring `5.3.20`
- Spring Security `5.6.10`
- Hibernate `5.6.14.Final`

### How to start project
___

- Clone this repository using SSH - `git@github.com:OleksiiKlymenko/cinema-app.git`
- Configure file to connect to db, because app uses MySQL - `src/main/resources/db.properties`
- Download and Install Apache Tomcat
- Configure Apache Tomcat:
  Artifact: war-exploded artifact
  Application context: "/"
- Using Postman you can try all features of this project, use `http://localhost:8080` as a start point

### Author
____
Oleksii Klymenko
