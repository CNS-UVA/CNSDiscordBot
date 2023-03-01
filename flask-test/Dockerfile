FROM python:3.8-slim-buster

WORKDIR /app
RUN  apt-get update
RUN  apt-get -y install libxml2-dev libxmlsec1-dev libxmlsec1-openssl gcc
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
ENV DISCORDTOKEN=token.txt


CMD [ "python3", "index.py"]
