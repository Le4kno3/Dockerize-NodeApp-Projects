### Dockerize React Sample "Create React App"

### To Start the docker container.

`docker-compose -f docker-compose-development.yml up`

### Note:

1. Make sure you stop all previous running docker containers before running a new docker command.
2. Make sure that "node_modules" are not present in your current working directory when you run docker compose, this will reduce the running time of the application.

### Successful Results

visit `http://localhost:4500` and check if the react node application is launched successfully.
