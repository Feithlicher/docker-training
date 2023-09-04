# Specify a base image
FROM node:14-alpine

WORKDIR /usr/app

# Install some dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Default command
CMD ["npm", "start"]


# How to build?: docker build -t feithlicher/simpleweb .
# How to run?: docker run -p 8080:8080 feithlicher/simpleweb
# Start a shell inside a contrainer: docker run -it feithlicher/simpleweb sh
# How to see all containers?: docker ps
# run a shell inside a container: docker exec -it eac3ae7a2c3e sh