# dockerized-docs-chef

# What is it? #
Dockerzied Chef documentation for offline use.

# Image description #
- Base image: `httpd:2.4.23-alpine`.
- The most current ansible `master` branch is cloned and built using Sphinx documentation generator.
- Chef documentation directory (`/chef-web-docs/build`) is linked to httpd `DocumentRoot` (`/usr/local/apache2/htdocs`)  

# How to use this image #

```console
$ docker run -d genadipost/dockerized-docs-chef

```

You can test it by visiting http://container-ip:80
