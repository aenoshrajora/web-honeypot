FROM python:3.8

LABEL MAINTAINER Aenosh Rajora "aenoshrajor79@gmail.com"

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

ADD honeypot/requirements.txt /requirements.txt
RUN pip install --upgrade pip
RUN pip install -r /requirements.txt
COPY honeypot/ / 
WORKDIR /
CMD python3 -u app.py