# Linux 伺服器建置報告

 - apache 網站伺服器建置
 - Mysql 資料庫伺服器建置
 - PHP
 - 網站程式開發

## apache 網站伺服器建置: 以Kali linux 2021.3版為基礎

### service apache2 status
```
apache2.service - The Apache HTTP Server
     Loaded: loaded (/lib/systemd/system/apache2.service; disabled; vendor preset: disabled)
     Active: inactive (dead)
       Docs: https://httpd.apache.org/docs/2.4/
```
### cd /etc/init.d

### ls
```
apache2              hwclock.sh         openvpn                      screen-cleanup
apache-htcacheclean  inetsim            plymouth                     smartmontools
apparmor             iodined            plymouth-log                 smbd
atftpd               ipsec              postgresql                   snmpd
avahi-daemon         keyboard-setup.sh  procps                       speech-dispatcher
binfmt-support       kmod               ptunnel                      ssh
bluetooth            lightdm            pulseaudio-enable-autospawn  sslh
console-setup.sh     mariadb            redsocks                     stunnel4
cron                 miredo             rpcbind                      sudo
cryptdisks           networking         rsync                        sysstat
cryptdisks-early     nfs-common         rsyslog                      udev
dbus                 nginx              rwhod                        virtualbox-guest-utils
dns2tcp              nmbd               samba-ad-dc                  x11-common
haveged              ntp                saned                        xl2tpd
```


```
#/etc/init.d/apache2 start
#/etc/init.d/apache2 stop
#/etc/init.d/apache2 restart
```
## ./apache2 -h 
```
Usage: apache2 {start|stop|graceful-stop|restart|reload|force-reload}
```
### ./apache2 start
```
Starting apache2 (via systemctl): apache2.service.
```
