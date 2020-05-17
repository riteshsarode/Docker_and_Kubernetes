# Use an existing docker image as a base
FROM alpine

#Download and install dependency
RUN apk add --update redis



# What to do whenit starts as a container
CMD ["redis-server"]
