# Use an official Node.js runtime as a base image
FROM --platform=linux/amd64 node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the application code to the container
COPY . .

# Expose the port on which your Node.js app will run
ENV PORT 80
EXPOSE 80

# Define the command to run your application
CMD ["node", "server.js"]
