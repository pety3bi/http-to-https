HTTP to HTTPS
=============

[![Docker Pulls](https://img.shields.io/docker/pulls/pety3bi/http2https.svg)](https://hub.docker.com/r/pety3bi/http2https/)

The web is moving to TLS. This is a Docker container that forces browser
redirection from HTTP to HTTPS for all hosts that hit it.

HTTP code 307 is used to redirect browsers so that the HTTP method does not
change (which would happen with old clients using 301/302).

https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/307

Usage:
--------

```bash
docker run -d -p80:80 pety3bi/http2https:latest
```
