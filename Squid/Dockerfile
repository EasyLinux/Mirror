FROM alpine:3.9
LABEL autohor="Serge NOEL <serge.noel@net6a.com>"

RUN apk update \
    && apk add --no-cache squid
    # echo "cache_access_log /dev/stdout" >> /etc/squid/squid.conf

VOLUME /var/cache/squid
EXPOSE 3128

CMD ["/usr/sbin/squid", "-N"]

