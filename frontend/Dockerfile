# Base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Install dependencies
COPY package.json .
RUN npm install

# Copy the rest of the app
COPY . .

# Build the app
RUN npm install

# Expose the port the app runs on
EXPOSE 3000

# Start the app
CMD ["npm", "start"]
