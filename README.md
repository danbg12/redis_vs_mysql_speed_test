# World Data Accessor

This Java mini-project provides access to geographical and demographic data from a database using Hibernate ORM. The project follows the separation of concerns principle and uses Maven for dependency management.

## Project Structure

- **com.javarush.dao**
    - `CityDAO`, `CountryDAO` – Data Access Object (DAO) classes for managing access to city and country data.

- **com.javarush.domain**
    - JPA entities representing database tables: `City`, `Country`, `CountryLanguage`, `Continent`.
    - The `redis` subpackage is reserved for potential Redis integration (currently may be empty or under development).

- **Main** – the main entry point class of the application.

## Configuration Files

- **hibernate.properties** – Hibernate configuration file.
- **spy.properties** – additional configuration for SQL query logging (likely using the P6Spy library).

## Requirements

- JDK 17+
- Maven 3.6+
- A compatible database (MySQL / PostgreSQL, etc.)
- Hibernate Core
- (Optional) P6Spy for query logging

## Running the Application

Make sure the database is properly configured in `hibernate.properties`, then run the `Main` class to initialize the application logic.

```bash
mvn clean install