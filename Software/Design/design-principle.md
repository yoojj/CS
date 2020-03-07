# Software Design Principle
: 소프트웨어 설계 원칙   

- [PIE](#pie)
- [SLAP](#slap)
- [DRY](#dry)
- [KISS](#kiss)
- [YAGNI](#yagni)

**OOP**  
- [RDD](./design-principle-oop.md#rdd)
- [SOLID](./design-principle-oop.md#solid)
- [GRASP](./design-principle-oop.md#grasp)



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



[top](#)
