2. [frontend 👩‍💻](#1-SSR?-CSR?)   
    - [1. SSR? CSR?](#1-SSR?-CSR?)
    - [2. SPA](#2-SPA)
    - [3. 크로스브라우징](3-크로스브라우징)

### 1. SSR? CSR?
<details>
<summary>설명</summary>

- SSR(Server Side Rendering)

`브라우저`=>`프론트 서버`=>`백엔드 서버`=>`데이터베이스` 를 거쳐 데이터베이스에서 데이터를 가져온 후 다시 브라우저에 데이터가 그려지는 형식

클라이언트가 페이지를 이동한다든가, 클릭으로 인한 다른 요청이 생길때마다 이 과정을 반복하기 때문에 화면에서 바뀌지 않아도 되는 부분도 계속해서 다시 렌더링되는 단점이 있다. 이는 곧 서버 부하 등의 문제를 일으킬 수 있다.

- CSR(Client Side Rendering)

CSR은 react, vue 등의 SPA(Single Page Application)에서 쓰이는 기법으로, 서버에서 화면을 구성했던 SSR 방식과 달리 클라이언트에서 화면을 구성한다.
화면을 그리는 코드는 다운받았지만 아직 데이터를 다운 받은 상태가 아니다. CSR의 경우 클라이언트의 요청이 발생하면 필요한 데이터만 백엔드 서버에 요청하여 데이터만 받아온다.
</details>

### 2. SPA
<details>
<summary>설명</summary>

SPA(Single Page Application)는 한 개(Single)의 Page로 구성된 Application이다.

- 장점

필요한 부분만 갱신하기 때문에 네이티브 앱에 가까운 자연스러운 페이지 이동과 사용자 경험(UX)을 제공할 수 있다.(웹앱)

- 단점
1. javaScript 파일을 번들링해서 한 번에 받기 때문에 초기 구동 속도가 느리다.
1. 검색엔진최적화(SEO)가 어려움

</details>

### 3. 크로스브라우징
<details>
<summary>설명</summary>
웹 페이지 제작 시에 모든 브라우저에서 깨지지 않고 의도한 대로 올바르게(호환성) 나오게 하는 작업을 말한다.
</details>

