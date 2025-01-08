# html-report-viewer

A microservices-based application to parse HTML test reports, store results in a database, and visualize them on a web application.

## Project Structure

- `uploader-service`: REST API to upload HTML reports.
- `parser-service`: Consumes RabbitMQ messages, parses HTML, and sends data to the database.
- `database-service`: Stores and retrieves test data.
- `visualizer-service`: Provides APIs for visualization and comparison.

## Setup Instructions

1. Clone the repository: `git clone <repo-url>`
2. Navigate to the service folder to set up each microservice.

## Technologies Used
- **Java (Spring Boot):** Uploader, Database, and Visualizer services.
- **Python (BeautifulSoup):** Parser service.
- **RabbitMQ:** Message broker for communication between services.
- **Docker Compose:** For orchestration of all services.