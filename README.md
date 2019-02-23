# MicroserviceExampleProject

This is a example project on microservices from JavaBrains implemented with Spring Boot.

Multiple microservices are communicating with each other using RestTemplate and WebClient with service discovery.
Created Eureka Server and had all these microservices register as Eureka Clients by adding them to the classpath.
Used LoadBalanced on RestTemplate to leverage eureka server with very minimal code changes.
Able to get all this functionality by having client side load balancing


'rating-data-service' and 'movie-info-service' - These two microservices are providing some data. The third microservice 'movie-catalog-service' calls those two, gets the data, consolidates the data and sends back a response

Output was fetched from  "http://localhost:8081/catalog/anyThing".
