# Markup Language
: 마크업 명령어-태그를 사용하여 요소를 정의하고 표현하는 언어        


**markup**    
: 원고에서 지시 문구를 대신하는 범용 교정 부호-태그를 표시하는 것  


**문서 마크업 언어**   
- GML
- SGML
    - HTML : 웹 문서 생성시 사용
    - XML : 구조화된 데이터 저장시 사용
        - DocBook
        - MathML
- Markdown
- ...

문서 마크업 언어 목록   
https://en.wikipedia.org/wiki/List_of_document_markup_languages    


**TeX 계열 언어**  
: 프로그래밍이 가능한 마크업 언어  

- LaTeX
- pTeX



## 마크업 언어 유형
- 표현적 마크업
- 절차적 마크업
- 기술적 마크업



### 표현적 마크업
Presentational markup  
: 요소의 표현을 위해 사용되나 요소의 구조에 영향을 미치지 않음  
: WYSIWYG를 사용하는 워드 처리 시스템에서 사용  
: 일반적으로 사용자에게 보이지 않도록 숨겨져 있음   


**WYSIWYG**   
: what you see is what you get  



### 절차적 마크업
Procedural markup  
: 프로그램에서 요소의 처리 방법-명령 제공   
: 문서 내용 시각적 표현에 대한 정보 제공   

- Troff
- PostScript
- TeX



### 기술적 마크업
Descriptive markup   
= 설명적 마크업, 의미적 마크업  

- SGML
- XML



## PML
Practical Markup Language   
: 실용 마크업 언어    
: 문서 마크업 언어의 단점을 보완한 새 마크업 언어   
: 기사, 서적, 보고서 등의 문서를 인간 친화적으로 작성하도록 설계

http://www.practical-programming.org/


```
<!-- html -->
<i>텍스트</i>
<b><i>텍스트</i></b>


{- PML -}
{i 텍스트}
{b {i 텍스트}}
```



[top](#)
