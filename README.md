# SPRING BOOT CQRS AND EVENT SOURCING FOR BANK ACCOUNTS (QUERY AND COMMMANDS) - Core Module

This a small CQRS and event sourcing example without Frameworks, developed using KAFKA (Topic-based) and the CQRS 
(Command Query Resposability Segregation) which is an approach to design Microservices nowadays. It consists of an CORE MODULE (for sharing 
some interfaces and utilities, ACCOUNTS COMMANDS Microservice (Creates the user accounts by using the MEDIATOR PATTERN to find the 
correct handler for each command), this ACCOUNS COMMANDS Microservice support several operations. Finally there is the QUERIES 
Microservice (Queries the accounts in different ways) which supports several operations over the user accounts BUT ONLY NON-MODIFYING
ones. It was developed by Luis Espinosa Llanos and it was used the following technologies and tools: 

<table style="width:100%">
  <tr>
    <td>
  	Core	
    </td>
    <td>
  	Java 16, Spring Boot 2, Data JPA, Hibernate, Loombok, Axon (Event store), Spring Cloud.
    </td>
  </tr>
  <tr>
    <td>
  	Design Patterns	
    </td>
    <td>
  	CQRS, Event Sourcing, Mediator pattern, liskov substitution principle.
    </td>
  </tr>
  <tr>
    <td>
  	Architectural Styles
    </td>
    <td>
  	MicroServices and RESTful
    </td>
  </tr>
  <tr>
    <td>
  	Database	
    </td>
    <td>
  	MongoDB (EventStore - Writing database), MySQL (Read database)
    </td>
  </tr>
  <tr>
    <td>
  	Server	
    </td>
    <td>
  	Apache Tomcat Embebido (Spring Boot)
    </td>
  </tr>
  <tr>
    <td>
  	Virtualization	
    </td>
    <td>
  	Docker, Docker-compose.
    </td>
  </tr>
  <tr>
    <td>
  	IDE	
    </td>
    <td>
  	Intellij IDE Ultimate
    </td>
  </tr>
  <tr>
    <td>
  	Executable	
    </td>
    <td>
  	Jar
    </td>
  </tr>
</table>


## Video
A video exposing the functionality of the proyect in local environment on a Desktop screen.

1. https://youtu.be/OjjqbaS2wQ0 (BASIC EXPLANATION)
2. https://youtu.be/DCDLv8HNQEc (WITH DOCKER COMPOSE DEPLOYMENT)

## Pictures
Some pictures of the project on a local environment respectively:

<table style="width:100%">
  <tr>
    <td>
  		<img width="450" alt="Image" src="https://user-images.githubusercontent.com/56041525/171011101-5653746e-ccde-4637-9b9e-74ea63ab9886.PNG">
	  </td>
    <td>
  	<img width="450" alt="Image" src="https://user-images.githubusercontent.com/56041525/171011153-7983ba0e-3d93-423d-80ee-7dbe2ad67578.PNG">
    </td>
  </tr>
</table>

<table style="width:100%">
  <tr>
    <td>
  		<img width="450" alt="Image" src="https://user-images.githubusercontent.com/56041525/171027655-1b87305e-bb7d-4ab4-9834-a11c8a40409d.png">
	  </td>
</table>

## Installation

Each proyect should be installed using the following command:
```bash
mvn clean install
```

## Usage
In the target folder you will find the Jar archive, of course the configuration for Login purposes was externalized, this is to say that
arguments have to be passed through command line, so please use the following command according to your values:

```bash
java -jar EACH_PROJECT.jar
```

## Contributing
This proyect is quite simple, and is part of my personal portfolio, so it is not intended to receive contributions.


## License
It is free.
