# Virtual Machine    
: OS 안에 가상 컴퓨터를 만들고 그 안에 다른 OS를 설치한 환경   
: 컴퓨터의 특정 구성을 소프트웨어를 통해 가상으로 구현  

물리 컴퓨터 - Host OS  
가상 컴퓨터 - Guest OS  


**데스크톱 가상화**   
Desktop Virtualization   
: 컴퓨터에 가상 머신을 구동 한 것


**하드웨어 가상 머신 소프트웨어**   
- [VirtualBox](./virtualbox.md)
- [VMware](./vmware.md)
- Parallels -- 맥
- QEMU -- 리눅스



## Virtual Machine Architecture
: Host OS와 Guest OS 사이에서 가상 라우터를 통해 가상 IP로 통신   

```
Guest OS -- 가상 라우터 -- Host OS -- 네트워크 카드    
```



[top](#)
