# LINUX 測試_4_2_Centos@Kali_2019.md

- docker pull centos
- docker run -itd --name centos-A111E111 centos

```
root@kali:~# docker run -itd --name centos-A111E111 centos
48f9577f1ff4638ec70a94a9424e14ef3536315893d38aec0ffab6b5c79c4eb6

root@kali:~# docker exec -it centos-A111E111 /bin/bash

[root@48f9577f1ff4 /]# uname -a
Linux 48f9577f1ff4 4.19.0-kali4-amd64 #1 SMP Debian 4.19.28-2kali1 (2019-03-18) x86_64 x86_64 x86_64 GNU/Linux

[root@48f9577f1ff4 /]# cat /etc/os-release
NAME="CentOS Linux"
VERSION="8"
ID="centos"
ID_LIKE="rhel fedora"
VERSION_ID="8"
PLATFORM_ID="platform:el8"
PRETTY_NAME="CentOS Linux 8"
ANSI_COLOR="0;31"
CPE_NAME="cpe:/o:centos:centos:8"
HOME_URL="https://centos.org/"
BUG_REPORT_URL="https://bugs.centos.org/"
CENTOS_MANTISBT_PROJECT="CentOS-8"
CENTOS_MANTISBT_PROJECT_VERSION="8"
[root@48f9577f1ff4 /]# 
```
