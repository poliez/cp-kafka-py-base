FROM python:3.7.1-slim-stretch

LABEL version="0.1.1"
LABEL maintainer.name="Paolo Anastagi"
LABEL maintainer.email="poliez.poliez.p@gmail.com"

RUN apt-get update; \
    apt-get install curl -y; \
    curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py | python; \
    pip install confluent-kafka[avro]; \
    mkdir /app;

WORKDIR /app

ONBUILD COPY pyproject.* .

ONBUILD RUN poetry install --no-interaction --no-dev