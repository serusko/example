# Use Node.js image as base
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the React app using Vite
RUN npm run build

# Serve the built files using a static server
# Use a lightweight server like serve or an HTTP server
RUN npm install -g serve

# Expose the HTTP port
EXPOSE 3000

# Start the server
CMD ["serve", "-s", "dist"]