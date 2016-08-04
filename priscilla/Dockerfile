FROM debian:jessie

RUN apt-get update
RUN apt-get install -y ca-certificates

ADD http://priscilla.chat/downloads/priscilla/latest/linux/amd64/priscilla /priscilla

RUN chmod a+x /priscilla
RUN mkdir -p /var/log

EXPOSE 4517

CMD ["/priscilla", "-conf", "/etc/priscilla.yml"]
