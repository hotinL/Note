### Redis安装

- Redis的安装

### Redis5.0 启动报错

1. `WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128`
2. `WARNING overcommit_memory is set to 0! Background save may fail under low memory condition. To fix this issue add 'vm.overcommit_memory = 1' to /etc/sysctl.conf and then rebootrcommit_memory=1' for this to take effect`
3. `WARNING you have Transparent Huge Pages (THP) support enabled in your kernel. This will create latency and memory usage issues with Redis. To fix this issue run the command 'echo never > /sys/kernel/mm/transparent_hugepage/enabled' as root, and add it to your /etc/rc.local in order to retain the setting after a reboot. Redis must be restarted after THP is disabled`

#### 防火墙相关操作

##### 启动

> `systemctl start firewalld.service`

##### 关闭

> `systemctl stop firewalld.service`

##### 更新

>  `firewall-cmd --reload`

##### 开启端口

> `firewall-cmd --zone=public --add-port=6379/tcp --permanent  `       
>
> `--permanent`  永久生效    

##### 关闭端口

> `firewall-cmd --remove-port=6379/tcp --permanent  `           

##### 查看所有端口

> `firewall-cmd --zone=public --list-ports`



