FROM node:alpine

# /app is where my node application source code will reside,
# this means "." will always point to "/app" from now on.
WORKDIR '/app'

# copy package.json to my "/app" directory
COPY --chown=node:node package.json .

# setting permissions
RUN chown -R node:node /app/

# download all dependencies
RUN npm install

# copy all files from local environment to docker
# the first "." is for local file system, the second "." is for docker file system
COPY . .

# set the user
USER node

# on the "/app" run "npm run build"
RUN npm run build

# 
FROM nginx
COPY --from=0 /app/build /usr/share/nginx/html

