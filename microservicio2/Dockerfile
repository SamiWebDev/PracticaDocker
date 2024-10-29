FROM node:22.11.0-alpine

WORKDIR /opt

COPY microservicio2/package*.json ./

RUN npm install

RUN npm run test

COPY microservicio2/ .

EXPOSE 3000

CMD ["npm", "run", "start"]
