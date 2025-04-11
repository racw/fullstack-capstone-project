# Update to Node.js 18 which supports node: imports
FROM node:18.12.1-slim

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json files
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy application code
COPY . .

# Expose port (if needed)
EXPOSE 9000

# Run the application
CMD ["node", "index.js"]