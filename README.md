## 在vps安装KCPTUN的代码

1:wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh

2:chmod +x ./kcptun.sh

3:./kcptun.sh

也可以用下面的一步代码

wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh && chmod +x ./kcptun.sh && ./kcptun.sh

或者我自己的

wget --no-check-certificate https://github.com/wangxiaoke123/kcptun/raw/master/kcptun/kcptun.sh && chmod +x ./kcptun.sh && ./kcptun.sh

原作者已删除bin文件，需要手动下载自己包里的bin文件

启动：
supervisorctl start kcptun

停止：
supervisorctl stop kcptun

重启：
supervisorctl restart kcptun

状态：
supervisorctl status kcptun

卸载：
./kcptun.sh uninstall

## 如果出现问题如：
Starting supervisor: Error: Another program is already listening on a port that one of our HTTP servers is configured to use.  Shut this program down first before starting supervisord.
For help, use /usr/bin/supervisord -h

通过解除.sock file的连接来解决问题:sudo unlink /var/run/supervisor.sock

## kcptun客户端下载和kcptun启动工具
https://github.com/xtaci/kcptun/releases

https://github.com/dfdragon/kcptun_gclient/releases
