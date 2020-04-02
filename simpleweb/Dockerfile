# Specify a base image
FROM node:alpine

# Specifying this, create a new directorfor us to work and separate out our files from the filesystem files
WORKDIR /usr/app

# Install some depenendencies

# First copy dependency files and then install npm
COPY ./package.json ./
RUN npm install

# now copy everything, so that if any changes is made in application wh doesn't need dependencies to be installed, it won't and only application file changes will be copied.
COPY ./ ./

# Default command
CMD ["npm", "start"]
