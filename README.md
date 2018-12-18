## 在vps安装KCPTUN的代码

1:wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh

2:chmod +x ./kcptun.sh

3:./kcptun.sh

也可以用下面的一步代码

wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh && chmod +x ./kcptun.sh && ./kcptun.sh

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
