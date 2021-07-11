# KITY-STYLE

## Installation

1. Install NodeJS
2. Install Golang
3. Install dependencies

```
$ cd client
$ npm i

$ cd server
$ go get
```

## Running

**Client**
```
$ cd client
$ npm start
```
Access your app with localhost:3000

**Server**
```
$ cd server
$ ./run.sh
```
Access GraphQL Playground on localhost:8080

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
```

## Known problems

**Problem:** GraphQL Playground: __mode Graphql unable to change stream__
**Solution:** Clear Localstorage
