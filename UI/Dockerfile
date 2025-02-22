# Use Node.js as the build environment
FROM node:18 as build

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json for dependency installation
COPY your-folder-name/package*.json ./

# Install dependencies
RUN npm install

# Copy the entire Angular project
COPY your-folder-name .

# Build the Angular app
RUN npm run build --prod
