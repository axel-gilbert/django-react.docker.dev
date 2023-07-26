# Base image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./

RUN npm install

# Bundle app source
COPY . .

# Expose the port the app runs in
EXPOSE 8080

# Serve the app
CMD [ "npm", "start" ]
