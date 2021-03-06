
# Alankar Apte

# Implemented
PostgreSQL 
Swagger2 with UI

# Objective
This project demonstrate the use of JSON with spring-boot + PostgreSQL
We are storing JSON record in DB
We have used Swagger2 to documents APIs

# Reference: 
JSON usage - https://vladmihalcea.com/how-to-map-json-objects-using-generic-hibernate-types/

Swagger - https://dzone.com/articles/spring-boot-restful-api-documentation-with-swagger

### To make use of the JSON Hibernate Types, we must declare them using the @TypeDef annotation:
@TypeDefs({
    @TypeDef(name = "json", typeClass = JsonStringType.class),
    @TypeDef(name = "jsonb", typeClass = JsonBinaryType.class)
})

### MySQL 5.7 adds support for JSON types, which, at the JDBC level, need to be materialized as String. For this reason, we are going to use JsonStringType.
    @Type(type = "json")
    @Column(columnDefinition = "json")
    private Location location;


### For the JSON column type, the two JSON Object(s) mapping must be changed as follows
    @Type(type = "jsonb")
    @Column(columnDefinition = "json")
    private Location location;
    
OR

    @Type(type = "jsonb")
    @Column(columnDefinition = "jsonb")
    private Location location;


---

---



# Read Me First
The following was discovered as part of building this project:

* The original package name 'com.alankar.springboot-json-column-example' is invalid and this project uses 'com.alankar.springbootjsoncolumnexample' instead.

# Getting Started

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.4.2/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.4.2/maven-plugin/reference/html/#build-image)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/2.4.2/reference/htmlsingle/#using-boot-devtools)
* [Liquibase Migration](https://docs.spring.io/spring-boot/docs/2.4.2/reference/htmlsingle/#howto-execute-liquibase-database-migrations-on-startup)
* [Spring Data JPA](https://docs.spring.io/spring-boot/docs/2.4.2/reference/htmlsingle/#boot-features-jpa-and-spring-data)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.4.2/reference/htmlsingle/#boot-features-developing-web-applications)

### Guides
The following guides illustrate how to use some features concretely:

* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)

