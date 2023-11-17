<div align=center>
   
 # 🌺 Java API

RESTful API from DIO's BackEnd JAVA bootcamp. built in Java 17 with Spring Boot 3.

</div>

## Main Technologies
  - **Java 17**: We will use the latest LTS version of Java to take advantage of the latest innovations that this robust and widely used language offers;
  - **Spring Boot 3**: We will work with the newest version of Spring Boot, which maximizes developer productivity through its powerful self-configuration premise;
  - **Spring Data JPA**: We will explore how this tool can simplify our data access layer, facilitating integration with SQL databases;
  - **OpenAPI (Swagger)**: We will create effective and easy-to-understand API documentation using OpenAPI (Swagger), perfectly aligned with the high productivity that Spring Boot offers;
  - **Railway**: facilitates the deployment and monitoring of our solutions in the cloud, in addition to offering several databases as a service and CI/CD pipelines.

## Preview Figma
- [FIGMA](https://www.figma.com/file/0ZsjwjsYlYd3timxqMWlbj/SANTANDER---Projeto-Web%2FMobile?type=design&node-id=1421%3A432&mode=design&t=6dPQuerScEQH0zAn-1)

Figma was used to abstract the domain of this API, being useful in the analysis and design of the solution.

## Class Diagram (API Domain)

```mermaid
classDiagram
   class User {
     -String name
     -Account account
     -Feature[] features
     -Card card
     -News[] news
   }

   class Account {
     -String number
     -String agency
     -Number balance
     -Number limit
   }

   classFeature {
     -String icon
     -String description
   }

   class Card {
     -String number
     -Number limit
   }

   class News {
     -String icon
     -String description
   }

   User "1" *-- "1" Account
   User "1" *-- "N" Feature
   User "1" *-- "1" Card
   User "1" *-- "N" News
```

## API Documentation (Swagger)

### [https://sdw-2023-prd.up.railway.app/swagger-ui.html](https://sdw-2023-prd.up.railway.app/swagger-ui.html)

This API will be available on Railway for a limited period of time, but this is open source. Therefore, feel free to clone it, modify it (as it is a good base project for new projects) and run it locally or wherever you find most interesting! Just don’t forget to tag us when you share your solution 🥰

</div>
