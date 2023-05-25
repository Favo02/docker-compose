FROM node:18-alpine

WORKDIR /app

# copy package.json and install dependencies
COPY package*.json ./
RUN npm ci

# copy and build content
COPY . .
RUN npm run build

# install serve and serve app
RUN npm install -g serve
EXPOSE 3000
CMD serve -s build
