# p5.js

생활코딩 모션그래픽을 위한 p5.js tutorial 내용 정리.
https://opentutorials.org/course/4659/30108

p5.js로 할 수 있는 작업 3가지
------------------------
- 정지된 '그림'을 그리는 법을 익힌다.
- 그림을 움직이는 방법(애니메이션)
- 사용자와 '상호작용' 하는 방법

실행; 따라야하는 약속
-----------------------
1. 제일 먼저 실행되어야하는 함수 -> setup함수 안에 코드 작성
(초기화 관련, 한번만 실행될 코드)
2. 애니메이션과 같이 반복적인 실행 필요 -> draw함수 안에 코드를 작성
(반복적으로 실행될 코드)

```js
<html>
  <head>
    <script src="https://cdn.jsdelivr.net/npm/p5@1.3.1/lib/p5.min.js"></script>
  </head>
  <body>
    <script>
      function setup() {
        createCanvas(300, 700);
      }
      function draw() {
        background("cyan");
      }
    </script>
  </body>
</html>
```



그림그리기
-----------------------
그림의 위치를 표시하는 방법?
- 수학 : 좌표평면 이용 -> 숫자로 위치표시    
	가로, 세로 2개의 축이 만나는 곳(0, 0)은 '기준'   
- 모니터의 좌표계 : (0, 0) 은 화면이 시작되는 기준   
( 0 기준 오른쪽 하단 사분면에 모니터가 있다고 생각한다.)  
x축은 수학 좌표평면과 일치(오른쪽으로 갈수록 크고 왼쪽으로 갈수록 작다)  
***y축은 반대(아래로 갈수록 크고 위로 갈수록 작다)  
숫자가 클수록 아래쪽이고 숫자가 작을수록 위쪽

http://p5js.org/ - 레퍼런스 - 도형 - circle() 
예제/설명/문법이 있고 
- 예제- 실행(값 변경)해보며 사용법 추측
- 문법- 정확하게 어떻게 사용하는가 읽어보기
- 원을 그리는 방법 -> circle(x, y, 원의 지름)


애니메이션
-----------------------
- setup 함수가 실행된 이후 실행되는 draw함수 사용
- random함수의 활용 -> 역동적인 애니메이션 가능
- 이동하는 그림 표현방법
1. setup 함수에 x, y의 초기 위치 값을 주고
x = 0;
y = 0;
2. draw 함수에 x, y가 이동하도록 값을 더해준다
x = x + 10;
y = y + 5;

변수 windowWidth, windowHeight : canvas 전체를 채울 수 있다. 


참고 도서, 사이트
--------------------
- khanacademy.org/computing  
- 'nature of code'  
국내 번역본 (Processing, java)  
natureofcode.com 
강의 https://www.youtube.com/watch?v=70MQ-FugwbI (2020년에 js로 변경) 
