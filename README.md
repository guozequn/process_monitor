# Process Monitor Script

由于使用upstart管理crond存在bug，开机无法自动启动
另一方面supervisor被RD乱用导致socket被占用
所以临时写了这个脚本来管理crond以及一些其他的服务，在进程退出后自动拉起。

Recover crond when crash happends
This script can also monitor custom programs by adding config file, running stablely under upstart's managements.
