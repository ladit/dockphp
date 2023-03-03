# dockphp

a personalized docker image for php web development mainly, trimed down version of [laradock](https://github.com/laradock/laradock). It is based on php:fpm-alpine. Latest php 7/8 is supported.

- use alpine, size down to 155MB uncompressed
- timezone: Asia/Shanghai
- nginx with logrotate

default php modules:

```
[PHP Modules]
bcmath
Core
ctype
curl
date
dom
fileinfo
filter
ftp
gd
grpc
hash
iconv
json
libxml
mbstring
mcrypt
mongodb
mysqlnd
openssl
pcre
PDO
pdo_mysql
pdo_sqlite
Phar
posix
protobuf
random
rdkafka
readline
redis
Reflection
session
SimpleXML
sodium
SPL
sqlite3
standard
tokenizer
xdebug
xlswriter
xml
xmlreader
xmlwriter
yaml
Zend OPcache
zlib

[Zend Modules]
Xdebug
Zend OPcache
```
