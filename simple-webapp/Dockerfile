# specify base image
FROM node:alpine

# Add working direcotry
WORKDIR /usr/app

# Install dependencies
COPY ./package.json ./
RUN npm install

# To avoid invalidating cache on small changes to source code. Package.json will avoid building npm container on every change
COPY ./ ./

# setup default command
CMD [ "npm", "start"]