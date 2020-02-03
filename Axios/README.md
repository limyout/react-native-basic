## Axios


* promise API 지원

  - 여기서 promise란 자바스크립트 비동기 처리에 사용되는 객체입니다. 또 자바스크립트의 비동기 처리란 ‘특정 코드의 실행이 완료될 때까지 기다리지 않고 다음 코드를 먼저 수행하는 자바스크립트의 특성’을 의미합니다. 즉 axios는 비동기 통신을 지원합니다.

 

* json 데이터로 자동변환

  - Axios는 요청을 보낼 때 자동으로 데이터를 문자열 화합니다. 그러나 Fetch()를 사용할 때는 수동으로 수행해야 합니다. 

 

* 광범위한 브라우저

  - Axois는 오래된 브라우저에서 아무런 문제 없이 실행할 수 있습니다. 반면에 Fetch()는 polyfill을 수동 설치하여 비슷한 기능을 구현할 수 있습니다.

 

* 응답 시간 초과 설정

  - Axios에서는 config 객체의 optional 속성을 사용하여 요청이 중단되기 전의 시간 (밀리 초)을 설정할 수 있습니다. Fetch()는 AbortController 인터페이스를 통해 유사한 기능을 제공합니다. 그러나 Axios만큼 간단하지는 않습니다.

 

* 동시 요청

  - Axios는 axios.all() 사용하여 동시 요청을 기능을 제공합니다.

 
<br>
<br>
결론적으로 Axios는 대부분의 HTTP 통신 요구에 맞는 적절한 패키지로 사용하기 쉬운 API를 제공합니다. 하지만 fetch API도 facebook에서 기본적으로 쉽게 사용하기 위한 통신 API므로 사용자의 상황과 선호에 따라 무엇을 사용할지 정하면 좋을 것 같습니다. 
<br>
<br>

## installation
```
yarn add axios
```

or

```
npm install axios
```
<br>

## Project

![1](https://user-images.githubusercontent.com/58720791/73621315-0198ce00-4679-11ea-9ac6-c99fe6d2b119.PNG)
<br>

<br>

![2](https://user-images.githubusercontent.com/58720791/73621317-02316480-4679-11ea-9b30-d7c42874c924.PNG)
<br>

<br>

![3](https://user-images.githubusercontent.com/58720791/73621318-02316480-4679-11ea-8c15-bf2728592ec7.PNG)
<br>
<br>

## Project result

![1](https://user-images.githubusercontent.com/58720791/73632848-5e5baf00-46a0-11ea-89be-c4140ab0c2ab.PNG)
