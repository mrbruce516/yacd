# yacd
clash dashboard for docker

## 快速使用
```bash
docker run --name yacd -d --net=host mrbruce516/yacd
```
若需要开机就对clash进行监控，则带上 `--restart` 参数
```bash
docker run --name yacd -d --net=host --restart=unless-stopped mrbruce516/yacd
```
