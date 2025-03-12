# Use Node.js for development
FROM node:20
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the frontend port
EXPOSE 5173

# Start the app in development mode with hot reload
CMD ["npm", "run", "dev"]
