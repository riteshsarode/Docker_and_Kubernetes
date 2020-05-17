# specify base image
FROM node:alpine

# Add working direcotry
WORKDIR /usr/app

# Install dependencies
COPY ./ ./
RUN npm install

# setup default command
CMD [ "npm", "start"]