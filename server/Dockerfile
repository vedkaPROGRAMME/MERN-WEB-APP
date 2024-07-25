FROM node:16-alpine 

WORKDIR /app

COPY *.json .

RUN npm install

COPY . .

EXPOSE 5000

CMD ["npm","start"]





























