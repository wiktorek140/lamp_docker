FROM alpine:latest
LABEL maintainer="wiktor Strzebala wiktorek140@tlen.pl"
LABEL description="Przykladowy Dockerfile dla serwera Apache & PHP."
ENV PHPVERSION=7
RUN apk add --update apache2 php${PHPVERSION}-apache2 php${PHPVERSION}
EXPOSE 80/tcp
ENTRYPOINT ["httpd"]
CMD ["-D", "FOREGROUND"]
