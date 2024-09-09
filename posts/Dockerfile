#1. use an official Node.js runtime as a parent image
FROM node:alpine
#2. set the working directory in the container
WORKDIR /app
#3.copy package.json file to the working directory
COPY package.json ./
#4.install any dependencies
RUN npm install
#5.copy the rest of the application code to the working directory
COPY ./ ./
#6.start tha application using the npm start script defined in package.json
CMD ["npm","start"]