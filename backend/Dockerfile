ARG NODE_VERSION=18.16.0

FROM node:${NODE_VERSION}-alpine

# Create App Directory
# RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 5000

CMD [ "npm", "start" ]