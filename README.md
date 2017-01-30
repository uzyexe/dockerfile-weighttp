# uzyexe/weighttp

This is weighttp container.

## What is weighttp

weighttp - a lightweight and simple webserver benchmarking tool

[http://redmine.lighttpd.net/projects/weighttp/wiki](http://redmine.lighttpd.net/projects/weighttp/wiki)

## Dockerfile

[**Trusted Build**](https://registry.hub.docker.com/u/uzyexe/weighttp/)

This Docker image is based on the official [debian:jessie](https://hub.docker.com/_/debian/) base image.

## How to use this image

```
usage: docker run --rm uzyexe/weighttp <options> <url>
  -n num   number of requests    (mandatory)
  -t num   threadcount           (default: 1)
  -c num   concurrent clients    (default: 1)
  -k       keep alive            (default: no)
  -6       use ipv6              (default: no)
  -H str   add header to request
  -h       show help and exit
  -v       show version and exit

example: docker run --rm uzyexe/weighttp -n 10000 -c 10 -t 2 -k -H "User-Agent: foo" localhost/index.html
```

# Authors

* Shuji Yamada (<uzy.exe@gmail.com>)

## License

This project is licensed under the terms of the MIT license.
