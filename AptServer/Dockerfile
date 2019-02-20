FROM alpine:3.9
LABEL author="Serge NOEL <serge.noel@easylinux.fr>"

RUN apk add python \
    && mkdir -p /Data/mirror

WORKDIR /Data/mirror
EXPOSE 80
VOLUME /Data/mirror

CMD ["python","-m","SimpleHTTPServer","80"]
