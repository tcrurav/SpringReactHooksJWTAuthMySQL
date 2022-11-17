# Testing from bezcoder (Spring Boot + React + MySQL + JWT Authentication)

It's just that... Just testing from bezcoder. This project is putting together 2 of the examples of bezcoder site using Spring Boot + JWT Authentication + React with hooks without Redux + MySQL.

## Getting Started

For the initial steps give a try to my following video for the basics of Spring:
https://www.youtube.com/watch?v=DvzGf0cAlg4

It's a step by step guide to understand how to make a Spring project implementing RESTFul and JPA accessing MySQL.

For this project please read the links at the bottom of this README.md file. It's so well explained by bezcoder.

### For the most impatient learners

Clone this project:

````
git clone https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL.git
````

Open the backend with Eclipse and change the backend/src/main/resources/application.properties according to your database credentials.

In your database you will notice this is the Entity-Relationship Diagram:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/MySQLDiagram.png)

In your database table roles add the following data:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/roles.png)

Now you can start your backend project.

And after that create with POSTMAN your first user:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/signup.png)

The result in the tables of the database is the following:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/TableUsersAfterSignUp.png)

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/TableUsersRolesAfterSignUp.png)

Now you can login with the created user using POSTMAN:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/login.png)

With the token obtained after login you can test you can access with your user role (ROLE_USER):

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/userAccessContentWithToken.png)

And also is interesting to test that the user cannot access an end-point which needs other Role to access:

![screenshots](https://github.com/tcrurav/SpringReactHooksJWTAuthMySQL/blob/master/screenshots/userCannotAccessModeratorContentWithHisUserToken.png)

There are a lot of more tests you can accomplish like creating a user with other role and test what he/she can access and not.

After that you can try the React frontend.

For that do the following:

````
cd frontend
npm install
npm start
````

And now just signup and login with a user to test it all.

Enjoy!!!

### Prerequisites

All you need is... some time and...
* Eclipse IDE.
* STS 4, installed through the Eclipse Marketplace.
* MySQL Workbench, to host the database also included in the project.
* PostMan, for the RESTFul tests.
* More hours than you first could think of...

## Built With

* [Eclipse IDE](https://www.eclipse.org/ide/) - The IDE used
* [Maven](https://maven.apache.org/) - Dependency Management
* [Spring Tools 4](https://spring.io/tools) - The framework used
* [MySQL Workbench](https://www.mysql.com/products/workbench/) - The Database used

## Acknowledgments

* https://www.bezkoder.com/spring-boot-jwt-authentication/. Spring Boot Token based Authentication with Spring Security & JWT
* https://github.com/bezkoder/spring-boot-spring-security-jwt-authentication. Spring Boot JWT Authentication example with Spring Security & Spring Data JPA
* https://www.bezkoder.com/react-hooks-jwt-auth/. React Hooks: JWT Authentication (without Redux) example
* https://github.com/bezkoder/react-hooks-jwt-auth. React Hooks: JWT Authentication (without Redux) example
* https://www.getpostman.com/. Used to test the RESTFul end points of the project.
* https://gist.github.com/PurpleBooth/109311bb0361f32d87a2. A very complete template for README.md files.