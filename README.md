# pure-ftpd
A docker image to manage a pure-ftpd server


```
docker run -d --name ftpd -p 21:21 -p 30000-30009:30000-30009 \
  -v `pwd`/ftpusers:/home/ftpusers \
  -v `pwd`/pure-ftpd:/etc/pure-ftpd \
  -e "PUBLICHOST=127.0.0.1" \
    ypereirareis/ftpd
```
