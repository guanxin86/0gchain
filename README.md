# 0gchain
0gchain常用命令
### storage查询
```
curl -X POST http://localhost:5678 -H "Content-Type: application/json" -d '{"jsonrpc":"2.0","method":"zgs_getStatus","params":[],"id":1}'  | jq
```
### 更新addrbook(itrockert)
```
wget -O $HOME/.0gchain/config/addrbook.json https://server-5.itrocket.net/testnet/og/addrbook.json
```
### 高度查询
[itrocket/0g](https://testnet.itrocket.net/og)
### 编辑存储config文件
```
nano $HOME/0g-storage-node/run/config-testnet.toml
```
### 查询日志
```
tail -f -n 100 ./0g-storage-node/run/log/zgs.log.$(date +"%Y-%m-%d")
```
