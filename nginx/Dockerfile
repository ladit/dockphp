FROM nginx:alpine

RUN set -eux; \
    apk --no-cache add tzdata logrotate; \
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
    apk del tzdata;
