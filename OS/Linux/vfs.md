# Virtual File System   
= 가상 파일 시스템 스위치       
: 커널과 파일 시스템 사이에 형성된 추상화 계층-인터페이스        
: 사용자-프로그램이 파일 시스템에 접근시 각각의 파일 시스템에 대해 알 필요없이 VFS을 통해 접근     


```
    커널
-------------
가상 파일 시스템
-------------
  파일 시스템
```


**지원**    
- 디스크 파일 시스템
- 네트워크 파일 시스템
- 특수 파일 시스템



## VFS Data Structures
- superblock object
- inode object
- dentry object
- file object
