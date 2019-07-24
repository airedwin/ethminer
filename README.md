# Ethereum CUDA Miner
Based on work by Anthony-Tatowicz https://github.com/Anthony-Tatowicz/docker-ethminer/ \
Updated to use nvidia's cuda 10.1 docker image\
Updated to use ethmine 0.18.0

### Docker container for Ethereum mining with CUDA.

Simple and easy to run, if you have a Nvidia GPU and want to mine eth.

**Note:** This image builds ethminer, which is an activily maintained Genoil fork <https://github.com/ethereum-mining/ethminer>

### Requirements
- Nvidia drivers for your GPU, you can get them here: [Nvidia drivers](http://www.nvidia.com/Download/index.aspx)
- Nvidia-docker (so docker can access your GPU) install instructions here: [nvidia-docker](https://github.com/NVIDIA/nvidia-docker)

### How to run
```
$ nvidia-docker run -it airedwin/ethminer ARG1 ARG2 ...

# Example
$ nvidia-docker run -it airedwin/ethminer \
-P stratum://0x123456789@us1.ethermine.org:4444
```

**Note:** `-U` is set by default

### Help
`$ etherminer --help`

