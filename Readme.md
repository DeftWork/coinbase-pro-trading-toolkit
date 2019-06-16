# Coinbase Pro Trading toolkit

A [Docker](http://docker.com) file to build images for AMD & ARM devices with a installation of [Coinbase Pro Trading toolkit](https://github.com/coinbase/coinbase-pro-trading-toolkit) that provide all the tools traders need, both professional and hobbyist alike, to create automated trading bots on the Coinbase Pro and supported digital asset exchanges.

> Be aware! You should read carefully the usage documentation of every tool!

## Thanks to

- [Coinbase Pro Trading toolkit](https://github.com/coinbase/coinbase-pro-trading-toolkit)

## Details

- [GitHub](https://github.com/DeftWork/coinbase-pro-trading-toolkit)
- [Deft.Work my personal blog](http://deft.work)

| Docker Hub | Docker Pulls | Docker Stars | Docker Build | Size/Layers |
| --- | --- | --- | --- | --- |
| [coinbase-pro-trading-toolkit](https://hub.docker.com/r/elswork/coinbase-pro-trading-toolkit "elswork/coinbase-pro-trading-toolkit on Docker Hub") | [![](https://img.shields.io/docker/pulls/elswork/coinbase-pro-trading-toolkit.svg)](https://hub.docker.com/r/elswork/coinbase-pro-trading-toolkit "elswork/coinbase-pro-trading-toolkit on Docker Hub") | [![](https://img.shields.io/docker/stars/elswork/coinbase-pro-trading-toolkit.svg)](https://hub.docker.com/r/elswork/coinbase-pro-trading-toolkit "elswork/coinbase-pro-trading-toolkit on Docker Hub") | [![](https://img.shields.io/docker/build/elswork/coinbase-pro-trading-toolkit.svg)](https://hub.docker.com/r/elswork/coinbase-pro-trading-toolkit "elswork/coinbase-pro-trading-toolkit on Docker Hub") | [![](https://images.microbadger.com/badges/image/elswork/coinbase-pro-trading-toolkit.svg)](https://microbadger.com/images/elswork/coinbase-pro-trading-toolkit "elswork/coinbase-pro-trading-toolkit on microbadger.com") |

## Build Instructions

Build for amd64, armv7l, aarch64 architecture (thanks to its [Multi-Arch](https://blog.docker.com/2017/11/multi-arch-all-the-things/) base image)

``` sh
docker build -t elswork/coinbase-pro-trading-toolkit .
```

### Serve 

Test the coinbase-pro-trading-toolkit Docker image.

``` sh
docker run -it --rm elswork/coinbase-pro-trading-toolkit yarn test
``` 

Execute sample code from tutorials.

``` sh
docker run -it --rm elswork/coinbase-pro-trading-toolkit:armv7l ts-node tutorials/t001_feeds.ts
``` 

``` sh
docker run -it --rm elswork/coinbase-pro-trading-toolkit:armv7l ts-node tutorials/t002_liveOrderbook.ts
``` 

``` sh
docker run -it --rm elswork/coinbase-pro-trading-toolkit:armv7l ts-node tutorials/t003_tickertape.ts
``` 

And so ...
