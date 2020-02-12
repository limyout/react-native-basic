## AsyncStorage


* Using Promise

```
const makeGetRequest = () =>
 getJSON().then(response => {
 console.log(response); // this will log JSON data
 return "done";
});
 
makeGetRequest();
```

 

* Using async/await

```
const makeGetRequest = async () => {
 console.log(await getJSON()); // this will log response/JSON data
 return "done";
};
 
makeGetRequest();
```
<br>
위 함수는 앞에 'async'라는 키워드가 있다. await 키워드는 비동기식으로 정의된 기능 내에서만 사용할 수 있다. 'await getJSON()'은 getJSON() promise가 결정되어 그 값 출력할 때까지 'console.log' 호출이 기다린다는 것을 의미한다.
