### 학습목표
* HTML 기초
* CSS 기초

## HTML(HyperText Markup Language)

문서의 틀이나 내용을 다루는 언어

* HTML은 tag들의 집합
* tag : 부등호(< >)로 묶인 HTML의 기본 구성 요소
	Tree Structure 
  	(따로 상세히 정리하여 추가)
  
  ```
  <div></div> | <body></body> | <title></title> 등
  ```
  
  * html 확장자 사용
## Markup Language(마크업)
>태그 등을 이용하여 문서나 데이터의 구조를 명기하는 언어의 한 가지
>>태그
* 원래 텍스트와는 별도로 원고의 교정부호 및 주석을 표현하기 위한 것이었으나 용도가 점차 확장되어 문서의 구조를 표현하는 역할을 하게 됨
<br>
 * 문서의 골격에 해당하는 부분을 작성
 <br>
* 일반적으로는 데이터를 기술하는 정도로만 사용되기 때문에 프로그래밍 언어와는 구분됨

### 마크업 언어 종류
- GenCode / troff | nroff / TeX
Scribe / GML/ SGML /HTML / XML

- XML 기반 프로그램 : RDF/XML, XForms, DocBook, SOAP, WOL(Web Ontology Language) 등
XHTML

- XML 기반 HTML
json
yaml


### Self-closing tag
![](https://velog.velcdn.com/images/minthug94_/post/8c13de7a-7bb2-41de-8163-bed23cff4158/image.png)

```
<img src = "minthug.png"> </img>
<img src = "minthug.png" /> 
```


|태그	 |	설명		 |
|----|------------|
|div|  div 태그는 한줄을 차지한다  | 
|span|   span 태그는 컨텐츠 크기만큼 공간을 차지한다  | 
|img|  img 태그는 이미지 삽입 |
|a|  a태그는 링크 삽입  | 
|ul & li|   ul(un ordered),li 태그는 리스트  | 


-----
# CSS 기초

<span style="background:dimgray; color:yellow">HTML, CSS, JavaScript</span>는 웹 애플리케이션을 만드는 세 가지의 주축입니다. 
CSS는 웹 페이지의 스타일링을 담당!
하지만 CSS는 오직 화려함만을 위해 사용되지는 않는다. 
웹 페이지를 화려하게 꾸미기 전에 먼저 웹 페이지의 구성을 정돈해야 하는데,
이러한 역할도 CSS가 수행한다.

콘텐츠의 배치와 위치 (레이아웃 디자인)
텍스트를 강조하거나 밑줄을 치는 등, 최소한의 타이포그래피 (Typography)
즉, CSS를 통해 화면에 나타나는 정보들의 레이아웃을 최적화함으로써 정보 전달력을 끌어올리며, 컨텐츠의 가독성을 향상시킬 수 있다. 
또한, 색약을 가진 장애인에게 적합하도록 화면을 재구성하거나, 다크 모드 기능을 제공하는 데에도 CSS가 핵심적으로 사용된다. 

<span style="background:dimgray; color:yellow; text-decoration:underline">CSS는 결국 효율적으로 사용자 인터페이스(User Interface, UI)를 구성함으로써 더 나은 사용자 경험(User experience, UX)을 제공하기 위해 사용한다.</span>

## CSS 뜯어보기
![](https://velog.velcdn.com/images/minthug94_/post/1e271bc5-9cdb-4030-925e-4feecdcbfd62/image.png)
<p style="text-align:center; margin: 0px"> [CSS 문법 기본 구성] </p>

### 기본적인 셀렉터(selector)

css 선택자란?
우리가 html 파일을 만들었다면 각각의 태그에 다르게 css 를 설정 할 것입니다. 이 때, 어느 요소에 스타일을 적용할지 알려주는 방식이 바로 css 선택자 입니다.

선택자가 어떻게 쓰이는지 확인해볼까요?

div {     color: black;     background-color: yellow; } 
div 태그들에게 css 를 주기 위해서 div 라는 선택자를 사용하였습니다. 이렇게 되면 html 문서에 모든 div 태그들에는 { } 안에 적용해준 css 속성값들이 적용이 됩니다. div 처럼 태그의 이름 말고도 선택자를 주는 방식이 굉장히 다양한데 이를 알아보도록 하겠습니다.

 

선택자의 종류
 

[ 선택자를 하나만 쓸 경우 ]

 

전체 선택자
전체 선택자는 * 을 사용하여 나타냅니다.
html 의 모든 태그에 대하여 적용합니다.
* { margin: 0 auto; }
태그 선택자
태그 선택자는 태그의 이름 을 사용하여 나타냅니다.
태그명이 선택자와 같은 태그들에 대하여 적용합니다.
p { color: red; }
클래스 선택자
클래스 선택자는 .클래스이름 을 사용하여 나타냅니다.
클래스가 클래스이름과 같은 태그들에 대하여 적용합니다.
.ClassName { width: 100px; }
ID 선택자
ID 선택자는 #아이디이름 을 사용하여 나타냅니다.
ID가 ID 이름과 같은 태그에 대해서 적용합니다.
#IdName { position: fixed; }
 

[ 선택자를 여러 개 쓸 경우]

 

선택자를 여러 개 쓰는 경우를 복합 선택자라고 합니다. 복합 선택자에도 여러 가지 종류가 있어 이에 대해서 알아보겠습니다.

하위 선택자
하위 선택자는 선택자 사이를 공백을 사용하여 나타냅니다.
앞 요소의 자손인 뒷 요소를 선택합니다.
section ul { text-shadow: none; }
자식 선택자
하위 선택자는 선택자 사이를 > 를 사용하여 나타냅니다.
앞 요소의 자식 인 뒷 요소를 선택합니다.
section > ul { text-shadow: none; }





















-----
참고 사이트 :
https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/HTML_basics

https://ssungkang.tistory.com/entry/css-css-%EC%84%A0%ED%83%9D%EC%9E%90selector-%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%EC%98%88%EC%8B%9C

