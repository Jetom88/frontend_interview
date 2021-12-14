# frontend_interview 🎤

1. [CS 💻 ](#RESTful이란?)   
    - [1. RESTful이란?](#RESTful이란?)   
    - [2. RESTful하다?](#RESTful하다?)
    - [3. Restful API와 GraphQL 차이점](#Restful-API와-GraphQL-차이점)
    - [4. CORS](#CORS)
    - [5. URL?](#URL?)
    - [6. HTTP / HTTPS?](#HTTP-/-HTTPS?)
    - [7. JWT?](#JWT?)
    - [8. 브라우저의 작동원리](#브라우저의-작동원리)
    - [9. 렌더링 엔진](#렌더링-엔진)

### 1. RESTful이란?
<details>
<summary>설명</summary>
REST(REpresentational State Transfer)ful API는 HTTP 통신에서 어떤 차원에 대한 CRUD 요청을 Resource와 Method로 표현하여 특정한 형태로 전달하는 방식<br/>
<br/>
RESTful API는 아래와 같다.<br/>
- Resource(자원, URI)<br/>
- Method(요청 방식, GET or POST 등)<br/>
- Representation of Resource(자원의 형태, JSON or XML 등)

---

**CRUD Operation**<br/>
1. Create : 생성(POST)<br/>
2. Read : 조회(GET)<br/>
3. Update : 수정(PUT)<br/>
4. Delete : 삭제(DELETE)<br/>
5. HEAD: header 정보 조회(HEAD)
</details>

### 2. RESTful하다?

<details>
<summary>설명</summary>
많은 API 개발자들은 RESTful한 API란, ‘각 구성요소들의 역할이 완벽하게 분리되어 있는 것’ 이라고 한다. URI는 각 리소스(자원)를 명확하게 인식할 수 있도록 용이한 표현방식을 가져야 하며, 각 리소스에 대한 행위(메소드)를 HTTP 메소드를 이용하여 Uniform(일관성)하게 정의할 수 있어야 한다. 
</details>

### 3. Restful API와 GraphQL 차이점

<details>
<summary>설명</summary>
RESTful API 는 Resource 마다 하나의 Endpoint 를 가지고, 그 Endpoint 에서 그 Resource 에 대한 거의 모든 것을 담당한다. 반면, GraphQL 은 전체 API 를 위해서 단 하나의 Endpoint 만을 사용한다. <br/>
<br/>
Restful API 는 하나의 Endpoint 에서 돌려줄 수 있는 응답의 구조가 정해져 있는 경우가 많다. 반면, GraphQL 은 사용자가 응답의 구조를 자신이 원하는 방식으로 바꿀 수 있다.

---
**GraphQL?**

GraphQL 은 Graph Query Language 의 줄임말이다.

GraphQL 은 Query Language 중에서도 **Server API 를 통해 정보를 주고받기 위해 사용하는 Query Language** 이다.

```
Restful API 로는 다양한 기종에서 필요한 정보들을 일일히 구현하는 것이 힘들었다. 
예를 들어 IOS 와 Android 에서 필요한 정보들이 조금씩 달랐고, 그 다른 부분마다 API를 구현하는 것이 힘들었다.
```

</details>

### 4. CORS

<details><summary>설명
</summary>

Cross-Origin Resource Sharing(CORS)은 추가적인 HTTP header를 사용해서 애플리케이션이 다른 origin의 리소스에 접근할 수 있도록 하는 메커니즘을 말 한다. 하지만 다른 origin에서 내 리소스에 함부로 접근하지 못하게 하기 위해 사용된다.

</details>

### 5. URL?

<details><summary>설명
</summary>

네트워크 상에서 자원이 어디 있는지를 알려주기 위한 규약 

![url](https://user-images.githubusercontent.com/64053930/145674613-3725786d-dd58-402c-9d94-4310f0bf370c.png)<br/>
(이미지 출처: https://beomy.github.io/tech/browser/cors/)
</details>

### 6. HTTP / HTTPS?

<details><summary>설명
</summary>

- http?<br/>
    서버/클라이언트 모델을 따라 데이터를 주고 받기 위한 프로토콜
    
- https?<br/>
    HTTP에 데이터 암호화가 추가된 프로토콜

</details>

### 7. JWT?

<details><summary>설명
</summary>

선택적 서명 및 선택적 암호화를 사용하여 데이터를 만들기 위한 인터넷 표준으로, 페이로드는 몇몇 클레임(claim) 표명(assert)을 처리하는 JSON을 보관하고 있다. 토큰은 비공개 시크릿 키 또는 공개/비공개 키를 사용하여 서명된다.

JSON 객체를 사용해 입장권을 발급해준다고 생각하면 된다.

</details>

### 8. 브라우저의 작동원리

<details><summary>설명
</summary>

웹 브라우저가 웹 서버에 필요한 자원(웹 페이지)을 요청하면 서버는 응답하고 웹 브라우저는 이를 해석한 후 사용자(Client)에게 보여준다. 보통 자원은 HTML 문서지만 PDF, 이미지 등 다양한 형태일 수 있다.

![image](https://user-images.githubusercontent.com/64053930/145927721-8f12b961-f1c7-4a5f-8732-8b6974e3fed8.png)
(이미지 출처: https://d2.naver.com/helloworld/59361)

</details>

### 9. 렌더링 엔진

<details><summary>설명
</summary>

> 렌더링 엔진은 HTML, XML, 이미지 등 요청받은 내용을 브라우저 화면에 표시하는 엔진

각 브라우저마다 렌더링 엔진이 다르기 때문에 같은 페이지가 다르게 보이는 경우가 있다.


```
-moz-border-radius: 1em; // 파이어폭스 브라우저에 적용
-ms-border-radius: 2em; // 익스플로어에 적용, 보통 생략
-o-border-radius: 3em; // 오페라에 적용
-webkit-border-radius: 4em; // 구글, 사파리 브라우저에 적용
```

렌더링 엔진의 종류는 아래와 같다.

- Blink - 크롬, 오페라
- Webkit - 사파리
- Trident - 익스플로어
-  EdgeHTML - 마이크로소프트 엣지

*Blink는 구글이 Webkit을 대체하기 위해 자체적으로 개발한 엔진*

렌더링 엔진은 좀 더 나은 사용자 경험을 위해 가능하면 빠르게 내용을 표시그래서 일련의 과정들이 동기적으로 진행되지 않습니다. HTML을 파싱 할 때까지 기다리지 않고 렌더 트리 배치와 그리기 과정을 시작
</details>
