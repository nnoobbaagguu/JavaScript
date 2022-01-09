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

[HTML Event Attributes](https://www.w3schools.com/tags/ref_eventattributes.asp)

<h3>콘솔(Console)</h3>
HTML 파일을 수정하지 않고 콘솔을 이용하여 간단하게 JavaScript 코드를 실행할 수 있다.<br>
Windows 11, Edge 웹 브라우저에서 임의의 웹 페이지를 열고 F12 키를 눌러 DevTools를 실행시킨다. 콘솔 탭을 누르고, JavaScript 코드를 작성하여 실행할 수 있다.<br>
Enter 키를 누르면 바로 실행되고, Shift 키와 Enter 키를 동시에 누르면 코드를 여러 줄 작성할 수 있다.

<h3>JavaScript 데이터 타입 - 숫자, 문자열</h3>

[JavaScript의 타입과 자료구조](https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures)

<h3>변수와 대입연산자</h3>

변수의 선언

```
  var word = "hello";
```

변수의 값은 변할 수 있고 var (변수의 이름)과 같이 선언한다. 대입연산자 = 왼쪽에는 변수가 오고 오른쪽에는 대입할 값이 온다.
