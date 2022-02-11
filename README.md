# dockphp

a personalized docker image for php web development mainly, trimed down version of [laradock](https://github.com/laradock/laradock). It is based on php:8-fpm-alpine. no other php version supported for now.

- use alpine, size down to 128MB uncompressed
- timezone: Asia/Shanghai
- nginx with logrotate

php modules:

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
hash
iconv
json
libxml
mbstring
mongodb
mysqlnd
openssl
pcre
PDO
pdo_mysql
pdo_sqlite
Phar
posix
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
