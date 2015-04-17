### 1.安装
安装的过程中会出现没法访问https://index.docker.io/v1/repositories/library/centos/images，可以设置代理
设置步骤：
##### 1.在/etc/sysconfig/docker修改配置如下：
HTTP_PROXY=http://<your ip address>
http_proxy=$HTTP_PROXY
HTTPS_PROXY=$HTTP_PROXY
https_proxy=$HTTP_PROXY
export HTTP_PROXY HTTPS_PROXY http_proxy https_proxy
#### 2.重启docker
sudo service docker reload
