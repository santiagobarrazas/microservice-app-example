FROM node:8.17.0-alpine AS node

WORKDIR /app

COPY . .

RUN npm install
RUN npm run build

ENV PORT=8080
ENV AUTH_API_ADDRESS=http://127.0.0.1:8000
ENV TODOS_API_ADDRESS=http://127.0.0.1:8082
ENV ZIPKIN_URL=http://127.0.0.1:9411/api/v2/spans

EXPOSE 8080

CMD ["npm","start"]
