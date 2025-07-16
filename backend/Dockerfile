FROM node:18

# Set working directory
WORKDIR /app
# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install
# Install nodemon globally (optional but recommended)
 RUN npm install -g nodemon
# Copy the .env and source files
COPY . .
# Expose port
EXPOSE 5000
# Start the app
CMD ["nodemon", "app.js"]