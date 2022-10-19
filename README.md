# my_react
Building REST API with Express and authenticate by Passport with express-jwt strategy.

You can now access to `/cat/public` api.

To login and get JWT token:
```sh
curl --location --request POST 'http://localhost:3003/user/login' --header 'Content-Type: application/json' --data-raw '{"username": "codering", "password": "code"}'
```
To call secured api:
```sh
curl --location --request GET 'http://localhost:3003/code/private' --header 'Authorization: Bearer <jwt-token-from-login-api>'
``` 
