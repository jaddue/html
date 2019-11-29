# HTML이란?

HTML은 웹사이트 콘텐츠를 설명하는데 사용되는 마크업 언어


html에서 

ht는 HyperText 약자 
사용자 경험으로 text에 밑줄이 긋게 되고 이것을 클릭하게 되면 페이지가 전환되는 시스템

m은 markup은 구조를 설정할 때 사용

l은 Language 언어

> 구조를 설계할 때 사용하는 언어
> hyperlink 시스템을 가지고 있다. 
> .html 확장자를 가진 text에 불과하다.

1. text파일을 웹브라우저가 해석하고
2. 해석한 결과 구조를 통해 사용자가 보도록 렌더링 (그림을 그린다)
3. 렌더링 한 뷰를 사용자가 보게 된다.

# 시멘틱 마크업 (Semantic Markup)
> 의미를 부여하는 구조 설계

HTML은 콘텐츠의 의미를 설명하는데 유일한 목적을 가짐
구조 설계 (Structure Design)을 목표

## 컨텐츠를 감싸지 않는 요소 (empty element)

```html
<!-- 독타입이란 문서 유형 정의  (Document Type Definition) : 웹 표준 문서이자, 모던 브라우저에서 잘 돌아가는 호환되는 문서 -->
<!-- 독타입이 없게 되면 비표준 문서가 됨 -->
<!DOCTYPE html>
<!-- root element : 모든 요소의 조상 문서에서 사용되는 가장 주요한 언어를 지정할 수 있다. -->
<!-- lang의 정보는 장애인분들이 쓰는 스크린리더(낭독프로그램)에 읽게 만들어 줌 -->
<!-- -KR은 로컬 정보로 남한을 의미. 지역을 구분해야 될 경우 사용 en-GB, en-US, en-CA -->
<html lang="ko-KR">
    <!-- 브라우저가 인식할 수 있는 정보를 제공해 주는 영역 html의 자식 first child -->
    <head>
        <!-- empty element : 메타컨텐츠엔 글자 인코딩이 utf-8로 되어있다라는 정보만 필요해서 닫는 태그 불필요 -->
        <meta charset="utf-8">
    </head>
    <!-- 콘텐츠 영역 html의 자식 last child -->
    <body>
        <h1>해딩 엘리먼트 제목. h1는 대제목. 보통 문서에 한번 사용</h1>
        <h2>h1보단 덜 중요한 제목</h2>
        <h3>h2보단 덜 중요한 제목</h3>
        ...
        <h6>h6까지 사용 제목</h6>
        <p title="Development Tools">p 엘리먼트는 paragraph의 약자입니다. 단락</p>
        <!-- src : source, alt : alterate text 대체 텍스트로 이미지가 깨질 경우 대체 -->
        <!-- alt는 전맹시작장애자를 위한 대체 수단으로 이미지의 동등한 텍스트를 제공 받을 권리가 있다. 의무를 지켜줄 필요가 있다. > 접근성 준수 -->
        <!-- 대체 텍스트 작성 방법 : 1. 이미지 내용을 분석 2. 묘사. alt예시 -->
        <img src="" alt="html의 구조를 코딩중인 자두님">
    </body>
</html>
```
