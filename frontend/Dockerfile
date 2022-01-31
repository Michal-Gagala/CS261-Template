FROM node:16.13.2-bullseye
WORKDIR /app/frontend

# COPY package.json package-lock.json ./
COPY package.json ./
RUN npm install 
RUN npm install react-scripts@3.4.1 -g 
COPY . ./
EXPOSE 3000


# # pull official base image
# FROM node:16.13.2-bullseye

# # set working directory
# WORKDIR /app

# # add `/app/node_modules/.bin` to $PATH
# ENV PATH /app/node_modules/.bin:$PATH

# # install app dependencies
# COPY package.json ./

# CMD ["ls"]

# # COPY package-lock.json ./
# RUN npm install
# RUN npm install react-scripts@3.4.1 -g

# # add app
# COPY . ./

# # start app
# # CMD ["npm", "start"]