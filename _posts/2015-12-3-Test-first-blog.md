---
layout: post
title: You're up and running!
---


server≈‰÷√
root@Node-1:~# cat /etc/ntp.conf 
peer 10.10.10.3 burst iburst minpoll 4 maxpoll 4
peer 10.10.10.2 burst iburst minpoll 4 maxpoll 4
# internal ntp server
server 127.127.1.0 burst iburst minpoll 4 maxpoll 4
fudge 127.127.1.0 stratum 10
disable monitor

client 1≈‰÷√
root@Node-2:~# cat /etc/ntp.conf 
peer 10.10.10.1 burst iburst minpoll 4 maxpoll 4
peer 10.10.10.3 burst iburst minpoll 4 maxpoll 4
# internal ntp server
server 10.10.10.1 burst iburst minpoll 4 maxpoll 4

client 2 ≈‰÷√
root@Node-3:~# cat /etc/ntp.conf 
peer 10.10.10.1 burst iburst minpoll 4 maxpoll 4
peer 10.10.10.2 burst iburst minpoll 4 maxpoll 4
# internal ntp server
server 10.10.10.1 burst iburst minpoll 4 maxpoll 4




![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/luqitao/luqitao.github.io) on GitHub.