FROM python:3.8-slim
#FROM ubuntu:latest

# Document who is responsible for this image
MAINTAINER Avantika Singh "as13594@nyu.edu"

# Install just the Python runtime (no dev)
RUN apt-get update
RUN apt-get install -y build-essential
COPY /pytorch-mnist/requirements.txt /tmp
COPY /pytorch-mnist/main.py  /tmp
WORKDIR /tmp
RUN pip3 install -r requirements.txt
CMD [ "python3", "main.py" ]

