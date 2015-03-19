# docker-nodejs

A compilation of [NodeJS](https://nodejs.org/) builds for various Operating Systems.


# Howto

* Clone this repository
* Pull a NodeJS docker image: docker pull yoanisgil/nodejs:centos6.6-0.12
* Launch the demo application: docker run -it --rm --name my-running-script -v "$PWD":/tmp -w /tmp -p 8000:8000 yoanisgil/nodejs:centos6.6-0.12 node apps.js
* Visit your browser at: http://localhost:8000 (Note if you're running Docker on OSX you need to get the IP address by running "boot2docker ip")
