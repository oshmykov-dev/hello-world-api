# Hello World API

A Java-based API service built with Maven and OpenAPI. This project is tightly coupled with the [hello-world-spec](https://github.com/oshmykov-dev/hello-world-spec) package, which contains the OpenAPI specification and generated models.

## Prerequisites

- Java 17 or higher
- Apache Maven 3.6.0 or higher
- GitHub Personal Access Token with `read:packages` scope
- GitHub Package Registry access to [oshmykov-dev/hello-world-spec](https://github.com/oshmykov-dev/hello-world-spec)

## Configuration

### GitHub Package Registry Authentication

1. Create a GitHub Personal Access Token with `read:packages` scope from [GitHub Settings](https://github.com/settings/tokens)

2. The project includes a `.mvn/settings.xml` file that's already configured for GitHub Package Registry access. You just need to update it with your GitHub credentials:

   - Open `.mvn/settings.xml`
   - Replace `YOUR_GITHUB_USERNAME` with your GitHub username
   - Replace `YOUR_GITHUB_TOKEN` with your Personal Access Token

This settings file is automatically used by Maven when building the project.

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

## Dependencies

This project depends on the following external package:

- **hello-world-spec**: Contains the OpenAPI specification and generated models
  - GitHub: [oshmykov-dev/hello-world-spec](https://github.com/oshmykov-dev/hello-world-spec)
  - GitHub Packages: [View Packages](https://github.com/oshmykov-dev/hello-world-spec/packages/)
  - Maven: `com.example.helloworld:hello-world-spec`

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

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
