# Liquibase Data Types Project

This project is a Java application that uses Liquibase for database migrations. 

## Project Structure

```
liquibase-data-types
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── avilaqdaniel
│   │   │           └── App.java
│   │   ├── resources
│   │       ├── db
│   │       │   ├── changelog
│   │       │   │   └── db.changelog-master.xml
│   │       └── liquibase.properties
│   └── test
│       ├── java
│       │   └── com
│       │       └── avilaqdaniel
│       │           └── AppTest.java
│       └── resources
├── pom.xml
└── README.md
```

## Setup Instructions

1. **Clone the repository:**
   ```
   git clone <repository-url>
   cd liquibase-data-types
   ```

2. **Build the project:**
   ```
   mvn clean install
   ```

3. **Configure Liquibase:**
   Update the `src/main/resources/liquibase.properties` file with your database connection details.

4. **Run the application:**
   ```
   mvn exec:java -Dexec.mainClass="com.avilaqdaniel.App"
   ```

## Usage

The application initializes and runs Liquibase migrations defined in `db.changelog-master.xml`. Ensure your database is accessible and the connection properties are correctly set in `liquibase.properties`.

## Testing

Unit tests are located in the `src/test/java/com/avilaqdaniel/AppTest.java` file. You can run the tests using:
```
mvn test
```

## License

This project is licensed under the MIT License.