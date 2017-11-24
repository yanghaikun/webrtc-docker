FROM ubuntu:17.10
RUN rm /etc/apt/sources.list
COPY sources.list /etc/apt/
RUN cat /etc/apt/sources.list
RUN apt-get update
RUN apt-get install coturn --assume-yes

EXPOSE 3478
EXPOSE 3479
CMD turnserver -a -f -v --mobility -m 10 --max-bps=100000 --min-port=32355 --max-port=65535 --user=ling:ling1234 --user=ling2:ling1234 -r demo
