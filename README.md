# 我没有上传文件，都是不能访问的
使用的最大chunk大小 256kb（默认），最大子LINK数为174（默认）
# 如何贡献
ipfs add -r --raw-leaves --cid-version 1 -H {文件夹}
### 大于10G文件
ipfs config --json Experimental.FilestoreEnabled true   
ipfs add -r --raw-leaves --cid-version 1 --nocopy -H {文件夹}
# 来源
- [kubo](https://github.com/ipfs/kubo)   
- [Touhou Lossless Music Collection v.19 (torrent)](https://sites.google.com/site/tlmcfiles/Touhou%20lossless%20music%20collection%20v.19.torrent)
- [TLMC](http://www.tlmc.eu/2018/01/tlmc-v19.html)
# 其他
- [ipfs desktop](https://github.com/ipfs-shipyard/ipfs-desktop#ipfs-desktop)
请选择当您生成一个分享链接时，使用哪一个公共网关。 http://209.94.90.1
# 新使用
ipfs init   
ipfs daemon 

http://127.0.0.1:8080/ipfs/{CID哈希}
