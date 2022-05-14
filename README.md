# HiMiner_Encrypt
以太坊本地加密挖矿，防止审查，百分之百加密数据，原理是本地加密后提交到服务器，服务器解密后再转发到矿池。网络中传输的就是一些列乱码。

# 操作方法
太帅了
机器连不上池子的可以试一下用hive官方版修改的本地代理，本地代理可以百分之百防止挖矿审查：
原理就是飞行表配置为本地，挖矿软件提交到本机加密后再提交到服务器，服务器解密后到矿池。

# Linux 服务器
### 1.在机器上运行这个命令
```
curl -s https://kocloud.oss-cn-hangzhou.aliyuncs.com/install_himiner.sh | bash
```
### 2.在飞行表上配置（挖矿地址）
```
127.0.0.1:8888
```

# window 下面如何操作
### 1.下载地址 https://kocloud.oss-cn-hangzhou.aliyuncs.com/himiner-win.exe
### 2.下载后打开软件，即可看见挖矿地址，一般是127.0.0.1:8888 挖矿地址填写这个即可
如果你想局域网内所有矿机都可以用这个加密，可以用这台电脑的局域网ip:8888到挖矿软件的矿池地址里
查看局域网地址:win+R弹出运行输入cmd打开命令提示符 输入ipconfig找到192.168开头的某个地址即为局域网地址
这个客户客户端设置开机自启：
右键himiner-win.exe点复制
打开文件夹，地址栏输入 %USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup 敲回车 然后在文件夹内右键-粘贴快捷方式
