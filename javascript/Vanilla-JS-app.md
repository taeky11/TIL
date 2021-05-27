# 바닐라 JS로 크롬 앱 만들기

바닐라 JS로 크롬 앱 만들기(노마드코더) 강의 요약

# Whta is javascript?

- Frontend, 웹에서 쓰이는 유일한 언어

- Javascript의 version - ES5, ES6
  ECMAScript는 Specification의 name
  ES5는 5ECMAScript, ES6는 6ECMAScript을 의미
- Specification란? 체계적인 메뉴얼/안내 책자와 같은 것( 이걸 적으면 브라우저는 이렇게 나와야한 다, 다른 걸 적으면 브라우저는 에러를 띄워야 한다. 등의 내용)

### 바닐라 자바스크립트란?

JavaScript의 한 종류, Library가 없는 것
브라우저를 통해 우리에게 제공된 JavaScript.

- 정리: JavaScript는 언어, ECMAScript는 Specification.

- 바닐라 자바스크립트는 쌩얼,
  Library, Framework는 메이크업, 화장과 같음. 자바스크립트를 원래보다 조금 더 예쁘게 만들어준다.

- Vanilla JavaScript를 배워야하는 이유?
  ex. 포토샵 툴(SW)은 다룰 수 있지만 사진은 못찍는 경우(색감, 구도에 대한 이해나 감각/ 퀄리티에 대한 기준이 없는 경우) = JavaScript를 제대로 모르고 사용하는 경우와 같다.
- Vanilla JavaScript를 배우는 것 = 웹에서의 기초가 되는 언어를 배우는 것과 같음.
- 답답한 면이 있지만 웹 상에서 본 모든 것들은 이 언어로 구성되어있고 강력하다.

# What are we learning?

What you learn is a concept. 모든 언어에서 동일하게 담고 있는 개념. ex)function, variable, 그 외 조건, event, class, objects, arrays..

프로그래밍 언어는 따라야하는 규칙과 문법이 있다.

- javascript로 작성된 의미있는 한 줄을 Expressions이고 하고 ;(세미콜론)으로 마친다. ex) console.log(a);

## 1. Variable 변수

- 변하는 값을 담는 그릇
- 변수는 선언, 초기화, 값을 업데이트(수정) 하는 과정으로 사용
- let : 변수를 초기화하거나 생성(선언=저장 공간을 만듦) 할 때 쓴다.
  ex) let a = 5;
- 변수를 수정(업데이트) 할 때는 let 쓰지 않는다. ex) a = 4;
- JavaScript는 코드를 위에서 아래로 실행. ∴ 제일 마지막에 저장된 값이 출력된다.

- let, const, var  
   let 과 const
  let, var : 값이 바뀌는 것 허용
  const : 상수. (변하지 않는 값) 값이 바뀌는 것을 허용하지 않음

### 변수에 넣을 수 있는 data의 종류(data type on JS)

- 주석 comment : 한 줄 → //, 여러 라인 → /_ 내용 _/
- 변수를 선언할 때 기본: 처음은 const로 선언, 진짜 필요할 때만 let 쓴다.
- string, boolean(true & false), number, float
