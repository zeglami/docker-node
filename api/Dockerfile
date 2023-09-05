# Use the official Node.js 20 image based on Alpine Linux as the base image.
FROM node:20-alpine

# Install the nodemon package globally to enable automatic server restarts during development.
RUN npm install -g nodemon

# Set the working directory inside the container to /app.
WORKDIR /app

# Copy the package.json file from the host machine into the container.
COPY package.json .

# Install the Node.js dependencies defined in package.json.
RUN npm install

# Copy all the application source code and files from the host machine into the container.
COPY . .

# Expose port 4000 to allow incoming connections to the application.
EXPOSE 4000

# Define the default command to run when the container starts.
# In this case, it runs 'npm run dev', which typically starts a development server.
CMD ["npm", "run", "dev"]
