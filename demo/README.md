# Spring Boot Login System

This is a simple Spring Boot login system that demonstrates basic authentication functionality.

## Features

- Login page with username/password authentication
- Simple hardcoded authentication (admin/password)
- Home page after successful login
- Modern, responsive UI

## How to Run

### Prerequisites
- Java 8 or higher (JDK required for compilation)
- Gradle 6.8.3 or compatible version

### Running the Application

1. **Compile and run the application:**
   ```bash
   cd demo
   ./gradlew bootRun
   ```

2. **Access the application:**
   - Open your web browser
   - Navigate to: `http://localhost:8080/login`

### Demo Credentials
- **Username:** admin
- **Password:** password

## Project Structure

```
demo/
├── src/main/java/com/example/demo/
│   └── SimpleLoginApplication.java    # Main application class with controllers
├── src/main/resources/
│   ├── application.properties         # Application configuration
│   └── templates/
│       ├── login.html                 # Login page template
│       └── home.html                  # Home page template
└── build.gradle                       # Build configuration
```

## Troubleshooting

### Java Version Issues
If you encounter Java version issues:
1. Ensure you have JDK (not just JRE) installed
2. Check your JAVA_HOME environment variable
3. Verify Java version: `java -version`

### Port Already in Use
If port 8080 is already in use:
1. Change the port in `application.properties`:
   ```properties
   server.port=8081
   ```
2. Access the application at `http://localhost:8081/login`

## Technology Stack

- **Spring Boot 2.1.18**
- **Spring Web**
- **Thymeleaf** (for templating)
- **Gradle** (for build management)

## Notes

This is a simplified demo application for educational purposes. In a production environment, you would want to:
- Use proper password encryption
- Implement database-backed user management
- Add proper security configurations
- Use HTTPS
- Implement proper session management
