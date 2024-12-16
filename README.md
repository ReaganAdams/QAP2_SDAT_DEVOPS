Features

Member Management

Create Member: Add new members to the system.

Search Members:

By name

By membership type (duration)

By phone number

By membership start date

Tournament Management

Create Tournament: Register new tournaments.

Search Tournaments:

By start date

By location

Retrieve all members participating in a specific tournament

Member-Tournament Interaction

Add Members to Tournaments: Link members to tournaments.

View Participating Members: List all members for a given tournament.

Prerequisites

Ensure the following tools are installed on your system:

Docker

Docker Compose

Java 17

Maven

MySQL (if running the database locally)

1. Clone the Repository

git clone <repository_url>
cd <repository_name>

2. Configure the Database

The project uses a MySQL database named golf1. If you're not using Docker for the database, ensure you create the database manually:

CREATE DATABASE golf1;

Update the database credentials in src/main/resources/application.properties if necessary.

3. Build the Project

Run the following command to build the project:

mvn clean install

4. Run Using Docker

To start the application and database using Docker, run:

docker-compose up --build

This command will:

Start a MySQL database container.

Build and start the Spring Boot application container.

The application will be available at http://localhost:8080.

