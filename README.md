# 阿里云盘小白羊版v3 Mac版
## 使用说明
由于macOS版本内置的Aria2有问题，因此需要在使用前自行安装Aria2并配置。  

1. 使用Homebrew安装aria2。
```bash
brew install aria2
```
2. 创建Aria2配置文件。
```bash
cd ~
mkdir .aria2
cd .aria2
vi aria2.conf
```
3. 填入以下配置文件
```
log-level=error
file-allocation=trunc
user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36
max-concurrent-downloads=64
max-connection-per-server=16
enable-rpc=true
rpc-allow-origin-all=true
rpc-listen-all=false
rpc-listen-port=16800
rpc-secret=S4znWTaZYQi3cpRNb
rpc-secure=false
pause-metadata=true
http-no-cache=true
disk-cache=32M
continue=true
allow-overwrite=true
auto-file-renaming=false
max-download-result=1000
no-netrc=true
reuse-uri=true
quiet=true
disable-ipv6=false
check-certificate=false
save-session=
save-session-interval=0
follow-metalink=false
follow-torrent=false
enable-dht=false
enable-dht6=false
bt-enable-lpd=false
enable-peer-exchange=false
bt-request-peer-speed-limit=1
dht-file-path=
dht-file-path6=
seed-time=0
force-save=false
bt-save-metadata=false
```
4. 启动Aria2。
```bash
aria2c --conf-path="/Users/xxxx/.aria2/aria2.conf" -D
```

**缺点是每次重启之后可能需要重新启动Aria2，你也可以自行加入开机自启动，会麻烦一些。**


## 项目说明
[阿里云盘小白羊版v3修复版 by odomu](https://github.com/odomu/aliyunpan)
<br>
[阿里云盘小白羊版v3的延续版 by PingKuNet](https://github.com/PingKuNet/aliyunpan)
<br>
[原阿里云盘小白羊版v3 by aliyunpan](https://github.com/liupan1890/aliyunpan)