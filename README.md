# Size Service for E-commerce Application

This project is a Size Service for an e-commerce clothing application. The Size Service is designed to manage clothing sizes, allowing other microservices within the platform to effectively interact with size data. By centralizing size management, it ensures consistency and accuracy in the representation of clothing sizes across the e-commerce platform.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Service](#running-the-service)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Size Service is a RESTful API built using Spring Boot. It provides endpoints for creating, updating, retrieving, and deleting clothing sizes. This service plays a crucial role in the product management system by ensuring that size data is uniformly managed and easily accessible to other microservices.

## Features

- **Create Sizes:** Allows the creation of new clothing sizes with detailed descriptions.
- **Retrieve Sizes:** Enables fetching details of existing sizes, supporting features like product filtering and search.

## Prerequisites

- Java 17 or higher
- Maven 3.6.3 or higher
- Spring Boot 3 or higher

## Installation

1. Clone the repository:

    - ```sh
      git clone https://github.com/Agustin199811/size-service.git
      cd size-service
      ```

2. Build the project using Maven:

    - ```sh
      mvn clean install
      ```

## Configuration

The configuration for the Size Service is located in `src/main/resources/application.properties`. Below is an example configuration:

```properties
spring.datasource.url=jdbc:mariadb://clot-mariadb.cp88o8squjfi.us-east-1.rds.amazonaws.com:3306/clot
spring.datasource.username=root
spring.datasource.password=root1234

eureka.client.service-url.defaultZone=http://clot-ecommerce-ELB-1792240696.us-east-1.elb.amazonaws.com:8761/eureka/
eureka.client.register-with-eureka=true
eureka.client.fetch-registry=true
```

## Running the Service

To run the service registry, use the following command:

 ```sh
    mvn spring-boot:run
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please send us an email at
`toapantaagustin9c@gmail.com` with details about your proposed changes or improvements. We look forward to hearing from you!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
