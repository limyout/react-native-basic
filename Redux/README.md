
## Flux / Redux
<br>

**Redux**
"Redux"는 react-native를 개발하는데 좋은 아키텍쳐 패턴
<br>
<br>

**아키텍쳐 패턴이 생겨난 과정**
<br>
리엑티브(Reactive eXtension) 패러다임은 마이크로소프트가 창안한 개념
<br>
**데이터 흐름에 따른 변화를 만드는 비동기적 프로그래밍 패러다임"**
<br>
* RxAndroid
* RxJava
* ReactiveCorcoa
* React
* React Native
* 그 외
<br>
이렇게 확장되어가는 중
<br>
React -> React native
Flux design pattern -> Redux design pattern
<br>
으로 확장
<br>
<br>

**Flux?**
<br>
앱의 상태값들이 store에 유지가 되고, 이벤트가 발생하면 dispatcher을 통해 action이 상태를 변화시킴.<br>
상태 변경을 listening 하고 있다가 변경되면 View는 다시 렌더링 함.
<br>
<br>

**Redux?**
<br>
앱의 상태 모두를 하나의 store안에 트리 구조로 저장.<br>
![캡처](https://user-images.githubusercontent.com/58720791/74312489-239afa80-4db5-11ea-9423-9b262d2149c5.PNG)<br>
store은 전체 상태의 구조 유지를 위해 두 가지 생성.<br>
* reducer ; 변화시킬 데이터 구조를 가지고 있음
* middleware ; 추가로 필요한 상태 트리구조 정보 또는 기타 변화시키는 역할을 담당
<br>
<br>

action이 store을 변경<br>
![캡처2](https://user-images.githubusercontent.com/58720791/74312492-24cc2780-4db5-11ea-9f74-9567c2c0464b.PNG)
* action은 state의 변화를 이끌어 내기위해 정의 되어있는 종류(타입)들
<br>
<br>

action이 어떻게 변경시켜야 하는지 reducer이 정의<br>
![캡처3](https://user-images.githubusercontent.com/58720791/74312494-24cc2780-4db5-11ea-81e6-ed84dd6d4881.PNG)
<br>
<br>

View가 변화될 데이터를 구독하고, 변화시킬 action을 dispatch 하는 것을 바인딩함.<br>
![캡처4](https://user-images.githubusercontent.com/58720791/74312496-2564be00-4db5-11ea-8e2b-d98d355d8755.PNG)
<br>
<br>

container은 store의 상태값이 변화되는지 subscrib, subscript하고 있는데 redux에서는 props에 담아 넘겨줌.<br>
![캡처5](https://user-images.githubusercontent.com/58720791/74312499-25fd5480-4db5-11ea-9d84-647c3386d619.PNG)
<br>
<br>

container의 화면에서는 사용하기 위해 props를 state에 map하는 과정이 진행.<br>
![캡처6](https://user-images.githubusercontent.com/58720791/74312501-2695eb00-4db5-11ea-8be9-907e1fc1542e.PNG)
<br>
<br>

화면의 mainthread runloop에서 클릭 등 이벤트가 발생해서 변경 요청을 하면 container에서 action을 보냄<br> -> dispatch action이라 함.<br>
![캡처7](https://user-images.githubusercontent.com/58720791/74312503-272e8180-4db5-11ea-831f-ee463a6a7c49.PNG)
<br>
<br>

state를 변경하기 위해 비동기 처리를 하는 경우(네트워크 처리)를 위해 action과 reducer 사이에 middleware를 둠.(ex thunk, saga, etc...)<br>
![캡처8](https://user-images.githubusercontent.com/58720791/74312505-272e8180-4db5-11ea-84bf-9830761fd8fb.PNG)
<br>
<br>





