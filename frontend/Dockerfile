FROM node:alpine as builder
# working directory
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build
# block 1 ends here

# host using nginx
FROM nginx
COPY --from=builder /app/build /usr/share/nginx/html




