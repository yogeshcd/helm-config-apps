# select base image
# expose port for documentation
# set working directory
# copy necessary files
# install necessary packages
# start the server by cmd

FROM node:14
EXPOSE 1004
WORKDIR /app
COPY . .
RUN npm install
CMD [ "node", "index.js"]