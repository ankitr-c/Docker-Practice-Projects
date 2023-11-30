# FROM node:21-alpine

# WORKDIR /app

# COPY package*.json .

# RUN npm config set strict-ssl false
# RUN npm install

# COPY . .

# EXPOSE 3200
 
# CMD [ "npm", "start" ,"index.js"]

FROM node:21-alpine as build

WORKDIR /app

COPY package*.json .

RUN npm config set strict-ssl false
RUN npm install

FROM node:21-alpine

COPY --from=build /app/ .

EXPOSE 3200
 
CMD [ "npm", "start" ,"index.js"]

