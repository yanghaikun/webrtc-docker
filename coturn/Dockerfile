FROM ubuntu:17.10
RUN rm /etc/apt/sources.list
COPY sources.list /etc/apt/
RUN cat /etc/apt/sources.list
RUN apt-get update
RUN apt-get install coturn --assume-yes

EXPOSE 3478

CMD turnserver
