FROM node:boron

#MAINTAINER Ivan Font <ifont@redhat.com>
MAINTAINER Lacoste <git@delfosse.com>

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Clone game source code
RUN git clone https://github.com/lac0ste-oss/pacman.git .

# Install app dependencies
RUN npm install

# Expose port 8080
EXPOSE 8080

# Run container
CMD ["npm", "start"]
