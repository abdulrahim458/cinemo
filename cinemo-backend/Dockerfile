FROM node:16

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package.json app.js ./

RUN npm install

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "node", "app.js" ]
