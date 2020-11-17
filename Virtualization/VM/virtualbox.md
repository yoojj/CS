# VirtualBox
: 데스크톱 가상화 소프트웨어

- VirtualBox Install
- VBoxManage



## VirtualBox Install

```bash
# 의존 패키지 설치
$ sudo yum install -y gcc make patch dkms qt libgomp
$ sudo yum install -y kernel-headers kernel-devel fontforge binutils glibc-headers glibc-devel

$ cd /etc/yum.repos.d
$ sudo wget http://download.virtualbox.org/virtualbox/rpm/rhel/virtualbox.repo

$ sudo yum repolist
$ yum list VirtualBox*
$ sudo yum install VirtualBox-6.1

$ virtualbox
```



[top](#)
