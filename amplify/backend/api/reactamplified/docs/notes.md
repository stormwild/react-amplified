# Welcome!
#
# This is an in-browser tool for writing, validating, and testing GraphQL queries.
#
# An example query named "GetPost" might look like:
#
#     query GetPost {
#       singlePost(id: 123) {
#         id
#         title
#       }
#     }
#
# An example mutation named "PutPost" might look like:
#
#     mutation PutPost {
#       putPost(id: 123, title: "Hello, world!") {
#         id
#         title
#       }
#     }
#
# Keyboard shortcuts:
#
#  Prettify Query:  Ctrl+Shift+P (also removes comments)
#       Run Query:  Ctrl+Enter   (or press the play button above)
#   Auto Complete:  Ctrl+Space   (or just start typing)
#

```gql
query getTodo($id:ID!) {
  getTodo(id: $id) {
    id
    name
    description
  }
}
```

variables

```json
{
  "id": 1
}
```

```
mutation createTodo {
  createTodo(input: {
    name: "Build an API"
    description: "Build a serverless API with Amplify and GraphQL"
  }) {
    id
    name
    description
  }
}

query listTodos {
  listTodos {
    items {
      id
      description
      name
    }
  }
}
```