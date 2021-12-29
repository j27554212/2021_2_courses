## node.js
- docker pull node
- docker run -itd --name node-test node

```
root@kali:~# docker pull node
Using default tag: latest
latest: Pulling from library/node
0e29546d541c: Pull complete 
9b829c73b52b: Pull complete 
cb5b7ae36172: Pull complete 
6494e4811622: Pull complete 
6f9f74896dfa: Pull complete 
f2930ff7fb60: Pull complete 
c1d26179dd86: Pull complete 
1fa56dd41537: Pull complete 
321141c774e9: Pull complete 
Digest: sha256:36aca218a5eb57cb23bc790a030591382c7664c15a384e2ddc2075761ac7e701
Status: Downloaded newer image for node:latest
docker.io/library/node:latest


root@kali:~# docker run -itd --name node-test node
bdd9898a46bd8c3f42cb9f1ae334826dbdafa43de585f4755686bb913774dd43

root@kali:~# docker exec -it node-test /bin/bash
root@bdd9898a46bd:/# uname -a
Linux bdd9898a46bd 4.19.0-kali4-amd64 #1 SMP Debian 4.19.28-2kali1 (2019-03-18) x86_64 GNU/Linux
root@bdd9898a46bd:/# node -v
v17.3.0
root@bdd9898a46bd:/# 
```
