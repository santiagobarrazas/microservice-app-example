FROM python:3.6-alpine

WORKDIR /app

COPY . .

RUN apk add build-base

RUN pip install -r requirements.txt

ENV REDIS_HOST=172.20.0.2
ENV REDIS_PORT=6379
ENV REDIS_CHANNEL=log_channel
ENV ZIPKIN_URL=127.0.0.1

CMD ["python3","-u","main.py"]
