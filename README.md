# microservices-with-spring-cloud
A set of simple microservices built with Spring cloud

## Running with Docker

- Go to the naming-server directory and run the following commands
	- mvn clean package
	- docker build -t naming:latest .
- Go to the forex directory and run the following commands
	- mvn clean package
	- docker build -t forex:latest .
- Go to the currencyconversion directory and run the following commands
	- mvn clean package
	- docker build -t currencycon:latest .
- Go to the root directory and run the following commands
	- docker swarm init
	- docker-compose stack deploy -c docker-compose.yaml microservices

Visit the eureka server at http://localhost:8761
