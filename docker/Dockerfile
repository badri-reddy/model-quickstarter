FROM openjdk:8u242-jdk-buster

MAINTAINER  DBpedia Spotlight Team <dbp-spotlight-developers@lists.sourceforge.net>

RUN apt-get update
RUN apt-get install -y apt-utils

RUN apt-get install maven -y && git clone https://github.com/badri-reddy/model-quickstarter.git && git clone https://github.com/badri-reddy/wikistatsextractor.git && git clone https://github.com/badri-reddy/dbpedia-spotlight-model.git && mv dbpedia-spotlight-model dbpedia-spotlight && cd dbpedia-spotlight && mvn clean install

SHELL ["/bin/bash", "-c"]
