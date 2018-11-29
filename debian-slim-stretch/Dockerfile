FROM python:3.7.1-slim-stretch

LABEL version="0.1.4"
LABEL maintainer.name="Paolo Anastagi"
LABEL maintainer.email="poliez.poliez.p@gmail.com"

RUN apt-get update; \
    apt-get install curl -y; \
    curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py > get-poetry.py ; \
    python get-poetry.py ; \
    pip install confluent-kafka[avro]; \
    apt-get purge curl -y ; \
    apt-get autoremove -y ; \
    apt-get autoclean  -y ;

ENV PATH /root/.poetry/bin:$PATH