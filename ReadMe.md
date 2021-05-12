### Hardware requirment

Minimum:

CPU: 16 cores, RAM: 32G, Bandwidth: 100M, Disk: 1T

Recommended:

CPU: > 32 cores RAM: > 48G, Bandwidth: > 500M, Disk: > 2T

### Features

* Use official java-tron docker image (Although I would recommand you build your own docker images from source)
* Health check
* Mainnet config copied from [here](https://github.com/tronprotocol/tron-deployment/blob/master/main_net_config.conf)
* Log to docker stdout instead of a log file

### Usage:

```sh
docker-compose up -d --build

# Get sync/unFetchSynNum info
curl http://127.0.0.1:8090/wallet/getnodeinfo
```

### TODO

* Switch to [opentron](https://github.com/opentron/opentron) (arm64 server supported!)
* Swtich to Kubernetes with HA
