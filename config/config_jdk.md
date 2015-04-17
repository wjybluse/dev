### 1.安装jdk
本次安装最新版的jdk，即jdk1.8，所以官方的仓库没有提供类似的东西,先去oracle的观望下载适合自container的版本

### 2.过程
>>在Dockerfile所在的目录建文件夹叫jdk
>>在Dockerfile里面加入 ADD ./jdk /tmp/jdk
>>安装命令rpm -ivh xx.rmp

### 3.备注
还可以增加自己的app folder，环境变量，然后启动自己的应用

