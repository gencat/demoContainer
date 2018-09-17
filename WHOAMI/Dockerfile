FROM alpine

RUN apk add --no-cache py2-pip \
    && pip install --upgrade pip \
    && pip install flask \
    && rm -rf /var/cache/apk/*

COPY . /app
WORKDIR /app

EXPOSE 5000

CMD ["python","app.py"]
