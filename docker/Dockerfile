# check=skip=JSONArgsRecommended
FROM ubuntu:22.04

WORKDIR /src
COPY src/main.py /src/main.py
COPY requirements.txt /src/requirements.txt
RUN apt update &&\
    apt install -y python3.10 &&\
    apt install -y python3-pip
RUN pip install -U pip &&\
    pip install -r /src/requirements.txt
