from node:alpine
workdir /usr/app
copy package.json .
run npm install
copy . .
cmd ["npm", "start"]
