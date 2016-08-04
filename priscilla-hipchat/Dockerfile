FROM debian:jessie

ADD http://priscilla.chat/downloads/priscilla-hipchat/latest/linux/amd64/priscilla-hipchat /priscilla-hipchat

RUN chmod a+x /priscilla-hipchat
RUN mkdir -p /var/log

CMD ["/priscilla-hipchat", "-conf", "/etc/priscilla.yml", "-confname", "hipchat"]
