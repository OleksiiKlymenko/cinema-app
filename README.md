# Cinema App
______________________
### Description
This project allow you to manage your own cinema. Here we have two 
roles ADMIN and USER, each of these roles has own features, use following 
endpoints to try all functionality:
- `POST: /register` - to register new user (USER Role by default)
- `GET: /cinema-halls`  - for USER and ADMIN, to get all available cinema halls
- `POST: /cinema-halls` - for ADMIN, to create a cinema hall
- `GET: /movies` - for USER and ADMIN, to get all available movies
- `POST: /movies` - for ADMIN, to create a movie
- `GET: /movie-sessions/available` - for USER and ADMIN, to get all available movie sessions (depends on showtime)
- `POST: /movie-sessions` - for ADMIN, to create a movie session based on the movie, the cinema hall and the showtime
- `PUT,DELETE: /movie-sessions/{id}` - for ADMIN, to update or delete a movie session by its ID
- `PUT: /shopping-carts/movie-sessions` - for USER, to add a ticket to a movie session in the user's shopping cart
- `GET: /shopping-carts/by-user` - for USER, to get tickets in the user's shopping cart
- `POST: /orders/complete` - for USER, to buy tickets in the shopping cart
- `GET: /orders` - for USER, to get order history by user
- `GET: /users/by-email` - for ADMIN, to find a user by email

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
- Configure file to connect to db - `src/main/resources/db.properties`
- Configure Tomcat (Better to use version lower than Tomcat 10)
- Using Postman you can try all features of this project, use `http://localhost:8080` as a start point

### Author
____
Oleksii Klymenko
