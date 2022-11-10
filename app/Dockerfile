# pulling the image
FROM node:alpine

# creating the working directory 
WORKDIR /usr/src/app

# copy the package.json files from local machine to the workdir in container
COPY package*.json ./

# run npm install 
RUN npm install

# copy the generated modules and all other files to the container
COPY . .

# node app is running on port 5000 within the container, so need to expose it
EXPOSE 5000

# the command that starts app
CMD ["node", "index.js"]
