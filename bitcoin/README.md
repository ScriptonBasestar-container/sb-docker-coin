# Bitcoin

## Usage

### Build

```
docker build --build-arg TARGETPLATFORM=linux/amd64 -t sb-docker-bitcoin .
```

### Run

```
docker run --rm sb-docker-bitcoin bitcoind
```

### Push

```
docker tag sb-docker-bitcoin quay.io/scriptonbasestar/sb-docker-bitcoin
docker push quay.io/scriptonbasestar/sb-docker-bitcoin
```

## Config

```
-v ./example/bitcoin.conf:$BITCOIN_DATA/bitcoin.conf
```

| OS | Path |
| :------------- | :----------- |
|  Windows XP | `C:\Documents and Settings\<username>\Application Data\Bitcoin\bitcoin.conf` |
| Windows Vista, 7, 10 | `C:\Users\<username>\AppData\Roaming\Bitcoin` |
| Linux | `/home/<username>/.bitcoin/bitcoin.conf` |
| Mac OSX | `/Users/<username>/Library/Application Support/Bitcoin/bitcoin.conf` |

## REF

필요한 부분 퍼다가 씀

* https://github.com/ScriptonBasestar-docker/docker-bitcoin-core
* https://github.com/ruimarinho/docker-bitcoin-core

* https://bitcoin.stackexchange.com/questions/11190/where-is-the-configuration-file-of-bitcoin-qt-kept