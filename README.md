# X-Transact: Microservices-Based Banking Application

-Transact is a comprehensive banking application designed to demonstrate the implementation of microservices architecture using Spring Boot.he project encompasses distinct services for managing loans, cards, and accounts, and integrates advanced features such as containerization, message-driven solutions with Kafka, and monitoring tools including Prometheus, Grafana, Loki, and Promtail.dditionally, the application is orchestrated using Kubernetes for efficient deployment and scalability.
## Features

- **Accounts Microservice**: anages customer account information and related operations.- **Cards Microservice**: andles credit and debit card services, including issuance and management.- **Loans Microservice**: versees loan products, applications, and processing.- **Configuration Server**: entralized configuration management for all microservices.- **Eureka Server**: ervice discovery to facilitate communication between microservices.- **Gateway Server**: PI gateway that routes requests to the appropriate microservices.- **Message Broker**: mplements Apache Kafka for asynchronous communication between services.- **Monitoring and Logging**: ntegrates Prometheus and Grafana for monitoring, and Loki with Promtail for logging.- **Containerization and Orchestration**: tilizes Docker for containerization and Kubernetes for orchestration and management.
## Prerequisites

Before setting up the application, ensure you have the following installed:

- ava Development Kit (JDK) 11 or higher- ocker- ubernetes- pache Kafka- rometheus- rafana- oki- romtail
## Getting Started

1. **Clone the Repository**:

   ``bash
   git clone https://github.com/Aaditatgithub/X-Transact.git
   cd X-Transact
   ```
2. **Build the Microservices**:

   avigate to each microservice directory (`accounts`, `cards`, `loans`, etc.) and build them using Maven:
   ``bash
   mvn clean install
   ```
3. **Start the Infrastructure Services**:

   se Docker Compose to start the configuration server, Eureka server, and gateway server:
   ``bash
   docker-compose up -d
   ```
4. **Deploy Microservices to Kubernetes**:

   pply the Kubernetes deployment files located in the `k8s` directory:
   ``bash
   kubectl apply -f k8s/
   ```
5. **Set Up Monitoring and Logging**:

   onfigure Prometheus, Grafana, Loki, and Promtail using the provided configuration files in the `monitoring` directory.
6. **Access the Application**:

   he application can be accessed via the API gateway. Ensure that all services are up and running, and use the gateway's endpoint to interact with the microservices.
## Contributing

ontributions are welcome!lease fork the repository and create a pull request with your changes.nsure that your code adheres to the project's coding standards and includes appropriate tests.
## License

his project is licensed under the MIT License.ee the [LICENSE](LICENSE) file for more details.
---

This project was developed as a learning exercise to explore microservices architecture using Spring Boot and associated technologies.*
