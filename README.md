# SRUN_LOGIN

使用方法：

环境变量

`SRUN_UNAME`: 用户名

`SRUN_PASSWD`: 密码

`SRUN_HOST`: 域名，默认10.248.98.2

比方说路由器是梅林，就挂在WAN-START脚本下面就好。

交叉编译推荐用gox：

```bash
# set goproxy.io as proxy
export GOPROXY=https://goproxy.io
# install gox
go get -u github.com/mitchellh/gox
# cross compile
gox
```