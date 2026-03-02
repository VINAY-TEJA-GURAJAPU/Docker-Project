# Lightweight Node base image
FROM node:18-alpine

# Create app directory
WORKDIR /app

# Copy dependency files first (for better caching)
COPY package*.json ./

# Install only production dependencies
RUN npm install --omit=dev

# Copy application source code
COPY . .

# Create non-root user for security
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

# Switch to non-root user
USER appuser

# Expose backend port
EXPOSE 5000

# Start application
CMD ["npm", "start"]