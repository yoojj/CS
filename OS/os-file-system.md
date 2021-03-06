# OS File System
: 저장 장치에서 파일을 읽거나 저장하고 검색이 용이하도록 관리하는 체계 및 프로그램     

- [File](#file)
- [File System](#file-system)



## File
: 저장 장치에 저장되고 조회, 변경, 삭제 가능한 논리적 단위의 데이터 집합            
: 유닉스(리눅스) 경우 일반 파일, 심볼릭 링크, 디바이스, FIFO 파일 등 데이터 집합 모두 파일로 간주    


**파일 구성** (메타 정보)      
- 데이터
- 파일 상태 정보
    - 이름
    - 식별자 : 파일 시스템에서 파일을 식별하는 고유 태그 번호로 사용자는 읽을 수 없음  
    - 종류
    - 크기
    - 소유자   
    - 권한 : 읽기, 쓰기, 실행 등 제어  
    - 위치 : 파일이 저장된 위치
    - 시간 : 파일 접근 시간, 파일 수정 시간 등
    - ...


**파일 분류**     
- 데이터 파일
    - 텍스트 파일 (ASCII 파일)
    - 바이너리 파일
- 프로그램 파일
    - 원시 프로그램 파일
    - 목적 프로그램 파일
    - 실행 파일



## File Operation
= 파일 작업, 파일 조작   

- 파일 생성
- 파일 작성
- 파일 저장
- 파일 조회  
- 파일 삭제
- 파일명 변경
- 파일 복사  
- ...



## File Storage

- 저장 매체
- 접근 장치
- 저장 장치  
    - 1차 저장 장치 -- 소멸성  
        - 메인 메모리 : 파일 처리를 위한 공간  
        - 캐시 메모리 : 메인 메모리 성능 향상
        - 플래시 메모리 -- 비휘발성  
    - 2차 저장 장치 -- 비소멸성  
        - 자기 디스크
        - 광 디스크  
        - 자기 테이프
        - ...



## File Access
: 파일 사용시 메인 메모리에 적재된 상태여야 하므로 저장 장치에 존재하는 파일에 접근해야 함    
: 성능을 위해 저장 장치에 파일 접근을 최소화해야 좋음     


**Access Method**  
- 순차 접근
- 직접 접근
- 색인화된 접근
    - Index Access Method
    - Index sequential Access Method



### 순차 접근
: 저장 장치에서 첫 레코드부터 순차적으로 탐색하여 원하는 레코드에 접근    
: 일반적인 방법이나 순차적으로 접근하므로 빈번한 파일 작업시 느림  



### 직접 접근
= 임의 접근   
: 주소 결정 기법을 이용하여 원하는 레코드에 직접 접근   



[top](#)
