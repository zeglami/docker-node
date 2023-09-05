# Use the official Node.js 20 image based on Alpine Linux as the base image.
FROM node:20-alpine

# Set the working directory inside the container to /app.
WORKDIR /app

# Copy the package.json file from the host machine into the container.
COPY package.json .

# Install the Node.js dependencies defined in package.json.
RUN npm install

# Copy all the application source code and files from the host machine into the container.
COPY . .

# Expose port 3000 to allow incoming connections to the application.
# required for Docker Desktop port mapping
EXPOSE 3000
# Define the default command to run when the container starts.
# In this case, it runs 'npm start', which is typically the command to start the application.
CMD ["npm", "start"]
