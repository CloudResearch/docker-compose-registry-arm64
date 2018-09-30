# Docker Compose for Registry ARM64

Fully working example of [Deploying Example](https://docs.docker.com/registry/deploying/). Used my docker registry image [Docker Registry ARM64](https://github.com/CloudResearch/docker-registry-arm64). 

## Content

* [The why?](#Why?)
* [What to do?](#What-to-do?)


## Why?

This package was developed for running docker registry on ARM64 devices. Builder image is based on arm64v8/golang and final registry image is based upon arm64v8/debian.


## What to do?

This image is build for ARM64. Based on the original distribution package.  
1. Just clone this repo.
2. Generate htpasswd with: ```htpasswd -B -c data/auth/htpasswd```
3. Put your certificate and private key in ```data/certs/```
4. ``docker-compose up -d``. Running on Port 5030. Done!

Used and tested on ARM64 [scaleway](http://scaleway.com) instance



