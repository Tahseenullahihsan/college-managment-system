# Use node base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the .env and source files
COPY . .

# Expose port
EXPOSE 3000

# Start the app
CMD ["npm", "start"]
