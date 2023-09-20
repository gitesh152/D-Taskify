ARG NODE_VERSION=18.16.0

FROM node:${NODE_VERSION}-alpine

WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

CMD [ "npm", "start" ]