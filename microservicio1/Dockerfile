FROM node:22.9.0-alpine


WORKDIR /opt

COPY package*.json ./

RUN npm install

RUN npm run test

COPY . .

EXPOSE 3000

CMD ["npm", "run", "dev"]
