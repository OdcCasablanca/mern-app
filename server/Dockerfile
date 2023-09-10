# Use the official Node.js LTS image as the base image
FROM node:16

# Set the working directory inside the container
WORKDIR /app/server

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install backend dependencies
RUN npm install

# Copy the rest of the backend source code to the container
COPY . .

# Expose the port the Node.js app runs on
EXPOSE 8081

# Start the Node.js app
CMD ["npm", "start"]
