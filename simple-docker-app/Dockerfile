# set base image with version
FROM node:16

# set working directory in container 
WORKDIR /

# copy package.jon to root. In this case, dot is equal to container working directy which is set to /
# COPY package.json /
COPY package*.json ./

# install dependencies
RUN npm install

# left dot points to this local direcotry and dot on right points to the container root direcotry /
COPY . .

# expose container port
EXPOSE 3000

CMD [ "node", "server.mjs" ]
