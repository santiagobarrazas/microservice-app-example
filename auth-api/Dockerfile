FROM alpine:3.19

WORKDIR /app

COPY auth-api .
RUN apk add --no-cache libc6-compat

EXPOSE 8000

ENV JWT_SECRET=PRFT
ENV AUTH_API_PORT=8000
ENV USERS_API_ADDRESS=http://127.0.0.1:8083

CMD ["./auth-api"]
