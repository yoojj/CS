# Software Design Principle
: 소프트웨어 설계 원칙   

- [PIE](#pie)
- [SLAP](#slap)
- [DRY](#dry)
- [KISS](#kiss)
- [YAGNI](#yagni)

**OOP**  
- RDD
- [SOLID](#solid)
    - [SRP](#srp)
    - [OCP](#ocp)
    - [LSP](#lsp)
    - [ISP](#isp)
    - [DIP](#dip)


## PIE
Program Intently and Expressively      
: 의도를 표현하는 프로그램     
: 주석없이도 코드의 의도를 파악할 수 있게끔 코드 작성      



## SLAP
Single Level of Abstraction Principle     
: 가독성 목표     
: 복잡도에 따라 코드의 추상화를 고수준 추상화에서 저수준 추상화로 여러 계층으로 분리      
: 각 계층은 추상화 수준을 일치시켜 계층을 깨트리지 않도록 해야 함      
: 콜백 함수 사용과 모든 계층에서 공통으로 사용하는 함수나 모듈은 예외       

```
function 고수준() {
    중수준();
}

function 중수준() {
    저수준();
}

function 저수준() {
    // 구현
}
```



## DRY
Don’t Repeat Yourself   
: 재사용성 목표    
: 중복되는 코드는 함수화 또는 모듈화하고 이를 재사용    
: 반복되는 작업(ex. 빌드, 테스트 등)은 자동화    



## KISS
Keep It Simple Stupid     
: 단순성 목표   
: 불필요한 복잡성 지양   
: 시스템을 쉽게 이해하고 쉽게 확장하게 함        



## YAGNI
You Aren’t Gonna Need It  
: 단순성 목표   
: 당장 필요한 기능만 구현   
: 예상되는 기능을 추가하면 복잡성이 발생 함   


## RDD
Responsibility Driven Design



## SOLID

- [SRP](#srp)
- [OCP](#ocp)
- [LSP](#lsp)
- [ISP](#isp)
- [DIP](#dip)



### SRP   
Single Responsibility Principle   
: 단일 책임 원칙   
: 기능, 클래스, 모듈, 서비스에 명확하게 정의된 단일 책임만 부여해              
  자신에게 정의된 기능에만 집중하고 책임지는 설계 원칙     



### OCP
Open Closed Principle
: 개방 폐쇄 원칙     
: 확장을 위해서는 개방되고 변경을 위해서는 폐쇄되는 설계 원칙           
: 기능을 쉽게 확장할 수 있지만 확장한 기능이 다른 기능에 영향을 미치면 안됨  



### LSP
Liskov Substitution Principle   
: 리스코프 대체 원칙   
: 상속 관계인 서브 타입은 상위 타입의 조건-규약을 지켜 상위 타입을 치환할 수 있어야 하는 설계 원칙     
: 상위 타입의 규약을 지킬 수 없다면 별개 타입으로 구현해야 함   



### ISP
Interface Segregation Principle    
≒ GRASP    
: 인터페이스 분리 원칙   
: 모든 기능을 하나의 인터페이스에 포함하지 말고 기능에 따라 여러 인터페이스로 분리하는 설계 원칙   



### DIP
Dependency Inversion Principle   
: 의존 관계 역전 원칙  
: 추상화-인터페이스를 통해 객체를 느슨하게 결합하는 설계 원칙       
: 객체나 모듈은 추상화에 의존해야 함    

**dependency**        
: 의존성, 종속성   
: 한 클래스가 다른 클래스의 메소드를 사용하고 있는 관계   


```
상위 계층 -- 정책 결정
하위 계층 -- 세부 사항  
```


[top](#)
