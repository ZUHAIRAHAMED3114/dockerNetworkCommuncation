# Use an official Node.js image as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the app dependencies
RUN npm install

# Copy the application code to the container
COPY . .

# Build the React app
RUN npm run build

# Expose the port on which the app will run (adjust as needed)
EXPOSE 3000

# Define the command to run your app
CMD ["npm", "start"]
