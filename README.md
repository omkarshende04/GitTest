#Application Name
URL Shortener

#Description
URL Shortener is a web service that allows users to generate short, shareable URLs that redirect to long, complex URLs. Built with Java Spring Boot, the service supports basic URL shortening functionality along with features such as custom URL aliases and click tracking.


#Table of Contents
1.Installation
2.Usage
3.API Endpoints
4.Configuration
5.Running Tests
6.Contributing
7.License
8.Contact
9.Acknowledgments
---------------------------------------------------------------------------------------------------------------------------------------------------------

1.Installation
#Prerequisites
Before you begin, ensure you have the following installed:

Java 17 or higher
Maven 3.6 or higher
Git (for cloning the repository)

#steps
	A.Clone the repository: https://github.com/omkarshende04/UrlShortnerServices.git
	B.Build the project: mvn clean install
	c.Run the application: mvn spring-boot:run
	d.The application will start on http://localhost:8080.
---------------------------------------------------------------------------------------------------------------------------------------------------------

2. Usage
Once the application is running, you can use the following endpoints to interact with the URL Shortener service.
---------------------------------------------------------------------------------------------------------------------------------------------------------

3.API Endpoints

1. Shorten a URL
Endpoint: GET http://localhost:8080/getShortenUrl
Description: Generates a short URL for the given long URL.
Request Body:
{
    "originalurl" : "https://www.youtube.com/watch?v=BJAWM7KfswM"
}
Response:
localhost:8080/LOu0Zw3i

2. Redirect to Original URL
Endpoint: GET /{shortUrl}
Description: Redirects the user to the original long URL associated with the short URL.
Example:
Navigate to localhost:8080/LOu0Zw3i, and it will redirect to https://www.youtube.com/watch?v=BJAWM7KfswM.

3. Get Metrics Data
Endpoint: http://localhost:8080/getMetrics
Description: Get Mostly hit url data
Request Body:
NA
Response:
{
    "chatgpt.com": 3,
    "www.youtube.com": 2,
    "app.flowcv.com": 1
}
---------------------------------------------------------------------------------------------------------------------------------------------------------

4.Configuration

Application Properties
You can customize the application by editing the application.properties file:
server Port: Change the default port (8080): server.port=8081

Database Configuration:
spring.datasource.url=jdbc:h2:mem:urlshortnerDb;DB_CLOSE_DELAY=-1
spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.username=urlshortner
spring.datasource.password=urlshortner
spring.h2.console.enabled=true
---------------------------------------------------------------------------------------------------------------------------------------------------------

5.Running Tests
To run the unit tests for the project, use the following command: mvn test
You can find the test reports in the target/surefire-reports directory after running the tests.
---------------------------------------------------------------------------------------------------------------------------------------------------------

6.Contributing:
We welcome contributions to the URL Shortener project! To contribute, please follow these steps:
Fork the repository - clone it - create new branch - make changes and commit - Push
---------------------------------------------------------------------------------------------------------------------------------------------------------

7.License
NA
---------------------------------------------------------------------------------------------------------------------------------------------------------

8.Contact
For any questions or issues, please contact:

Name - omkar.shende04@gmail.com
username- https://github.com/omkarshende04 
---------------------------------------------------------------------------------------------------------------------------------------------------------

9.Acknowledgments
Thanks All Developers! You all are amazing 
---------------------------------------------------------------------------------------------------------------------------------------------------------