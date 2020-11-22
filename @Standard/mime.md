# MIME
Multipurpose Internet Mail Extensions    
: 전자 메일의 기능을 확장하기 위한 표준      
: 메시지 캡슐화와 오디오, 비디오 등 첨부 파일을 지원하기 위해 등장  

RFC
- https://tools.ietf.org/html/rfc1341    
- https://tools.ietf.org/html/rfc1521
- https://tools.ietf.org/html/rfc1522


**MIME Message**
```bash
# MIME Header
MIME-Version : 1.0
Content-Type := type/subtype ; parameter       
Content-Transfer-Encoding : 7bit | 8bit | base64 | quoted-printable | binary  
Content-ID :
Content-Description :
Content-Disposition :

# MIME Body
```



## MIME Type
= Content-Type    
: 데이터 타입을 구별하기 위한 문자열     
: 이메일 메시지 헤더와 HTTP 메시지 헤더에서 사용   


타입 | 설명
---|---
application | 애플리케이션 데이터, 바이너리 데이터
audio       | 오디오 파일
image       | 이미지 파일
message     | 메시지, 메시지에 대한 포인터  
multipart   | 멀티 메시지
text        | 사람이 읽을 수 있는 형식의 문자열 메시지
video       | 비디오 파일
x-token     | 비표준 혹은 사용자 정의 콘텐츠 타입

ex.
```
Content-Type : "application/x-www-form-urlencode"   
Content-Type : "audio/mpeg"
Content-Type : "image/jpeg"
Content-Type : "message/http"   
Content-Type : "multipart/formed-data"
Content-Type : "text/html"
Content-Type : "video/webm"
```



[top](#)
