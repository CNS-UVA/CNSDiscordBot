FROM python:3.8-slim-buster

WORKDIR /app
RUN  apt-get update
RUN  apt install -y xmlsec1 pkg-config libxml2-dev libxmlsec1-dev
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
ENV DISCORDTOKEN=token.txt


CMD [ "python3", "index.py"]
