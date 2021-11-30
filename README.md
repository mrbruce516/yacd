# yacd
clash dashboard for docker
https://hub.docker.com/r/mrbruce516/yacd

## 快速使用
```bash
docker run --name yacd -d --net=host mrbruce516/yacd
```
若需要开机就对clash进行监控，则带上 `--restart` 参数
```bash
docker run --name yacd -d --net=host --restart=unless-stopped mrbruce516/yacd
```
### 使用 `docker-compose` 部署 (可选)  
下载本仓库中的 `docker-compose.yml`，按照个人需求进行编辑
```bash
docker-compose up -d
```
