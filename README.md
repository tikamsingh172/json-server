# ✨How to Create json-server

## **`Quick Start`**

### Step:1

Create a folder:- `db`

### Step:2

> **In this folder, you run:**
>
>`npm install json-server`

### Step:3

Create a `db/db.json` file with data-

```json
{
  "users": [
    {
      "id": "1",
      "name": "Tikam singh",
      "email": "tikam172@gmail.com",
      "password": "tikam12345",
      "mobile": 8077682050
    },
    {
      "id": "2",
      "name": "Vishal Verma",
      "email": "verma@gmail.com",
      "password":"vishal12345"
      "mobile": 8077682050
    },
    {
      "id": "3",
      "name": "Ajay",
      "email": "ajay@gmail.com",
      "password": "ajay12345"
      "mobile": 8077682050
    }
  ],
  "products": [
    {
     "id": "1",
     "name": "Mobile",
     "color": "Black",
     "price": "25000 Rs/",
    },
    {
     "id": "2",
     "name": "Laptop",
     "color": "Red",
     "price": "80000 Rs/",
    }
  ]
}
```

### Step:4

> **start json-server with default port: 3000**
>`npx json-server db.json`
>
> **start json-server with custom port: 5000**
>`npx json-server db.json --port 5000`

#### Show all options:-

`npx json-server --help`

### Routes

Based on the example `db.json`, you'll get the following routes:

```javascript
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
