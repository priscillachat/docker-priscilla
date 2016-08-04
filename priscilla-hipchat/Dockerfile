FROM debian:jessie

RUN apt-get update
RUN apt-get install -y ca-certificates

ADD http://priscilla.chat/downloads/priscilla-hipchat/latest/linux/amd64/priscilla-hipchat /priscilla-hipchat

RUN chmod a+x /priscilla-hipchat
RUN mkdir -p /var/log

CMD ["/priscilla-hipchat", "-conf", "/etc/priscilla.yml", "-confname", "hipchat"]
