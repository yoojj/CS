# Snap
: Linux 패키지 관리 시스템

Fedora, CentOS : yum   
Ubuntu, Debian : apt-get   


```bash
$ sudo yum install epel-release
$ sudo yum install snapd

# 활성화
$ sudo systemctl enable --now snapd.socket

# 심볼릭 링크 생성
$ sudo ln -s /var/lib/snapd/snap /snap
```
