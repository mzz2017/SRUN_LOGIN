# SRUN_LOGIN

深澜网络准入认证系统一键登录

使用方法：

环境变量

`SRUN_UNAME`: 用户名

`SRUN_PASSWD`: 密码

`SRUN_HOST`: 域名，默认10.248.98.2

`SRUN_KEEP_ALIVE`: 设为1或true则每隔180秒发送一次请求以保持在线，可以与nohup一起使用

### Docker

```shell script
docker run -d --restart=always \
           -e SRUN_UNAME=yourusername \
           -e SRUN_PASSWD=yourpassword \
           -e SRUN_KEEP_ALIVE=1 \
           --name srun_login \
           mzz2017/srun_login
```
