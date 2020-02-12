## Context


* 전역적인 상태 관리

![캡처](https://user-images.githubusercontent.com/58720791/74316662-4f21e300-4dbd-11ea-8b3d-b7b4d1ede7ab.PNG)<br>

Root 컴포넌트의 state에는 value라는 값이 있고, 이 값을 변경시키는 handleSetValue라는 함수가 있다고 가정하자.<br>
value라는 값은 컴포넌트 F, J에서 보여주고 있고 이 값을 변화시키는 이벤트는 컴포넌트 G에서 발생.<br>
<br>
value값 : Root -> A -> B -> F, Root -> H -> J<br>
handleSetValue값 : Root -> A -> B -> E -> G<br>
<br>
의 형태로 value값과 handleSetValue함수를 props로 하위 컴포넌트엑 전달해주게됨.


![캡처2](https://user-images.githubusercontent.com/58720791/74316667-50531000-4dbd-11ea-870c-df32e9f9bb46.PNG)
