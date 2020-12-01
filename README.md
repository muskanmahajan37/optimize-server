# optimize-server

## /etc/security/limits.conf

```
root soft nofile 1040000
root hard nofile 1040000

root soft nofile 1040000
root hard nproc 1040000

root soft core unlimited
root hard core unlimited

* soft nofile 1040000
* hard nofile 1040000

* soft nofile 1040000
* hard nproc 1040000

* soft core unlimited
* hard core unlimited
```

## /proc/sys/fs/file-max

```
cat /proc/sys/fs/file-max
12553500
```

## /etc/sysctl.conf

```
net.ipv4.ip_local_port_range = 1024 65000
net.ipv4.tcp_mem = 786432 2097152 3145728
net.ipv4.tcp_rmem = 4096 4096 16777216
net.ipv4.tcp_wmem = 4096 4096 16777216
```
