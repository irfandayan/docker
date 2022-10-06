# set base image with version
FROM node:14

# set working directory in container 
WORKDIR /app

# copy package.jon to root. In this case, dot is equal to container working directy which is set to /app
# COPY package.json /app 
COPY package.json .

# install dependencies
RUN npm install

# left dot points to this local direcotry and dot on right points to the container root direcotry /app
COPY . . 

EXPOSE 80

# anonymous volume
# it does not persists data so use named volumes in run command
#VOLUME [ "/app/feedback" ]
#VOLUME ["/app/node_modules"]

CMD ["npm", "start"]