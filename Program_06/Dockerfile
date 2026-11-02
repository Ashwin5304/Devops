# Use the official Node.js 20 Alpine image
FROM node:20-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install all required Node.js dependencies
RUN npm install

# Copy all application files into the container
COPY . .

# Expose port 3000 for the application
EXPOSE 3000

# Start the Node.js application
CMD ["node", "app.js"]
