# Use an official Node.js runtime as a base image
FROM node:18-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the source code to the container
COPY ./src ./src

# Copy the public directory to the container
COPY ./public ./public

# Expose the port that the app will run on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]

