## Differences from the original
automatic build and push docker image  
updated alpine and packages  
added docker image build for arm64 servers  

### Upstream Links

* Docker Registry @ [nubacuk/3proxy](https://hub.docker.com/r/nubacuk/3proxy)
* Original GitHub @ [3proxy/3proxy](https://github.com/3proxy/3proxy)

### Docker run 
The architectures supported by this image are:

| Architecture | Available | Tag |
| :----: | :----: | ---- |
| x86-64 | ✅ | x86_64 |
| arm64 | ✅ | aarch64 |
  
  There are images for aarch64(arm) and x86_64

```
docker run -p 3128:3128 -p 1080:1080 -v /path/to/local/config/directory:/usr/local/3proxy/conf --restart always --name 3proxy nubacuk/3proxy:aarch64
```