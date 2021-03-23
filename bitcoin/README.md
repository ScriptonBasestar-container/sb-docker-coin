# Bitcoin

build image
```
docker build --build-arg TARGETPLATFORM=linux/amd64 -t sb-docker-bitcoin .
docker run --rm sb-docker-bitcoin bitcoind

docker tag sb-docker-bitcoin quay.io/scriptonbasestar/sb-docker-bitcoin
docker push quay.io/scriptonbasestar/sb-docker-bitcoin
```

## REF

필요한 부분 퍼다가 씀

* https://github.com/ScriptonBasestar-docker/docker-bitcoin-core
* https://github.com/ruimarinho/docker-bitcoin-core
