# set base image with version
FROM node:14

# set working directory in container 
WORKDIR /app

# copy package.jon to root. In this case, dot is equal to container working directy which is set to /app
# COPY package.json /app
COPY package*.json ./

# install dependencies
RUN npm install

# left dot points to this local direcotry and dot on right points to the container root direcotry /
COPY . ./app

# expose container port
EXPOSE 80

CMD [ "node", "server.js" ]
