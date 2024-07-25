FROM node:20 AS builder

WORKDIR /app

COPY *.json .

RUN npm install 

COPY . .

RUN npm run build

FROM nginx:1.25.2-alpine-slim

COPY --from=builder /app/build /usr/share/nginx/html

EXPOSE 80

CMD ["nginx","-g","daemon off;"]






























