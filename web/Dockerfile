# Stage 1: Build the React app
FROM node:18 as builder
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . ./
RUN npm run build

# Stage 2: Output build artifacts to a shared volume
FROM alpine:3.18
WORKDIR /app
COPY --from=builder /app/build /app/build
