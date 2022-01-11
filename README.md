<h1>JavaScript</h1>

[자바스크립트의 시작](https://www.boostcourse.org/cs124)<br>

<h2>1. 웹과 JavaScript</h2>

<h3> WEB과 JavaScript, HTML</h3>

HTML -> 정적(한번 화면에 출력되면 그 모습 그대로 유지됨)<br>
사용자와 동적으로 상호작용하는 웹페이지를 만들기 위한 기술 -> JavaScript<br>
=>HTML으로 만들어진 웹 페이지를 JavaScript를 이용하여 사용자와 상호작용할 수 있도록 기능을 추가<br>

<h3>JavaScript의 역할</h3>

JavaScript는 HTML을 제어하여 사용자와 상호작용하는 언어이다.<br>
웹 페이지는 한 번 출력되면 바뀔 수 없지만, Javascript 코드에 따라서 style 속성이 추가되면서 웹 페이지가 동적으로 변화함.<br>

<h3>서로 다른 언어인 HTML와 JavaScript의 상호작용</h3>

\<script>\</script><br>
script 태그 내부에 JavaScript 코드를 작성한다.<br>

```
<script>
  document.write('hello, world!');
</script>
```

<h3>이벤트(Event)</h3>

웹 브라우저에서 일어나는 사건들을 이벤트(event)라고 한다.<br>
이벤트를 통해 사용자의 동작을 감지하여 사용자와 웹은 이벤트를 통해 상호작용한다.<br>
이벤트를 통해서 JavaScript 코드를 실행할 수 있다.<br>
이벤트는 HTML 태그의 속성이며, JavaScript 코드값을 가진다.<br><br>

onclick 사용자가 어떤 것을 클릭하는 사건<br>
onchange 사용자가 입력하여 어떤 것의 내용을 바꾸는 사건<br>
onkeydown 사용자가 키보드를 누르는 사건<br>

```
<input type="button" value="hi" onclick="alert('hi')"> // alert('hi')는 JavaScript 코드이다.
<input type="button" value="hi" onclick="alert('hi')">
<input type="button" value="hi" onclick="alert('hi')">
```

[HTML Event Attributes](https://www.w3schools.com/tags/ref_eventattributes.asp)<br>

<h3>콘솔(Console)</h3>

HTML 파일을 수정하지 않고 콘솔을 이용하여 간단하게 JavaScript 코드를 실행할 수 있다.<br>
Windows 11, Edge 웹 브라우저에서 임의의 웹 페이지를 열고 F12 키를 눌러 DevTools를 실행시킨다. 콘솔 탭을 누르고, JavaScript 코드를 작성하여 실행할 수 있다.<br>
Enter 키를 누르면 바로 실행되고, Shift 키와 Enter 키를 동시에 누르면 코드를 여러 줄 작성할 수 있다.<br>

<h3>JavaScript 데이터 타입 - 숫자, 문자열</h3>

[JavaScript의 타입과 자료구조](https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures)<br>

<h3>변수와 대입연산자</h3>

변수의 선언<br>

```
  var word = "hello";
```

변수의 값은 변할 수 있고 var (변수의 이름)과 같이 선언한다. 대입연산자 = 왼쪽에는 변수가 오고 오른쪽에는 대입할 값이 온다.<br>

<h3>JavaScript를 통한 웹 브라우저의 제어</h3>

HTML은 정적인 언어이다. 하지만 JavaScript를 통해 HTML 태그의 style 속성을 변경하여 출력되는 웹 페이지의 내용을 동적으로 변경할 수 있다.<br>
HTML 태그의 style 속성은 CSS 언어로 작성된 코드의 값을 갖는다.<br>
CSS 언어를 이용하면 웹 페이지에 출력되는 디자인을 변경할 수 있다.<br>

<h3>CSS 기초</h3>

<h4>style 속성</h4>

```
  <h1 style="color: blue">Javascript<h1>
```

color: blue 코드가 CSS 코드이다.<br>

<h4>style 태그</h4>

\<div>\</div>, \<span>\</span> 태그<br>
다른 기능이 없고, CSS나 JavaScript 코드를 삽입하기 위한 태그이다.<br>
div 태그는 화면 전체를 사용하기 때문에 줄바꿈이 되고, span은 줄바꿈이 되지 않는다.<br>
div나 span 태그를 만들어 style 속성을 부여하면 이 태그로 감싸진 부분에 디자인이 적용된다.<br><br>

하지만 각 코드에 일일히 div나 span 태그를 사용하여 CSS 코드를 작성하거나, CSS 코드를 수정하는 것은 매우 번거롭다.<br>
따라서 \<head>\</head> 태그 내부에 \<style>\</style> 태그를 만들고 style 태그 내부에 CSS 코드를 작성한다.

<h4>style 태그와 선택자</h4>

style 태그에 CSS 코드를 작성하기 위해서는, CSS 코드를 작성할 태그들을 선택해야한다.<br>
태그에 새로운 속성을 부여해서 그룹짓고, 그룹화한 태그들 중에서 필요한 태그를 선택하면된다.<br>
태그를 그룹화하는 방법에는 id, class, 그리고 태그 그 자체가 있다.<br>

```
<head>
<style>
  .js {
    color: red;
  }
  #first {
    color: blue;
  }
  span {
    color: green;
  }
</style>
<\head>
<body>
  <span class="js">JavaScript</span><br>
  <span id="first" class="js">JavaScript</span><br>
<\body>
```

style 태그 내부에 id의 이름 앞에는 #을 붙이고, class의 이름 앞에는 .를 붙인다. 태그 이름의 경우에는 그대로 작성하면 된다.<br>
중괄호 내부에는 JavaScript 코드를 작성한다.<br><br>

class는 그룹을 의미하고 id는 특정한 것을 식별하는 것을 의미한다. 따라서 class는 중복하여 여러개의 태그에 적용할 수 있지만 id는 단 하나의 태그에만 사용된다. class 선택자가 id 선택자보다 더 포괄적이고 광범위하다.<br><br>

선택자의 우선순위는 id > class > 태그 이다.<br>

<h3>JavaScript로 제어할 태그 선택하기</h3>

<h4>querySelector 함수</h4>

querySelector 함수를 이용하여 원하는 태그를 선택한다.

```
document.querySelector("body");
document.querySelector(".js");
document.querySelector("$first");
```

<h2>JavaScript 제어문</h2>

<h3> 프로그램, 프로그래밍, 프로그래머와 JavaScript와 HTML의 차이</h3>

<p>HTML과 JavaScript는 모두 컴퓨터 언어이지만, JavaScript는 HTML과 다르게 컴퓨터 프로그래밍 언어이기도 하다.<br>
그러면 프로그래밍, 프로그램은 무엇일까?<br>
프로그램에는 순서라는 의미가 있다. 프로그래밍은 이런 순서를 만드는 행위를 말하고, 프로그래머는 프로그래밍, 이런 순서를 만드는 행위를 하는 사람을 의미한다.<br>
컴퓨터 프로그래밍 언어는 컴퓨터에 순서를 만들어 주는 언어, 즉 시간의 순서에 따라 실행되어야 할 기능을 글로 적어두는 방식을 의미한다.</p>

<p>그러면 HTML과 달리 JavaScript가 프로그래밍 언어인 이유는 무엇일까?<br>
HTML로 만든 웹 페이지는 시간의 순서에 따라 실행되지 않고, 한 번 만들어지면 바뀌지 않는다. 따라서 컴퓨터 프로그래밍 언어가 아니다.<br>
반면, JavaScript는 사용자와 상호작용하고, 이를 위해 시간에 따라 여러가지 기능들이 실행되어야 하기 때문에 프로그래밍의 형태를 띈다. 따라서 JavaScript는 컴퓨터 프로그래밍 언어라고 할 수 있다.</p>

<p>[생각해보기] 이번 강의에서 HTML과는 달리 Javascript는 컴퓨터 프로그래밍 언어라는 것을 배웠습니다. 오늘 배운 내용을 바탕으로 HTML은 왜 프로그래밍 언어가 아닌지 스스로에게 설명해봅시다.<br>
HTML로 만든 웹 페이지는 정적이며 시간의 순서에 따라 실행되거나 변화하는 흐름이 없다. 따라서 프로그래밍 언어라고 할 수 없다.</p>

<h3>조건문</h3>

<p>조건문은 프로그램이 조건에 따라서 다른 기능들이 다른 순서에 따라 실행되도록 만들어 주는 것이다.</p>

<p>[생각해보기] 조건문이 필요한 이유가 무엇일까요? 조건문을 사용하면 어떤 점이 더 편리할까요? 예시를 들어서 생각해봅시다.<br>
현재 상태에 따라서 다른 기능이 수행되어야 할 때 조건문이 필요하다. 혹은 현재 상태에서는 어떤 기능이 수행될 필요가 없을 경우 컴퓨터의 자원을 절약할 수 있다.</p>

<h4>비교 연산자와 Boolean</h4>

<p>비교연산자에는 일단 ===, <, >가 있다. 이 연산자들은 모두 이항 연산자이다.<br>
===는 비교 연산자라고 부르며, 왼쪽의 피연산자와 오른쪽의 피연산자가 같은지 판단한다. 두 값이 같으면 true를 반환하고, 두 값이 다르면 false를 반환한다.<br>
<, >는 두 값의 크기를 비교하는 연산자이다. HTML에서는 이 기호가 태그를 표현할 때 사용되므로 다른 표기를 사용한다. JavaScript 코드를 작성할 때는 <, >를 그대로 사용해도 된다. </p>

```
&lt // less than, <을 의미한다.
&gt // greater than, >을 의미한다.
```

비교 연산자가 반환하는 true, false 값을 Boolean 데이터 타입이라고 한다. Boolean 데이터 타입에는 true 아니면 false 두 가지의 값만 존재한다.

<p>[생각해보기 1] Javascript에서 '왼쪽이 오른쪽보다 크거나 같다'를 표현하기 위해서는 어떻게 비교 연산자를 사용하면 좋을까요? (힌트: javascript bigger than or equal to 라고 검색해보세요!)<br>
  </p>
  
