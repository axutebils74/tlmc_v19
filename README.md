# 我没有上传文件，都是不能访问的
使用的最大chunk大小 1MiB（即下面的--chunker,默认的为256KiB），最大子节点LINK数为174（默认的为174）
# 如何贡献
ipfs add -r --raw-leaves --cid-version 1  --chunker=size-1048576 -H {文件夹}
### 大于10G文件
ipfs config --json Experimental.FilestoreEnabled true   
ipfs add -r --raw-leaves --cid-version 1  --chunker=size-1048576 --nocopy -H {文件夹}
# 来源
- [kubo](https://github.com/ipfs/kubo)   
- [Touhou Lossless Music Collection v.19 (torrent)](https://sites.google.com/site/tlmcfiles/Touhou%20lossless%20music%20collection%20v.19.torrent)
- [Touhou Lossless Music Collection v.19](http://www.tlmc.eu/2018/01/tlmc-v19.html)
# 其他
- [ipfs desktop](https://github.com/ipfs-shipyard/ipfs-desktop#ipfs-desktop)
请选择当您生成一个分享链接时，使用哪一个公共网关。 http://209.94.90.1
# 新使用
ipfs init   
ipfs daemon 

http://127.0.0.1:8080/ipfs/{CID哈希}
# 待考虑
将 hash 算法换成 blake2b-256 即换成
ipfs add -r --raw-leaves --cid-version 1  --chunker=size-1048576 -hash=blake2b-256 --nocopy -H {文件夹}
