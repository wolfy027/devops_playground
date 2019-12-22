
#specify base image
FROM node:alpine

WORKDIR /usr/app

#Copy build files
COPY ./package.json ./

#Install some dependencies
RUN npm install

# Copy everything else
COPY ./ ./

#Default Command
CMD ["npm","start"]