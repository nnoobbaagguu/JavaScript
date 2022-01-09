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
<body>
  <script>
    document.write('hello, world!');
  </script>
</body>
```

<h3>이벤트(Event)</h3>
웹 브라우저에서 일어나는 사건들을 이벤트(event)라고 한다.<br>
이벤트를 통해 사용자의 동작을 감지하여 사용자와 웹은 이벤트를 통해 상호작용한다.<br>
이벤트를 통해서 JavaScript 코드를 실행할 수 있다.<br>
onclick 사용자가 어떤 것을 클릭하는 사건<br>
onchange 사용자가 입력하여 어떤 것의 내용을 바꾸는 사건<br>
onkeydown 사용자가 키보드를 누르는 사건<br>

```
<input type="button" value="hi" onclick="alert('hi')">
<input type="button" value="hi" onclick="alert('hi')">
<input type="button" value="hi" onclick="alert('hi')">
```

# 콘솔(Console)
이미 만들어진 웹 페이지에 콘솔 창을 띄워 JavaScript 코드를 작성하여 문제를 해결할 수 있다.
