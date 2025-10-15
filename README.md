# Hello World API

A Java-based API service built with Maven and OpenAPI.

## Prerequisites

- Java 17 or higher
- Apache Maven 3.6.0 or higher

## Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd hello-world-api
   ```

2. **Build the project**
   ```bash
   mvn clean install
   ```

3. **Run the application**
   ```bash
   mvn spring-boot:run
   ```

## Project Structure

```
hello-world-api/
├── src/                   # Source files
│   ├── main/             
│   │   ├── java/         # Java source code
│   │   └── resources/    # Configuration files
│   └── test/             # Test files
├── target/               # Compiled output (ignored by git)
├── pom.xml               # Maven configuration
└── README.md             # This file
```

## API Documentation

Once the application is running, you can access:

- **Swagger UI**: `http://localhost:8080/swagger-ui.html`
- **OpenAPI Documentation**: `http://localhost:8080/v3/api-docs`

## Development

### Building

```bash
mvn clean package
```

### Running Tests

```bash
mvn test
```

### Code Style

This project follows standard Java coding conventions. Please ensure your code is properly formatted before committing.

## License

[Specify your license here]

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
