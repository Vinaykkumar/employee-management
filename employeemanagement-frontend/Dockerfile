# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory in the container to /app
WORKDIR /app

# Install Node.js and npm
RUN apt-get update && apt-get install -y npm

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install Node.js dependencies
RUN npm install

# Copy the entire application directory into the container
COPY . .

# Expose port 3000 for the Node.js application
EXPOSE 3000

# Specify the command to start the Node.js application
CMD ["npm", "start"]
