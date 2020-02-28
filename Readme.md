# Excel Account Service

Excel Account Service is for providing Authentication and to manage user account for different services in Excel Platform.

It has two sub modules

  - See [Excel-Accounts-Frontend](https://gitlab.com/excel-mec/Excel-Accounts-Frontend/)
  - See [Excel-Accounts-Backend](https://gitlab.com/excel-mec/Excel-Accounts-Frontend/)

# Setting up Development Environment

#### Requirements:
  - You must have [docker](https://docker.com/) installed to run the application
  - To install docker follow this [documentation](https://docker.com/)


#### Cloning the repository:
  Direct contribution to the repository is not allowed. So you must first fork the repository and then to clone the repository with the submodules, do:
  ```sh
$ git clone --recurse-submodules -j8 https://gitlab.com/<YourUsername>/Excel-Account-Service.git
```

#### Running the Application:
To run the Application, make sure no processes are running in the following ports in localhost,
  - :80
  - :5000
  - :3000
  - :5432
 
Then build and run the following commands at the root of the repository
##### Build:
  ```sh
$ docker-compose build
```
##### Run:
  ```sh
$ docker-compose up
```

##### Run in background:
  ```sh
$ docker-compose up -d
```

Verify the application is running by visiting following route in the browser.
```sh
http://localhost
```

You can verify the individual services by visiting the routes
```sh
http://localhost:3000  (Frontend)
http://localhost:5000  (Backend)
```

# Stoping the Application
If you started the application by running the command `docker-compose up` press `Ctrl+c` on windows or `Cmd+c` on mac to stop. If the application is running in background, stop it by running,

```sh
$ docker-compose stop
```

##### To bring all the containers down:
```sh
$ docker-compose down
```

# Documentation
#### Api Documentation
The backend api documentation is automatically generated using swagger, you can view it by navigating to the route,
```sh
http://localhost/api/swagger
```

### Todos

 - Lol lot to do.