[# WEB dev
Web site clone coding for WB Developer Conference

Coding Festival: Clone Coding (Final)

1.0 WEB이란? HTTP, TCP통신
	1.1 서버와 클라이언트: HTTP, TCP
	1.2 용어들에 대한 정리: WEB, Code, Source, WEB Site, WEB Page, Domain
	1.3 WEB PAGE: HTML&CSS
	1.4 호스팅

2.0 WEB I: Static Web Page (HTML, CSS)
	1.1 HTML이란?
	1.2 HTML의 쓸모: 예시들
	1.3 준비물: Editor
	1.4 Mark Down 과 다른점
	1.5 Syntax
		1.5.1 Tag란?: <html></html>
		1.5.2 Tag I: h1~h6, strong, u
		1.5.3 기본 구성: !DOCTYPE html, Head, Body
		1.5.4 Tag II: 줄바꿈, 단락, Tag의 응용
		1.5.5 Tag III: Attribute
		1.5.6 Tag IV: Parent & Child, List만들기
	1.6 Resource

3.0 WEB II: Dynamic Web Page (Javascript)
	3.1 Javascript란?
	3.2 Javascript의 쓸모
	3.3 HTML과 CSS와의 차이점
	3.4 Javascript의 원리
	3.5 Javascript의 역할
	3.6 Syntax

5.0 Deploying & management: Github, Opensource
	5.1 Depoloy
	5.2 구름 IDE
	5.3 프론트엔드 서버 Depoly하기
	



















1.0 WEB이란? HTTP, TCP통신
1.1 웹개발에 대해서

	우리가 평소에 자주 접할수있는 여러 서비스들이 만들어지는 근원지이자 밑바탕이다. 용평에서 매일 만나 볼 수 있었던 줌도 웹서비스이고, JD때 과제를 제출하는 이메일도, 그리고 쉽게 정보를 찾을수 있는 구글, 네이버같은 검색엔진들도 웹이라는 세상 안에서 존재한다.
	
	웹이라는 이름에서 알수있듯 웹은 거미줄과 같이 연결되어 있다. 간단히 말하자면 서비스를 제공하는 Server와 그 서비스를 제공 받는 Client가 가장 기본적인 구조이다.
	
	이번 Code Festival에서 배우게 될 html, css, Javascript는 이러한 웹을 구성해주는 가장 기본적인 요소이다.

1.2 용어들에 대한 정리: WEB, WEB Site, WEB Page, Domain

	파이썬이나 자바 관련 수업을 들어본적이 있을것이다. 하지만 우리의 기대와는 달리 검정색 콘솔창에서 숫자나 글자를 띄우는 것 말고는 아무것도 할수가 없었을것이다. 우리가 보는 웹페이지나 앱들도 자바나 파이썬과 같은 언어로 작성되었다는데 이해가 되지 않을것이다. html, css 그리고 Javascript는 이러한 언어들을 시각적으로 변환시켜주는 가장 기본 적인 도구이다. 

	WEB site를 예시로 들어보겠다. WEB site는 한개 또는 여러개의 WEB page로 구성된 하나의 웹 정거장 정도로 이해하면 될것 같다. 우리가 보게 되는 창은 WEB page 이다. 웹페이지는 html으로 작성된다.

	우리가 보는 html파일들은 domain에 연결된 url을 통해 온다. 쉽게말하면 웹사이트가 가지는 링크다. 그 중 메인 링크가 있고, 그 뒤로 여러 웹페이지의 주소가 따라붙게 된다.

1.3 WEB PAGE: HTML&CSS

	html은 Hyper Text Markup Language 즉 텍스트를 조작할수 있게 만들어진 하나의 그림판이라고 보면 된다. 예를 들어보자. 지금 네이버를 접속하면 이렇게 글자만 깨진상태로 나온다. 이게 html이다. 이렇게 깨져서 보이는 이유는 CSS와 JAVA script가 없어서 그렇다.
	
	html로는 글자와 사진 그리고 버튼과 창 정도는 만들수 있지만 색을 칠하고, 구체적으로 객체들을 배치하기에는 한계가 있다. 여기서 CSS와 JAVA script가 아름답게 꾸미고, 내부적인 기능을 구성 할 수 있게 해준다.

1.4 호스팅

	기본적인 web page가 html, css, javascript로 이루어져 있는 것 을 알수있었다. 이제 서버를 베포시켜 모든 사용자들이 사용할수 있도록 하고싶다. 물론 모두가 아닌 같은 인터넷 망을 통해 배포시키는 방법도 있다. 가장 대표적인 예시가 우리학교의 와이파이 로그인창이 될것 같다. 만약 모두가 사용할수있는 공개적인 웹 서비스를 만들고 싶다면 http라는 기술을 사용하게 된다.
	
	다행히도 요즘에는 이런 웹페이지/웹사이트 베포를 쉽게해주는 tool들이 많이 활성화 되어 있다. 간단한 원리를 정리하자면 서버는 “index.html”이라는 웹사이트의 대표 페이지를 먼저 인식한다. index.html은 웹사이트의 모든 웹페이지 중 대표페이지, 즉 홈페이지이다.



2.0 WEB I: Static Web Page (HTML, CSS)

 우리가 따라 만들게될 웹페이지는 정적 웹 페이지 (Static Web Page)이다. 왜 정적 웹 페이지냐면 사용자가 웹페이지와 interect할수 있는 부분이 적기때문이다 정도로 이해해두자

2.1.5 Syntax
2.1.5.1 Tag란?: <html></html>
Tag 란 html의 기본적인 문법이다.
<></>의 형식으로 이루어져있다
반드시 <>로 시작하여 </>로 끝난다
태그의 대상은 태그와 태그 사이에 온다
html 테그는 무조건 전체를 덮고 있어야한다.

2.1.5.2 Tag I: h1~h6, strong, u
<h1>Hello World!</h1>
H1 태그는 문자 크기를 결정하는 태그이다. H1은 태그와 태그 사이에 있는 글자의 크기를 크게 만들어 준다
h1, h2, h3 같이 변형시킬수 있다.
h1부터 h7 까지 존재하며 1이 가장 크고 7이 가장 작다.
Strong 태그는 태그 사이의 글자를 강조표시해준다. 굵음
U태그는 밑줄
대충 이런 원리임

2.1.5.3 기본 구성: !DOCTYPE html, Head, Body…

<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>여기에는 문서의 제목을 입력해주세요</title>
  </head>
  <body>
    여기에 웹페이지에 표시할 콘텐츠(태그)를 입력해주세요
  </body>
</html>

우리가 보는 웹페이지 html은 이러한 구조를 가지고 있다.
<!DOCTYPE html> 은 이 문서가 html파일임을 알려준다.
크게 볼때 그 밑은 <html>로 쌓여져 있다. (우선 lang=”ko”는 설명 x)
그 밑은 head, body로 덮여 있다.
Head는 html문서의 기본적인 정보를 담는다.
예를 들면 html문서가 열리는 브라우저 탭 제목을 바꾸거나, 언어를 바꾸거나, CSS를 곁들일수 있다. 그림판으로 따지면 팔레트와 속성이다.
Body는 말그대로 몸통, 우리가 어떤 요소를 추가하고 싶고 제거하고싶을때 수정할수있는 부분이다. 그림판의 흰색바탕이라고 이해하면 쉽다.


2.1.5.4 Tag II: 줄바꿈, 단락, Tag의 응용

보통 문서를 작성할때 <p>태그를 사용한다. P는 paragraph의 p
P가 둘러쌓여진 태그들은 문단처럼 하나로 나뉘어진다.
Style 속성: <p style="margin-top:45px;">
그럼 이 태그 위쪽 공백이 생긴다. P 태그 이외에도 다른 여러가지 태그에도 이러한 기능이 존재하며, 이러한 기능은 attribute라 불린다, (검색팁: 태그이름 + 속성/attribute) 
이런 속성은 html을 응용하기 위해서는 필수적이다. 꼭 테그별로 자주 사용되는 속성을 알아 두도록 하자.


2.1.5.5 Tag III: Attribute (유용한 태그들과 속성들을 알아보자)
<img>
Img태그는 사진을 가져오는 태그이다. 이 태그는 특이하게도 태그를 닫지 않아도 된다
Img태그에는 src라는 속성이 존재한다. <img src = “이미지 주소”>
Src에는 이미지 위치가 있어야 한다. 예를 들어 (/home/photo/hello-world.jpg 혹은 https://manbangschool.org/2022/images/main-intro-main.jpg)
후자 예시의 경우 다른 웹사이트의 이미지의 주소이다. 그니까 다른 웹사이트의 사진까지 가져와 쓸수있다.
이미지 주소는 index.html이 속해있는 폴더를 기준으로 한다.
width&height: 이 속성들은 이미지의 사이즈를 조절한다.
 
	<img src=”hello-world.jpg” width=”100%” height=”45px”>
	
이때 사이즈를 %, 비율로 표시하게 된다면 전체화면을 기준으로 한 비율로 사이즈가 정해진다. 이로써 유동적인 디자인이 가능하다 ===> 모니터가 크던 작던 폰으로 보던 
이미지가 알아서 커지고 작아짐
만약 여기에  각각 margin을 추가한다면?


<a></a>
A 태그는 하이퍼링크를 만들 수 있도록 해준다.
A 태그의 속성: href, target
Href는 링크를 걸 대상을 의미한다. href=”링크주소”
Target은 링크를 열 방법을 의미한다. target=”링크를 이렇게 이렇게 열어주셈”
	링크를 여는 법)
_self: 지금 보는 페이지에서 열것
_blank: 새탭에서 링크를 열것
_parent: 부모 페이지로 // iframe 태그를 알아야함 = 복잡해짐 깊게 들어가지 말 것
_top: 최상위 페이지로  // iframe 태그를 알아야함 = 복잡해짐 깊게 들어가지 말 것 
	
<div>
     Div 태그는 여러 태그를 묶어 한번에 관리 할 수 있게 해준다. 우리가 평소에 보는 여러 웹서비스의 html문서들을 보면 가장 많이 사용되는 태그이니 주의깊게 알아두어야 한다.
여러 태그를 “묶어”준다. 이외에는 큰 기능이 없다. 그룹화
그림판과 비유하자면 드래그해서 객체를 한번에 다 같이 선택하는것이 되겠다. 

여기에 id속성을 부여할수있다

<body>
  <div id=”study”>
    <p>우와</p>
    <p>HTML 공부보소?</p>
  </div>
  <div id=”Wow~Boso?”>
    <p>슬프고 힘들어요</p>
    <p>올리버썜입ㄴ디ㅏ!</p>
  </div>
</body>


Class속성은 또 다르다. 예제 보고 알잘딱깔센
<body>
  <div id=”study”>
    <p class="text content">우와</p>
    <p class="text content">HTML 공부보소?</p>
  </div>
  <div id=”Wow~Boso?”>
    <p class="text content">슬프고 힘들어요</p>
    <p class="text content">올리버썜입ㄴ디ㅏ!</p>
  </div>
</body>
	
이런 개념들은 나중에 CSS배울때 써먹어야 하므로 알아만 두자. 이 그룹이 어떤 이름을 가진 그룹인지 구분하도록 해준다.

<span>
        Span태그는 라인 기준으로의 요소를 묶는 역할을 한다. 이게 뭔 소리냐면

<body>
  <p>
    안녕하세요?
    저는 <span>올리버 쌤입니다</span> 와 span보소?
  </p>
</body>
	이 태그도 CSS에서 깊게 다룰터이니 개념만
	

참고로 이런 묶어주는 태그에 전역속성을 부여할수있다.
	예시) 
	  <div id=”Wow~Boso?” title=”올리버썜의_감정상태”>
    <p class="text content">슬프고 힘들어요</p>
    <p class="text content">올리버썜입ㄴ디ㅏ!</p>
  </div>



1.5.6 Tag IV: Parent & Child, List만들기
   별거 없다.
<parent>
	<child></child>
</parent>
이 개념임


2.1.6 쓸만한 템플릿 혹은 자료

https://info.cern.ch/hypertext/WWW/TheProject.html (최초의 웹사이트, html만 사용해서 html 배우고 뜯어보도록)

검사버튼을 누르거나, 우클릭을 사용해서 소스 보기 아니면 웹사이트를 저장하면 index.html과 css, javascript를 포함한 소스들을 다운받아볼수 있다.

https://yunbinni.tistory.com/63
https://developer.mozilla.org/en-US/docs/Web/HTML/Element (공식문서)





2.1.7 CSS란?
html을 조금 아름답게 만들어주는 것들
그림판에서 서식, 팔레트에 해당하겠다.





2.1.7.1 CSS의 기본 원리
Css는 html을 꾸며주는 보조도구 이다.
기본적으로 style.css라는 파일명으로 존재할수도 있고(linking style sheet) 
<style></style>태그로 만들 수 있다(internal Style Sheet)
아니면 HTML 태그의 style 속성에 CSS 코드를 넣는다 (inline style sheet)

<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="style.css">                                                                               1번
    <title style="color: blue">여기에는 문서의 제목을 입력해주세요</title>                2번
    <style>
  h1 {
    color: blue;                            3번
  }
</style>
</head>
  <body>
    여기에 웹페이지에 표시할 콘텐츠(태그)를 입력해주세요
  </body>
</html>

이 세가지 옵션중 편한거 선택해서 쓰면 된다. 원하면 중복해서 사용이 가능하다. 그러나 최대한 효율적인 방법을 사용하자


2.1.7.2 태그 지정후 색바꾸기, 효과제거
CSS에서는 태그 통째로 지정하고 효과를 적용할수있다. 다음은 a태그에 대해서 한번에 효과를 적용하는 예시코드이다

a {
	color:yellow;
	text-decoration: none;
}

a태그에 감싸여있던 텍스트가 노랑색 텍스트로 바뀌었다. 하이퍼링크 밑줄은 사라졌다.
이때 모든 description 끝에는 ;이 있어야 한다

inline style형식

    <title style="color: blue;text-decoration: none">여기에는 문서의 제목을 입력해주세요</title>

 Css도 html 처럼 selector와 property 만 알면 거의 다 끝남 

2.1.7.3 선택자 selector
Class
Class는 내가 원하는 부분의 태그에 효과를 적용할때 도움이 된다
먼저 html 태그 안에 속성으로 class=”class이름” 을 지정하고
Css에 불러올때는 .class이름 {} 형식으로 사용하면 된다. (앞에 점 꼭 붙여야함)
하나의 태그가 여러 클래스를 가질수 있다. // class=”background active”
그럼 그 태그는 ‘background’이자 ‘active’클래스인거임
Css에서 각각 따로 호출하여 사용한다.
https://www.youtube.com/watch?v=8-rCMmamtDE 

2.1.7.4 Resource
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
      h1{
        border:5px solid red;
        padding:20px;
        margin:20px;
        display:block;
        width:100px;
      }
    </style>
  </head>
  <body>
    <h1>CSS</h1>
    <h1>CSS</h1>
  </body>
</html>
박스모델





박스모델 쓰는법: https://www.youtube.com/watch?v=4ir8XAf7wxI 

<!doctype html>
<html>
<head>
  <title>WEB - CSS</title>
  <meta charset="utf-8">
  <style>
    body{
      margin:0;
    }
    #active {
      color:red;
    }
    .saw {
      color:gray;
    }
    a {
      color:black;
      text-decoration: none;
    }
    h1 {
      font-size:45px;
      text-align: center;
      border-bottom:1px solid gray;
      margin:0;
      padding:20px;
    }
    ol{
      border-right:1px solid gray;
      width:100px;
      margin:0;
      padding:20px;
    }
  </style>
</head>
<body>
  <h1><a href="index.html">WEB</a></h1>
  <ol>
    <li><a href="1.html" class="saw">HTML</a></li>
    <li><a href="2.html" class="saw" id="active">CSS</a></li>
    <li><a href="3.html">JavaScript</a></li>
  </ol>
  <h2>CSS</h2>
  <p>
    Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the langua
  </body>
  </html>

그리드 쓰는법&써먹기: 
https://www.youtube.com/watch?v=M1eQFIBY2vI 
https://www.youtube.com/watch?v=AL8RSY8rADY 

Source code: https://www.opentutorials.org/course/3086/18322 


https://www.free-css.com/free-css-templates html과 css를 섞은 예시


2.1.7.5 미디어 쿼리와 반응형 디자인

https://www.opentutorials.org/course/3086/18323 
https://www.youtube.com/watch?v=ytl6TrroGis&list=LL&index=34&t=1s 
https://www.youtube.com/watch?v=TlRkmSEMV6w&list=LL&index=36 
https://www.youtube.com/shorts/eZv6kZBfDW0 
https://www.youtube.com/watch?v=JryRu5zby3A 

https://www.youtube.com/watch?v=s8CdkSRnU1k 
https://www.youtube.com/watch?v=CojyGfCMvuU 




Libraries

 위의 내용들을 모두 이해하고, 쓸수있다 하더라도 “어느세월에 다 만들지” 라는 불안감이 들수있다. 걱정하지 않아도 된다. 다른 사람들이 미리 만들어놓은 Library를 사용하면 쉽게 여러 요소들을  구현할수 있게된다.

BootStrap

 웹개발의 가장 대표적인 library이다. 인터넷을 사용해봤다면 bootstrap으로 디자인된 사이트를 한번이상은 봤을것이다. 사용방법은 간단하다. 우선 bootstarp 웹사이트에 들어가 보자.

html head에 
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

	을 붙여넣도록 하자. 이제 사용할 html 페이지에 대한 bootstrap 라이브러리 설치는 끝났다.

Boot strap 사이트로 다시 돌아와서 원하는 요소를 고른다.
css와 함께있는 요소를 원하는 부분에 복사 붙여넣기 한다.
안의 속성을 원하는데로 조절한다.
    <div class="card" style="width: 18rem;">
        <img src="..." class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">Card title</h5>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
      </div>
	
	다음은 카드를 만드는 부트스트렙의 예시이다. 

원리)

	이미 눈치챘을수 있겠지만 태그들의 Class들은 css부분에서 언급되었거나 전혀 사용되지  않았다, 그럼에도 예쁜 모양의 가공된 결과물이 나오는 이유는 바로 위의 설치코드(CDN 설치)에 있다. 바로 bootstrap 서버에 있는 CSS를 가져오는 것 이다. 이  뿐만 아니라 bootstarp에는 버튼, 경고창, 네비게이션바 같은 웹사이트의 기본적인 요소들이 잘 정리되어있고, 쉽게 가져다 쓸수 있다. 꼭 활용할수있도록 하자.


Scroll-out
	
	가끔 어떤 제품에 대한 홍보용으로 만들어진 사이트나 회사의 메인페이지에서 스크롤  하면 반응하며 움직이는 웹사이트를 볼수 있을것이다. 하지만 CSS와 JavaScript 만으로 하나하나 구현하기에는 시간도 많이  걸리고, 원하는 결과물이 나오지 않을 확률이 매우 높다. 이 Scroll-out 라이브러리는 스크롤 에니메이션을 굉장히 쉽게 만들어 준다. 

 <script src="https://unpkg.com/scroll-out/dist/scroll-out.min.js"></script>


	BootStrap과 같이 위 스크립트를 복붙해 cdn설치를 해준다. 참고로 이런 설치방법은 이 두개의 라이브러리 뿐만 아니라  다른 여러 종류의 라이브러리에도 존재한다. 원한다면 쉽게 가져다  쓸수있으니 쉡고 편리한 쓸만한 라이브러리를 찾아보는것도 좋은 웹사이트를 만들어볼수있는 효과적인 방법이라고 할수 있겠다.







사용방법

먼저 아래와 같은 CSS를 복붙해주자
        [data-scroll] {
            opacity: 0;
            will-change: transform, scale, opacity;
            transform: translateY(6rem);
            transition: all 0.5s cubic-bezier(0.165, 0.84, 0.44, 1);


            }


        [data-scroll='in'] {
            opacity: 1;
            transform: translateY(0);


            }


        [data-scroll='out'] {
            opacity: 0;
            }

위 세가지 CSS 파라미터들은 각각 “요소가 화면에 들어오기 전”, “요소가 화면에 들어온 후” , “요소가 화면에서 나간 뒤” 를 의미한다. 나머지는 하나하나 읽어보며 유추해보도록 하자

에니메이션이 적용되기 원하는 그룹을 <section> 테그로 묶고, data-scroll 이라는 atrribute을 추가해준다.
바디 마지막에 script 태그를 열고 
    <script>
        ScrollOut({
        });
    </script>
	을 붙여넣어준다.

이게 끝이다. 정말 쉽고 간단하다. 이와같이 웹사이트를 쉽게 꾸미고, 구현할수있게 해주는 라이브러리가 무수하게 많다. 여러가지를 응용해서 빌드해보는것도 추천한다.



5.0 Deploying & management: Github, Opensource
5.1 Depoloy

 Depoloy를 하기 위해서는 웹서버가 필요하다. 그 웹서버는 여러분의 렙탑이 될수도 있고, 대형 회사에서 쓸법할 커다란 서버 컴퓨터가 될수도 있다. 과거에는 서비스 제공자가 서버까지 같이 구축하는 경우가 많았는데 요즘에는 AWS나 Google Cloud, Microsoft Azure같은 클라우드 서비스로 기업에서 서버를 빌려쓰는 경우가 많다. 이게 더욱 경제적인 이유는 서버를 처음부터 끝까지 구축하는데 있어 복잡한 설치과정과 하드웨어적인 이슈까지, 그리고 효과적인 관리까지 기대할수 있기때문이다.

5.2 구름 IDE

 구름IDE은 온라인에서의 ide도 지원하며 위와같은 클라우드 플랫폼 서비스를 “무료로” 제공한다. 
	
	5.3 프론트엔드 서버 Depoly하기


이용할 개발환경: visual studio, groom ide
Ide 두개 쓰는 이유는 html, css짜기에는 visual studio가 너무 편함
Groom ide는 프레임워크 개발환경 구축, 빌드, 베포, 운영이 편하기에 우선 자바스크립트 전까지는 visual studio로 짜다 마지막 빌드 단계에서 사용할것임
서버문제
중국에서 사용가능
1인 1서버 가능
무료
리눅스
서버관련 자료는 리눅스가 9할 이상이라 이번기회에 리눅스도 잘 익히게 될?수있음
웹앱이 아니니 알빠아니지만 프레임워크설정하기 쉬워서 나중에 유용하게 쓸수있음
 



](https://github.com/notj-code/WBDC_WEBdev/blob/main/README.md)https://github.com/notj-code/WBDC_WEBdev/blob/main/README.md
