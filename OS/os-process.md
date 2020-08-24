# OS Process
≒ Task    
: 실행중인 프로그램의 인스턴스    
: 작업 처리를 위해 메모리에 로드된 명령어 집합   


- [프로세스 상태](#process-state)
- [프로세스 제어 블록](#process-control-block)
- [프로그램 주소 공간](#process-address-space)


**process vs program**    
: 프로그램 ≠ 프로세스    
: 프로그램은 기억 장치에 저장된 소스 코드 파일    

```
[ 프로그램 ] --> 메모리 --> [ 프로세스 ]

1. 프로그램 실행
2. OS를 통해 자원을 할당받아 메모리 확보
3. 로더에 의해 프로그램 명령어를 메모리에 적재  
    3-1. 코드가 적재된 메모리 주소를 명령 주소 레지스터에 저장
    3-2. 명령 주소 레지스터가 가르키는 주소를 명령 레지스터에 저장해 명령어 실행  
4. 프로세스 생성  
```


**process vs task vs thread**         
: 태스크는 프로그램이 메모리에 적재되어 호출할 수 있는 명령어 집합   
: 스레드는 프로세스의 실행 단위

```bash
                     프로그램
------------------------------------------------
|        프로세스        |    프로세스    |   ...
|   (스레드) (스레드) ... |               |

# 스레드는 해당 프로세스가 소유한 메모리와 자원에만 접근 가능  
```



## Process State
: 운영 체제에 따라 상태를 나타내는 단어 등이 다름    

```
created  -->  ready state  -->  running  -->  terminated  
생성 상태        준비 상태         실행 상태         종료 상태
```

- swapp in
    - ready : 필요한 자원을 소유하고 프로세서를 요청하고 있는 상태
    - running : 프로세서를 할당받은 상태
    - blocked, asleep
- swapp out
    - suspended ready : 프로세서를 요청한 상태
    - suspended blocked



## Process Control Block
: 프로세스 제어를 위해 프로세스에 대한 정보를 담고 있는 데이터 구조체     
: 프로세스 생성시 커널 공간에 만들어지며 프로세스가 종료되면 삭제됨    
: 운영 체제에 따라 다른 정보를 포함함      

**데이터 구성**   
- Process Identification Data
- Process State Data
- Process Control Data


```bash
Process ID            # 프로세스 고유 번호
Process Privileges    # 프로세스 권한
Process State         # 프로세스 상태
Process Pointer       # 상위 프로세스 주소  
Program Counter       # 다음 실행될 명령어 주소  
...
```



## Process Address Space  
: 프로그램이 실행되면 프로세스 주소 공간이 할당

종류 | 설명
---|---
code section(segment) | 프로그램 코드
data section(segment) | 정적 변수, 전역 변수 등 초기화 (bss 세그먼트 경우 초기화하지 않음)
heap  | 동적 할당 데이터
stack | 지역 변수, 함수, 임시 사용 데이터

! 기본은 4개이나 제조사의 컴파일러에 따라 차이 존재  



[top](#)
