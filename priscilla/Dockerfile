FROM busybox

ADD http://priscilla.chat/downloads/latest/linux/amd64/priscilla /priscilla

RUN chmod a+x /priscilla
RUN mkdir -p /var/log

EXPOSE 4517

CMD ["/priscilla", "-conf", "/etc/priscilla.yml", "-log", "/var/log/priscilla.log"]
