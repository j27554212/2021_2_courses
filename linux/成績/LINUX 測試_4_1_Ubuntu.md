

## https://www.runoob.com/docker/docker-install-ubuntu.html
- https://hub.docker.com/_/ubuntu?tab=tags&page=1
- docker pull ubuntu
- docker run -itd --name ubuntu-A111E111 ubuntu
- docker run -itd --name ubuntu-A111E111 ubuntu
   - d5a76ba7b04a5a34f559076050fdea83052cf6bd0cb315ecef22539adcbda6ec
- docker exec -it ubuntu-A111E111 /bin/bash
```
docker exec -it  ubuntu-A111E111 /bin/bash
root@d5a76ba7b04a:/# uname -a
Linux d5a76ba7b04a 4.19.0-kali4-amd64 #1 SMP Debian 4.19.28-2kali1 (2019-03-18) x86_64 x86_64 x86_64 GNU/Linux


root@d5a76ba7b04a:/# whoami
root


root@d5a76ba7b04a:/# cat /etc/os-release
NAME="Ubuntu"
VERSION="20.04.3 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.3 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
root@d5a76ba7b04a:/# 
```
