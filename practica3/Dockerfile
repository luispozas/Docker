#Esto es un ejemplo de DockerFile

FROM ubuntu:18.04
ENV LENGUAJE python
RUN apt-get update && apt-get install -y "$LENGUAJE"
RUN apt-get install -y wget
RUN mkdir /tmp/ejemplo
COPY Hola.txt /tmp/ejemplo

