# OOP Design Principle   
: 소프트웨어 설계 원칙   

- [RDD](#rdd)
- [SOLID](#solid)
    - [SRP](#srp)
    - [OCP](#ocp)
    - [LSP](#lsp)
    - [ISP](#isp)
    - [DIP](#dip)
- [GRASP](#grasp)



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



## GRASP
General Responsibility Assignment Software Principles     


1. 정보 담당자 Information Expert
2. 소유권한 Creator
3. 컨트롤러 Controller
4. 낮은 연결 Low Coupling
5. 높은 응집도 High Cohesion
6. 간접 참조 Indirection
7. 다형성 Polymorphism
8. 순수 조립 Pure Fabrication
9. 변화 보호 Protected Variations



[top](#)
