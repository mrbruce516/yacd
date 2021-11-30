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
由于yacd需要监听本地设备/局域网设备的clash状态用以控制，所以必须以host网络模式启动。

若需要更改端口，请进入容器修改 /etc/nginx/conf.d/default.conf 中的端口为你需要的端口即可

have fun!
