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
