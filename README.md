# Springboot GraphQL service

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
