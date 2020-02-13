## Context


* 전역적인 상태 관리

![캡처](https://user-images.githubusercontent.com/58720791/74316662-4f21e300-4dbd-11ea-8b3d-b7b4d1ede7ab.PNG)<br>

Root 컴포넌트의 state에는 value라는 값이 있고, 이 값을 변경시키는 handleSetValue라는 함수가 있다고 가정하자.<br>
value라는 값은 컴포넌트 F, J에서 보여주고 있고 이 값을 변화시키는 이벤트는 컴포넌트 G에서 발생.<br>
<br>
value값 : Root -> A -> B -> F, Root -> H -> J<br>
handleSetValue값 : Root -> A -> B -> E -> G<br>
<br>
의 형태로 value값과 handleSetValue함수를 props로 하위 컴포넌트에게 전달해주게됨.<br>
<br>
실제 프로젝트에서 컴포넌트의 깊이가 더욱 깊을 수 있고 데이터들이 훨씬 많아질 수 있어 유지보수성이 낮아질 가능성 존재.<br>
<br>
---> Redux나 MobX 같은 라이브러리를 사용.<br>
<br>
하지만 기존 Context API가 더욱 좋아짐.<br>



![캡처2](https://user-images.githubusercontent.com/58720791/74316667-50531000-4dbd-11ea-870c-df32e9f9bb46.PNG)<br>

더 이상 여러 컴포넌트를 거쳐 값을 전달해주는 것이 아니라 Context를 통해서 원하는 값이나 함수를 바로 쏴줄 수 있게 함.
<br>
<br>
## Using Context

* Context는 createContext라는 함수를 사용해서 만들고 이 함수를 호출하면 Provider과 Consumer라는 컴포넌트들이 반환됨.<br>

```
import React, { createContext } from 'react';

const Context = createContext();
const { Provider, Consumer: CounterConsumer } = Context;
```
* 
