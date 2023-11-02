#the base image of node
FROM node:18-slim

WORKDIR /node

#copy the package.json to the workdir
COPY package*.json ./

RUN npm install 

RUN npm i -D handlebars@4.5.0

COPY . .

#exporse the webapp to port 4000
EXPOSE 4000

CMD ["node", "index.js"]

