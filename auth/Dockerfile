FROM node:alpine

# Create non-root user
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

WORKDIR /app

# Copy only dependency files first (better caching)
COPY package.json yarn.lock ./

# Install dependencies (production only, lockfile respected)
RUN yarn install --frozen-lockfile --production

# Copy the rest of the app
COPY . .

# Change ownership so non-root user can access
RUN chown -R appuser:appgroup /app
USER appuser

CMD ["yarn", "start"]
