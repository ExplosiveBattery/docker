FROM alpine:3.7

ENV LANG="en_US.UTF-8" \
    LC_ALL="en_US.UTF-8" \
    LANGUAGE="en_US.UTF-8" \
    DB_USER="root" \
    DB_PASS="root" \
    TERM="xterm"

RUN apk -U upgrade && \
    apk --update add \
      mariadb mariadb-client \
      && \
      rm -rf /tmp/src && \
      rm -rf /var/cache/apk/*


ADD ./my.cnf /etc/mysql/my.cnf
ADD ./start.sh /start.sh

RUN chmod u+x /start.sh

VOLUME ["/data"]
EXPOSE 3306

CMD ["/start.sh"]
