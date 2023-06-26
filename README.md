# Formula1 API system
A demo restful API 


# Setup

### With Docker

- Open docker-compose.yml file
- Replace default environment config
- Run command
  ```
  docker compose up -d
  ```
- Access url http://localhost:3000/swagger

**Note**
replace 3000 with port at config step when access url


## Authorization

Project is pre-setup with demo Firebase project, use this command to get jwt token for testing

```shell
curl 'https://identitytoolkit.googleapis.com/v1/accounts:signInWithPassword?key=AIzaSyApLhjABcBUj5NjQb-witpumRhUgT11jWY' \
-H 'Content-Type: application/json' \
--data-binary '{"email":"demo1@formula1.demo","password":"123456","returnSecureToken":true}'
```

**Note**

This configuration might not work due to remove project, config another Firebase project replace configs above cli and in file ***src/bootstrap/firebase.ts***