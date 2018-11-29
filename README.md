# cp-kafka-py-base

[![](https://images.microbadger.com/badges/image/poliez/cp-kafka-py-base.svg)](https://microbadger.com/images/poliez/cp-kafka-py-base)

A Dockerfile that provides a base for using the [confluent-kafka python package](https://pypi.org/project/confluent-kafka) in your code. It comes with avro and its dependencies installed.

While the alpine one is available with and withouth [poetry](https://github.com/sdispater/poetry), the debian version only comes with it installed.

The alpine version is heavily inspired (basically the same) to [Python with libdrkafka](https://github.com/ucalgary/docker-python-librdkafka). 99% credits to them.