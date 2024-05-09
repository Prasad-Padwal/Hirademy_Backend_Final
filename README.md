### Assistant Management System

This project is a backend application designed to manage assistants using CRUD APIs. It allows users to perform operations like creating, reading, updating, and deleting assistant records. The application is built using Spring Boot and MYSQL, and it includes API endpoints for interacting with the assistant data.
Prerequisites: -
Java Development Kit (JDK) installed (version 8 or higher)
Maven installed
MySQL installed and running
Installation: -
Clone the repository:

git clone https://github.com/Prasad-Padwal/Hirademy_Backend_Final.git
Set up the database:
Create a MySQL database named assdb
Update the database configuration in src/main/resources/application.properties
spring.application.name=AssistantMangementSystem
spring.datasource.url=jdbc:mysql://localhost:3306/assdb
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

Run the application:
cd assistant-management-system 
mvn spring-boot:run

OR 

Right click on project in STS and Run as SpringBoot app



### API Endpoints
GET /api/assistants: Retrieve a list of all assistants.
GET /api/assistants/{id}: Retrieve details of a specific assistant by ID.
POST /api/assistants: Create a new assistant.
PUT /api/assistants/{id}: Update details of a specific assistant by ID.
DELETE /api/assistants/{id}: Delete a specific assistant by ID.

### Postman Collection
A Postman collection is provided to test the API endpoints. Follow these steps to use it:
Import the collection:
Download the Postman collection.
Open Postman and click on the "Import" button.
Select the downloaded JSON file.
Set environment variables:
Create a new environment in Postman.
Define variables for base_url (e.g., http://localhost:8080/api) and any other necessary variables.
Test the endpoints:
Use the imported collection to test each endpoint with different requests (GET, POST, PUT, DELETE).

