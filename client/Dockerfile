# Use the official Node.js LTS image as the base image
FROM node:16

# Set the working directory inside the container
WORKDIR /app/client

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy the rest of the frontend source code to the container
COPY . .


# Expose the port the React app runs on
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]
