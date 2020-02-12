
## Redux
<br>

**Redux**
"Redux"는 react-native를 개발하는데 좋은 아키텍쳐 패턴
<br>
<br>

**아키텍쳐 패턴이 생겨난 과정**
리엑티브(Reactive eXtension) 패러다임은 마이크로소프트가 창안한 개념
<br>
"데이터 흐름에 따른 변화를 만드는 비동기적 프로그래밍 패러다임"
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

**Dom?** ; Document Object Model
<br>
* A method of expressing structured documents through objects, written in HTML.
* Web browsers use DOM to apply javascript and CSS to objects.
<br>
<br>

**Hooks rule?**
<br>

1. It must be written at the top of the react function.
- Do not use within conditional statements, internal functions, or repeating statements.

2. Use only within the react function.
- Exceptional call within the custom function
<br>

ex)
```
const [name, setName] = useState("");

useEffect(()=>{

document.title = `search search search my ${name}`;

});
```
<br>
