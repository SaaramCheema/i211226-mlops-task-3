# Use Node.js as the base image
FROM node:18

WORKDIR /app

COPY package.json package-lock.json ./
RUN npm install

COPY . .

# Enable watch mode with Nodemon
RUN npm install -g nodemon
CMD ["nodemon", "src/server.js"]

EXPOSE 5000
