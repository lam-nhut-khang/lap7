# Base image
FROM node:18-slim

# Set working directory
WORKDIR /app

# Copy package files và cài dependencies
COPY package*.json ./
RUN npm ci --only=production

# Copy source code
COPY . .

# Expose port của service
EXPOSE 3002

# Lệnh chạy service
CMD ["node", "index.js"]