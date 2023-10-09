# go-graphql
In this repo Iam learning the patterns of GraphQL backend design

# How I Setuped this project :-
1. create a tools pkg and create a tools.go file where I imported the packages that i need to depend on 
    ```go
        //go:build tools

        package tools

        import (
            _ "github.com/99designs/gqlgen"
            _ "github.com/99designs/gqlgen/graphql/introspection"
        )
    ```

2. generate a graphql stuff using this cli command 
    ```cmd
        ➜ go-graphql git:(main) ✗ go run github.com/99designs/gqlgen init
            Creating gqlgen.yml
            Creating graph/schema.graphqls
            Creating server.go
            Generating...

            Exec "go run ./server.go" to start GraphQL server
    ```