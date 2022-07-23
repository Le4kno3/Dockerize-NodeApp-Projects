### Dockerize React Sample "Create React App" for Production environment

### To Start the docker container.

`docker-compose up`

### Note:

1. Make sure you stop all previous running docker containers before running a new docker command.
2. Make sure that "node_modules" are not present in your current working directory when you run docker compose, this will reduce the running time of the application.

### Successful Results

1. visit `http://localhost:80` and check if the react node application is launched successfully.

2. Local changes will not be reflected in the docker container. For any modifications to this docker source files, you need build the docker again `docker-compose up`.
