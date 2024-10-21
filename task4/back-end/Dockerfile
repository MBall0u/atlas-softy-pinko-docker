FROM ubuntu:latest

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y python3 -y && \
    apt-get install python3-pip -y && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install flask && \
    pip3 install flask-cors

COPY ./api.py /app/api.py

WORKDIR /app
EXPOSE 5252

CMD ["echo", "Hello, World!"]