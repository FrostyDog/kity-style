# KITY-STYLE

## How to run?

### Client

```
$ cd client
$ npm start
```

### Server
```
$ cd server
$ ./run.sh
```

## Development

Basic queries:

1. Fetching all Todos
```
{
    todos {
        id
        text
        done
        user {
            id
            name
        }
    }
}
```

2. Create New Todo
```
mutation {
    createTodo(input:{text:"Feed Kitty", userId:"1"}) {
        id
        text
        done
        user {
            id
            name
        }
    }
}
```
