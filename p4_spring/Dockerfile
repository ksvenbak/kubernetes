FROM fedora:32

# Create app directory
#WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json /

RUN npm install 
#RUN npm install npm@latest
# If you are building your code for production
# RUN npm ci --only=productio

# Bundle app source
COPY . .

# Expose the port
EXPOSE 8080
CMD [ "node", "./server.js" ]


