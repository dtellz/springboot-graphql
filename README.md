# Springboot GraphQL service

## Requirements
[Java >= 17](https://www.oracle.com/java/technologies/downloads)
[Maven >= 3.5](https://maven.apache.org/download.cgi)

## Local setup

Run the project

```bash
./mvnw spring-boot:run
```

Navigate to [http://localhost:8080/graphiql](http://localhost:8080/graphiql)

Example query:

```graphql
query bookDetails {
  bookById(id: "book-1") {
    id
    name
    pageCount
    author {
      id
      firstName
      lastName
    }
  }
}
```

## Run tests

Run all test suite

```bash
./mvnw test
```

Run the BookController test

```bash
./mvnw -Dtest=BookControllerTest test
```
