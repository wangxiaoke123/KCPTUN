1:wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh

2:chmod +x ./kcptun.sh

3:./kcptun.sh


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
