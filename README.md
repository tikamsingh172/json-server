# ✨How to Create json-server
---
### Step:1
Create a folder:- `db`

### Step:2
`npm install json-server`

### Step:3
Create a `db/db.json` file with data-
```json
{
  "users": [
    {
      "id": "1",
      "name": "Tikam singh",
      "email": "tikamsingh172@gmail.com",
      "password": "tikam12345",
      "mobile": 8077662051
    },
    {
      "id": "2",
      "name": "vishal-verma",
      "email": "vishal-verma@gmail.com",
      "password": "vishal-verma12345"
    },
    {
      "id": "3",
      "name": "ajay",
      "email": "ajay@gmail.com",
      "password": "ajay12345"
    }
  ],
  "products": [
    {
     "id": "1",
     "name": "mobile",
     "color": "black",
     "price": "5000 Rs/",
    },
    {
     "id": "2",
     "name": "laptop",
     "color": "red",
     "price": "80000 Rs/",
    }
  ]
}
```

### Step:4
> **start json-server with default port: 3000**
>
>`npx json-server db.json`

> **start json-server with custom port: 5000**
>
>`npx json-server db.json --port 5000`

#### Show all options:-
`npx json-server --help`

### Routes
Based on the example `db.json`, you'll get the following routes:

```
GET    /users
GET    /users/:id
POST   /users
PUT    /users/:id
PATCH  /users/:id
DELETE /users/:id

# Same for products
```

### Get more info:-
>[https://github.com/typicode/json-server](https://github.com/typicode/json-server)
>
>(or)
>
>[https://www.npmjs.com/package/json-server](https://www.npmjs.com/package/json-server)