FROM node:22.9.0-alpine

WORKDIR /opt

COPY microservicio2/package*.json ./

RUN npm install

COPY microservicio2/ .

RUN npm run test


EXPOSE 3000

CMD ["npm", "run", "start"]
