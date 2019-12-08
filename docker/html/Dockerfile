# Test web-app to use with Pluralsight courses and Docker Deep Dive book
# Linux x64
FROM alpine

# Install Node and NPM
RUN apk add --update nodejs nodejs-npm

RUN npm install -g http-server

# Copy app to /src
COPY . /src

WORKDIR /src

EXPOSE 8080

ENTRYPOINT ["http-server", "-p", "8080"]
