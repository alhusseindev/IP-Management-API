# IP Address Management REST API
An IP Address Management REST API on top of an H2 data store. It has the ability to add IP Addresses by CIDR block and then either acquire or release IP addresses individually. Each IP address will have a status associated with it that is either “available” or “acquired”.

## The REST API supports four endpoints:

* Create IP addresses - take in a CIDR block (e.g. 10.0.0.1/24) and add all IP addresses within that block to the data store with status “available”
* List IP addresses - return all IP addresses in the system with their current status
* Acquire an IP - set the status of a certain IP to “acquired”
* Release an IP - set the status of a certain IP to “available”


## Technologies that I used:
* Java
* Spring
* Spring Boot
* Spring Data
* JPA (Java Persistence API)
* JUnit
* Spring Boot Testing
* H2 Database
* Docker


### Docker Image
I pushed the the Docker image to Docker Hub, it can be accessed from here:

https://hub.docker.com/repository/docker/082497/ip-management-container

