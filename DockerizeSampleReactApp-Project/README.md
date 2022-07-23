### Dockerize React Sample "Create React App"

### To Start the docker container.

`docker-compose -f docker-compose-development.yml up`

### Note:

1. Make sure you stop all previous running docker containers before running a new docker command.
2. Make sure that "node_modules" are not present in your current working directory when you run docker compose, this will reduce the running time of the application.

### Successful Results

1. visit `http://localhost:4500` and check if the react node application is launched successfully.

2. Because we are using docker-compose to run the docker container, and also mapped our local directories with the docker file system, as a result, when you edit your local source code, it get automatically reflected inside the docker. (Although you need to refresh the browser, it will not automatically refresh)
