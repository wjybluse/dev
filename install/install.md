### 1.安装docker，此次以centos为例
安装稳定版本：
```shell
#install
sudo yum -y install docker
#start
sudo service docker start

#auto start
sudo chkconfig docker on

#remove
sudo yum -y remove docker
```

### 2.简单的查询命令
```shell
#list images
sudo docker images

#list all started container
sudo docker ps

#list all container
sudo docker ps -a

```

### 3.删除命令
```shell
#remove image 
sudo docker rmi <imageId>

#remove container
sudo docker rm <containerId>
```

### 4.创建dockerfile
Dockerfile简单的命令:
```
    FROM <image>:image 格式name:tag
    MAINTAINER :author
    RUN       :run command
    CMD       :can run only once
    EVN       :config env params
    ENTRYPOINT:cannot ovveried,same as CMD ,run after builded
```
### 5.构建自己的镜像
```shell
sudo docker build -t <name>/<xx> .
```

如果构建成功可以用sudo docker images 查看你自己的镜像

### 6.后记
1.4版本的docker好像有问题，连不上rehat的仓库，没找到问题，配置代理也不行，1.5没问题
后续将继续网络配置和卷的设置，还有container之间互通
