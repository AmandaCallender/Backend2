# cookbook-backend
Secret Family Recipe Cookbook - Backend

Section Contents:
- [/auth/login POST](#authlogin-post)
- [/auth/register POST](#authregister-post)
- [/api/users GET](#users-get)

### /auth/login POST

Expects an object with this format as the request body:
```
{
  "username": "User1",   //string
  "password": "password" //string
}
```

### /auth/register POST

Expects an object with this format as the request body:
```
{
  "username": "User1",   //string
  "password": "password" //string
}
```

### /users GET

Requires an `authorization` header with a JWT.
it  will return an array of objects in this format:
```
[
  {
    "id": 1,
    "username": "Amanda"
  },
  {
    "id": 6,
    "username": "Damian"
  },
  {
    "id": 4,
    "username": "Daniel"
  },
  {
    "id": 5,
    "username": "Mike"
  },
  {
    "id": 3,
    "username": "Shirley"
  },
  {
    "id": 2,
    "username": "Stephanie"
  }
]
```