FROM python:3.8-slim-buster

WORKDIR /app
RUN  apt-get update
RUN  apt install -y xmlsec1 
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
ENV DISCORDTOKEN=token.txt


CMD [ "python3", "index.py"]
