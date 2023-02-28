# Cinema App 🎬

Cinema App is a pet web application built using Spring and Hibernate frameworks. It allows users to send HTTP requests (GET, PUT, POST, DELETE) and work with JSON objects. The app was implemented following SOLID and OOP principles. It was developed using the CRUD methodology. The Cinema App has secured user authentication and authorization features.

## Project Structure 📁

Cinema App follows a standard project structure for Spring-based applications. Here is overview of the structure:

- `java`: This directory contains all the Java code of the application.

    - `config`:  Configuration classes of our application.

    - `controller`: Controller classes that handle the incoming requests.

    - `dao`: Classes that provide work with database.

    - `dto`: Data transfer objects for working with users.

    - `exception`: Custom exception classes used in the application.

    - `lib`: Custom annotations used for validating input data.

    - `model`: Entity classes used in the application.

    - `service`: Service classes that provide business logic.

    - `util`: Utility classes.

- `resources`: This directory contains the `db.properties` file, that has the database configuration.

### Current project functionality:
Here is the list of all endpoints with role required for access and their short description:
- GET: /cinema-halls - (user/admin) - get a list of all cinema halls.
- GET: /movies - (user/admin) - get a list of all movies.
- GET: /movie-sessions/available - (user/admin) - returns available movie sessions for specified movie and date.
- GET: /orders - (user) - get list of orders for current user.
- GET: /shopping-carts/by-user - (user) - get shopping cart of current user.
- GET: /users/by-email - (admin) - get user by email.
- POST: /register - (all) - register as a new user.
- POST: /cinema-halls - (admin) - create a new cinema hall.
- POST: /movies - (admin) - create a new movie.
- POST: /movie-sessions - (admin) - create movie session.
- POST: /orders/complete - (user) - create a new order for current user (transfer movie tickets from shopping cart to order and clear shopping cart).
- PUT: /movie-sessions/{id} - (admin) - update movie session.
- PUT: /shopping-carts/movie-sessions - (user) - creates a ticket for specified movie session and adds it to shopping cart of current user.
- DELETE: /movie-sessions/{id} - (admin) - delete movie session.


As you can see above this app has two roles: user and admin. User role is assigned automatically to every new user created.  

## Technologies & Requirements 🎥
Cinema App was built using the following technologies and patterns:

- IDE
- Java 17, MySQL, Tomcat v.9.0.5, Maven
- Spring Web MVC, Spring Security, Hibernate
- OOP, SOLID, CRUD
- Postman

## Installation 💻

Here are the steps to run this app locally:

1. Clone this repository and open it locally.
2. Add all the required configurations to db.properties file.
3. Install Tomcat.
4. Run the app.
5. Check which links and methods are available in [Readme.md](README.md) (functionality).
6. Connection established! 🎉

If you'd like to fork this project, feel free to use it in your own.
