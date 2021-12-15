3. [Javascript 🏃‍♀️](#1-ECMAScript와-JavaScript의-차이)   
    - [1. ECMAScript와 JavaScript의 차이](#1-ECMAScript와-JavaScript의-차이)
    - [2. ES6 이후 바뀐 것](#2-ES6-이후-바뀐-것)
    - [3. var, let, const 차이](3-var,-let,-const-차이)
    - [4. Hoisting](#4-Hoisting)
    - [5. this](5-this)

### 1. ECMAScript와 JavaScript의 차이
<details>
<summary>설명</summary>

-  ECMAScript<br/>
Ecma 인터내셔널에 의해 제정된 ECMA-262 기술 규격에 의해 정의된 범용 스크립트 언어

-  JavaScript<br/>
ECMAScript 사양을 준수하는 범용 스크립팅 언어
</details>

### 2. ES6 이후 바뀐 것
<details>
<summary>설명</summary>

1. let과 const
2. 구조분해 할당(destructuring assignment) - 
    - 배열, 객체의 값들을 추출하여 여러 변수에 할당할 수 있는 기능
3. 화살표 함수(Arrow function) 
    - 기존 함수 표현식에 비해 간결함을 제공
    - 함수를 정의하는 영역의 `this`를 그대로 전달받을 수 있다.
4. 템플릿 리터럴(``)
    - 객체의 속성을 작성할 때 변수명과 동일하다면 생략
    - 백틱으로 시작해서 백틱으로 끝난다.
</details>

### 3. var, let, const 차이
<details>
<summary>설명</summary>

- var

재할당 / 재선언이 가능하다.(프로젝트가 복잡해지면 문제가 발생한다.)

- let

재할당 가능 / 재선언 불가 (보통 반복문에서 많이 사용한다.)

- const 

재할당 / 재선언이 불가하다.

1. 변경이 발생하지 않는(재할당이 필요 없는 상수) 원시 값과 객체에는 const 키워드를 사용한다.
2. const 키워드를 사용하면 의도치 않은 재할당을 방지해 주기 때문에 보다 안전하다.(const 키워드는 재할당을 금지하므로 var, let 보다 안전하다.)
</details>

### 4. Hoisting
<details>
<summary>설명</summary>

함수 안에 있는 선언들을 모두 끌어올려서 해당 함수 유효 범위의 최상단에 선언하는 것을 말한다.
</details>

### 5. this
<details>
<summary>설명</summary>

this의 값은 함수를 호출하는 방법에 의해 결정된다. 실행하는 동안의 할당에 의해 설정될 수 없고, 함수가 호출될 때 마다 다를 수 있다. 
</details>

