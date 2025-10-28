# pull official base image
FROM node:lts-slim

# set work directory
WORKDIR /app/

# add to $PATH
ENV PATH /app/node_modules/.bin:$PATH

# install app dependencies
COPY package*.json ./
RUN npm install

EXPOSE 5173

CMD ["npm", "run", "dev"]
