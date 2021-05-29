# 바닐라 JS로 크롬 앱 만들기

바닐라 JS로 크롬 앱 만들기(노마드코더) 강의 요약

# Whta is javascript?

- Frontend, 웹에서 쓰이는 유일한 언어

- Javascript의 version - ES5, ES6
  ECMAScript는 Specification의 name
  ES5는 5ECMAScript, ES6는 6ECMAScript을 의미
- Specification란? 체계적인 메뉴얼/안내 책자와 같은 것( 이걸 적으면 브라우저는 이렇게 나와야한 다, 다른 걸 적으면 브라우저는 에러를 띄워야 한다. 등의 내용)

## 바닐라 자바스크립트란?

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

--
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

- 주석 comment :  
  한 줄 → //  
  여러 라인 → /\* 내용 \*/
- 변수를 선언할 때 기본 :  
  처음은 const로 선언, 진짜 필요할 때만 let 쓴다.
- string, boolean(true & false), number, float

## 2. Arrays

Organizing Data with Arrays
우리가 가진 데이터를 어떻게 정렬할까? 2가지 방법이 있다. Array와 Object.

- 문법을 위한 규칙Camel case (낙타 등처럼 울퉁불퉁한 모양)
  : 변수명은 언제나 소문자로 시작하고 중간에 띄어쓰기가 필요하면 그 대신 다음 단어의 첫 글자를 대문자로 쓴다.(∵ 자바스크립트는 변수명에 공백을 쓸 수 없으니)  
  ex) const daysOfWeek = "a"  
  : 스페이스가 없더라도 변수명에 ., /과 같은 문자를 넣으면 안된다.  
  ex) const ./lowerOfWeek (x)

### 1) Array배열

- 리스트처럼 데이터를 저장하는 곳. 여러 데이터를 하나로 묶는다.

```javascript
const mon = "Mon";
const tue = "Tue";
const wed = "Wed";
const thu = "Thu";
const fri = "Fri";

console.log(monday, tue, wed, thu, fri);
```

↑처럼 일일이 선언하면 불편

```javascript
const dayOfWeek = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];

console.log(daysOfWeek);
```

- 출력 할 데이터를 \[ \]\(브라켓\)로 감싸면 된다.  
  안에 들어갈 수 있는 데이터 타입은 텍스트, true/false, numbers, floats, ...등이 있다.

- Array 안의 규칙이 있음: 사람과 다르게 컴퓨터는 0부터 세기 시작한다.  
  ex) 만약 3번째 요일을 알고싶다면  
  console.log(daysOfWeek[2]);

Organizing Data with Objects

2. Object

- Array와 달리 Object에는 각 value에 이름을 줄 수 있다.

만약 A의 개인정보를 저장한다면
const Info= ["A","55", "Seoul", true];  
처럼 배열로 data를 정리하면 어느 순서에 무슨 정보가 있는지 알 수 없다.

- object 를 선언하기 위해서는 { }(중괄호, 컬리브라켓) 을 쓴다. object는 실제 객체를 만드는 것이고 label을 내가 저장하고 싶은 data에주는 것이다.
- ex)

```javascript
const nicoInfo = {
  name: "Nico",
  age: 33,
  gender: "Male",
};

console.log(nicoInfo.gender);
```

출력결과

```
Male
```

- name, age, gender처럼 내가 붙인 데이터의 이름만 사용하는 것이다.
- nicoInfo안의 값, Const안에 있는 값을 (gender) 바꿀 수 있다. 하지만 nicoInfo 자체를 바꿀 수는 없다.

```javascript
const Info = {
  name: "Nico",
  age: 30,
  gender: "Male",
};

Info.gender = "Female";

console.log(Info.gender);
```

출력결과

```
Female
```

## 정리

데이터를 정렬하는 2가지 방법→ Array와 Object

- DB에서 가져온 리스트 데이터라면 Array를 선택.
- 데이터를 합쳐야 한다면 Object 안에 Array를 넣을 수 있다. Array 안에 Object를 넣을 수도 있다.

### 자바스크립트의 기본 문법(규칙)

- **정렬할 데이터와 데이터 사이에는 ,(콤마, Comma)를 반드시 쓴다.**
- 또한, **String(문자열) 쓸 때 "(큰 따옴표, Quotation mark)를 앞 뒤에 반드시 넣는다**.→끝에 "를 안쓰면 다음"가 나올때까지 모두 텍스트로 취급
- console.log와 에러를 읽는다!
