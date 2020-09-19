# MVC
Model View Controller     
: 코드-컴포넌트를 구성하는 방법론   
: 컴포넌트를 데이터(Model), UI(View), 제어(Controller)에 따라 역할을 구분해 레이어를 분리하고          
&nbsp; 각 레이어에 속한 컴포넌트는 자신이 맡은 관심-역할에만 집중     
: 관심사를 분리하여 코드 관리를 수월하게 함   


**파생**  
- HMVC 계층 적 모델 뷰 컨트롤러
- MVA
- MVP
- MVVM


구성 요소 | 설명
---|---
model      | 데이터, 데이터베이스나 외부 API 접근  
view       | 표현, 모델을 사용해 렌더링
controller | 제어, 모델과 뷰 사이의 인터페이스


**Active Model MVC**   
: 모델의 상태 변경을 알리는 것은 모델 자신의 책임   
: 뷰나 컨트롤러를 통해 모델이 업데이트되면 이를 뷰에게 알림   


**Passive Model MVC**   
: 모델의 상태 변경을 알리는 것은 컨트롤러 책임    
: 컨트롤러는 모델을 업데이트 시키고 이를 뷰에게 알림     



## GUI MVC
: 초기 MVC 패턴은 GUI를 위한 아키텍처 스타일로 제시되어 UI, 비즈니스 로직, 데이터 접근을 기준으로 기능 분리    
: 초기 view는 시각적인 UI 구현만 가능했으며 이벤트 처리는 controller 담당        
: 이후 view와 controller를 쌍으로 구현해 위젯으로 사용하기도 함   
: 복잡하지 않은 GUI에만 적용 가능하며 UI가 발전하고 UI 로직이 복잡해지며 패턴이 변형됨       

1. 사용자 이벤트 발생
2. 컨트롤러에서 이벤트를 받아 (나중에는 뷰에서 이벤트를 받아 컨트롤러에 보냄)  
3. 이를 통해 모델 업데이트
4. 모델이 업데이트되면 이를 뷰에게 알려 렌더링을 요청  
5. 뷰는 업데이트된 모델을 사용해 렌더링  

http://heim.ifi.uio.no/~trygver/themes/mvc/mvc-index.html



## Web Application MVC
: HTTP 프로토콜의 특성으로 GUI 방식의 MVC 패턴 사용 불가 (Stateless 상태로 모델 유지 불가능)   
: Front Controller 패턴 도입    

1. 사용자 이벤트-요청 발생
2. 프론트 컨트롤러에서 모든 요청을 받아
3. 다른 컨트롤러에게 위임   
4. 요청을 전달받은 컨트롤러가 모델을 업데이트하고 이를 프론트 컨트롤러에게 전달하면
5. 프론트 컨트롤러가 뷰를 선택해 모델을 전달    


```
request  -->  front controller  -->  controller  
```


[top](#)
