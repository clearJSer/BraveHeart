# 背景
去了新的公司或者换了新的电脑 开始工作之前第一步就是配置git SSH环境 

这里整理了mac 和 windows环境下 配置github gitlab 和其他环境的SSH协议 

免去查找教程的烦恼 直接从这里起步！

这个文档目的是做到一劳永逸，利人利己！

### 1 Windows环境下

ssh-keygen -t rsa  -C "xxxx@xx.com你的邮箱"

// 秘钥文件重新命名的逻辑  
PS D:\WebGL> ssh-keygen -t rsa  -C "lakiliu@tencent.com"
Generating public/private rsa key pair.
Enter file in which to save the key (C:\Users\Administrator/.ssh/id_rsa): C:\Users\Administrator/.ssh/id_rsa_tx

#### 配置多环境配置文件
文件地址：  C:\Users\Administrator\.ssh
Host github
HostName github.com
IdentityFile ~/.ssh/id_rsa.github
```
User clearJSer

Host gitlab

HostName  gitlab.com 

IdentityFile `~/.ssh/id_rsa_gitlab`
```
Host对应的名称是一个别名，命名可以随意，用来进行远程连接，当然使用真实的主机名称也是可以的。
HostName和IdentityFile就是各自主机名称以及对应的秘钥文件了~

### 2 Mac环境下
.ssh 路径：  ~/.ssh

