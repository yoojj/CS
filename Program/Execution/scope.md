# Scope
: 변수의 수명-유효 범위

**종류**  
- [Lexical Scope](#lexical-scope)
- [Dynamic Scope](#dynamic-scope)



## Lexical Scope
= Static Scope, Rhetorical scope    
: 변수나 함수가 정의된 컨텍스트에 따라 유효 범위 결정    

소스코드가 작성된 그 문맥에서 결정
선언 위치에 따라 스코프가 달라지고 스코프에 따라 메모리 상주 주기가 결정    



## Dynamic Scope
: 변수나 함수가 호출된 호출 컨텍스트나 실행 컨텍스트에 따라 유효 범위 결정   


**perl**

```perl
$var = "global";

sub a() {
    local $var = "local";
    b();
}

sub b() {
    print "$var";
}

a();
b();
```


[top](#)
