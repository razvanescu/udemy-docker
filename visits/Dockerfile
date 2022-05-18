#Image
FROM node:alpine3.15

#Dependencies

WORKDIR '/app'

COPY package.json .
RUN npm install
COPY . .

#
CMD ["npm", "start"]