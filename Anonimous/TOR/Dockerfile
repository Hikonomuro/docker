FROM alpine:latest

EXPOSE 9001:9001 9050:9050

COPY /Data/. /var/lib/tor/
COPY torrc /etc/tor/

RUN apk update      \
    && apk upgrade  \
    && apk add tor  
    
CMD tor