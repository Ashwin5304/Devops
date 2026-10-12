
# Use Node.js version 22 with Alpine Linux
FROM node:22-alpine

# Set the working directory 
WORKDIR /app

# Copy package.json and package-lock.json 
COPY package*.json ./

# Install the  dependencies
RUN npm install

# Copy the application file 
COPY app.js .

# Expose port 3000 for the application
EXPOSE 3000

# Start 
CMD ["node", "app.js"]
