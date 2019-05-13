# docker-cnpm

docker image of [cnpmjs.org](https://cnpmjs.org/), the "Company NPM" by alibaba ![nodejs-version-badge](https://img.shields.io/badge/node.js->=_6-blue.svg?style=flat-square) ![cnpmjs.org-version-badge](https://img.shields.io/badge/cnpm-2.19.4-blue.svg?style=flat-square)

https://hub.docker.com/r/zuibunan/cnpmjs

# Easy

    $ docker pull zuibunan/cnpmjs
    $ docker run -d \
                 -e CNPMJS_REPOSITORY=zuibunan/cnpmjs.org \
                 -e CNPMJS_ORG_VERSION=3.0.0-rc.21 \
                 -p 7001:7001 \
                 -p 7002:7002 \
                 -v /path/to/config:/var/app/cnpmjs.org/config \
                 -v /path/to/customize/README.md:/var/app/cnpmjs.org/docs/web/readme.md \
                 -v /path/to/storage:/var/www \
                 --name cnpm zuibunan/cnpmjs

# Reference

1. [GitHub: cnpm/cnpmjs.org](https://github.com/cnpm/cnpmjs.org)
2. [跟我一起部署和定制 CNPM——基础部署](http://f2e.souche.com/blog/let-cnpm-base-deploy/)
3. [Deploy a private npm registry in 5 minutes](https://github.com/cnpm/cnpmjs.org/wiki/Deploy-a-private-npm-registry-in-5-minutes)
