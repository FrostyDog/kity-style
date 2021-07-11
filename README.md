# KITY-STYLE

## Installation

## Preflight Check

[] NodeJS
[] Go lang

### Client

```
$ cd client
$ npm i
```

### Server

```
$ cd server
$ go get
```

## Running

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

**Fetching all Todos**
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

**Create New Todo**
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
