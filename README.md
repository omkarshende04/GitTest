
# URL Shortener

URL Shortener is a web service that allows users to generate short, shareable URLs that redirect to long, complex URLs. Built with Java Spring Boot, the service supports basic URL shortening functionality.



## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [API Endpoints](#api-endpoints)
4. [Configuration](#configuration)
5. [Running Tests](#running-tests)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)
9. [Acknowledgments](#acknowledgments)



## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [API Endpoints](#api-endpoints)
4. [Configuration](#configuration)
5. [Running Tests](#running-tests)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)
9. [Acknowledgments](#acknowledgments)



## Installation

### Prerequisites

Before you begin, ensure you have the following installed:

- **Java 17** or higher
- **Maven 3.6** or higher
- **Git** (for cloning the repository)

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/omkarshende04/UrlShortnerServices.git

2. **Build the project:**
    ```Maven
    mvn clean install

3. **Run the application:**
    ```Maven
    mvn spring-boot:run

4. **Access the application:**   
The application will start on http://localhost:8080.
    
## Usage

Once the application is running, you can use the following endpoints to interact with the URL Shortener service:
## 3. API Endpoints

### 1. Shorten a URL

- **Endpoint:** `GET http://localhost:8080/getShortenUrl`
- **Description:** Generates a short URL for the given long URL.
- **Request Body:**
  ```json
  {
      "originalurl": "https://www.youtube.com/watch?v=BJAWM7KfswM"
  }
- **Response:**
    
    http://localhost:8080/LOu0Zw3i


### 2. Redirect to Original URL
- **Endpoint:** `GET /{shortUrl}`
- **Description:** Redirects the user to the original long URL associated with the short URL.
- **Example:** Navigate to http://localhost:8080/LOu0Zw3i, and it will redirect to https://www.youtube.com/watch?v=BJAWM7KfswM.


### 1. Get Metrics Data

- **Endpoint:** `GET http://localhost:8080/getMetrics`
- **Description:** Retrieves data on the most frequently hit URLs.
- **Request Body:** N/A

- **Response:**
    ```json
  {
    "oracle.com": 3,
    "www.youtube.com": 2,
    "facebook.com": 1
  }

## 4. Configuration

You can customize the application by editing the `application.properties` file:

### Application Properties

- **Server Port:** Change the default port (8080) by setting:
  ```properties
  server.port=8081

- **Database Configuration:** Configure the database with the following properties:
    ```properties
    spring.datasource.url=jdbc:h2:mem:urlshortnerDb;DB_CLOSE_DELAY=-1
    spring.datasource.driver-class-name=org.h2.Driver
    spring.datasource.username=urlshortner
    spring.datasource.password=urlshortner
    spring.h2.console.enabled=true
## 5. Running Tests

- To run the unit tests for the project, use the following command:

   ```bash
     mvn test

- After running the tests, you can find the test reports in the target/surefire-reports directory.
## 6. Contribution

We welcome contributions to the URL Shortener project! To contribute, please follow these steps:

- *Fork the repository*
- *Clone the repository*
- *Create a new branch*
- *Make changes and commit*
- *git add .*
- *git commit -m""*
- *git push origin your-branch-name*

## 7. License

This project does not have a specified license. Please check the repository or contact the maintainers for more information.
## 8. Contact

For any questions or issues, please contact:

- **Name:** Omkar Shende
- **Email:** [omkar.shende04@gmail.com](mailto:omkar.shende04@gmail.com)
- **GitHub:** [https://github.com/omkarshende04](https://github.com/omkarshende04) 
 ## 9. Acknowledgments

Thanks to all developers! You all are amazing!
