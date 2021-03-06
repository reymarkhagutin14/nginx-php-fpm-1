[![Docker Hub; wyveo/nginx-php-fpm](https://img.shields.io/badge/docker%20hub-wyveo%2Fnginx--php--fpm-blue.svg)](https://hub.docker.com/r/wyveo/nginx-php-fpm/) [![](https://images.microbadger.com/badges/image/wyveo/nginx-php-fpm.svg)](http://microbadger.com/images/wyveo/nginx-php-fpm "Get your own image badge on microbadger.com") ![nginx 1.15.4](https://img.shields.io/badge/nginx-1.15.4-brightgreen.svg) ![php 7.2.10](https://img.shields.io/badge/php--fpm-7.2.10-blue.svg) ![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)
## Introduction
This is a Dockerfile to build a debian based container image running nginx and php-fpm 7.2.x / 7.1.x / 7.0.x & Composer.

### Versioning
| Docker Tag | GitHub Release | Nginx Version | PHP Version | Debian Version |
|-----|-------|-----|--------|--------|
| latest | master Branch |1.15.4 | 7.2.10 | stretch |
| php72 | php72 Branch |1.15.4 | 7.2.10 | stretch |
| php71 | php71 Branch |1.15.4 | 7.1.22 | stretch |
| php70 | php70 Branch |1.15.4 | 7.0.32 | stretch |
## Building from source
To build from source you need to clone the git repo and run docker build:
```
$ git clone https://github.com/wyveo/nginx-php-fpm.git
$ cd nginx-php-fpm
```

followed by
```
$ docker build -t nginx-php-fpm:latest . # PHP 7.2.x
```


or
```
$ docker build -t nginx-php-fpm:php71 . # PHP 7.1.x
```


## Pulling from Docker Hub
```
$ docker pull wyveo/nginx-php-fpm:latest
```

## Running
To run the container:
```
$ sudo docker run -d wyveo/nginx-php-fpm:latest
```

Default web root:
```
/usr/share/nginx/html
```
