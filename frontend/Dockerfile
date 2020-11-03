FROM node:14

# set up angular cli
RUN npm install -g @angular/cli

WORKDIR /app
COPY package.json /app
RUN npm install 
COPY . /app

# create dist
RUN ng build --prod