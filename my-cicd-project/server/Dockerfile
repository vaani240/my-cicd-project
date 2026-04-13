# Use Node.js version 20
FROM node:20-alpine

# Create a folder for the app inside the container
WORKDIR /app

# Copy the "package" files first to install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of your server code
COPY . .

# Tell the container to use port 5000
EXPOSE 5000

# The command to start the server
CMD ["npm", "start"]