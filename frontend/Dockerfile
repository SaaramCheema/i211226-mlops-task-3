# Use Node.js as the base image
FROM node:18

WORKDIR /app

COPY package.json package-lock.json ./
RUN npm install

COPY . .

# Enable hot reload
CMD ["npm", "start"]

EXPOSE 3000
