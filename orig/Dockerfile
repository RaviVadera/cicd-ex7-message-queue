# Use latest NodeJS v16.x
FROM node:16
# Indicate that this will be production environment
ENV NODE_ENV=production
# Change CWD to /app
WORKDIR /app
# Copy dependency configuration
COPY ["package.json", "package-lock.json*", "./"]
# Install production dependencies
RUN npm install --omit=dev
# Copy source files
COPY . .
# Expose port for listening
EXPOSE 3000
# Set entrypoint for the image
ENTRYPOINT ["npm", "start"]