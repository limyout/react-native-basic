## react-native 초기 설정 오류


It appears in \node_modules\metro-config\src\defaults\blacklist.js, there is an invalid regular expression that needed changed. I changed the first expression under sharedBlacklist from:


```
var sharedBlacklist = [
  /node_modules[/\\]react[/\\]dist[/\\].*/,
  /website\/node_modules\/.*/,
  /heapCapture\/bundle\.js/,
  /.*\/__tests__\/.*/
];
```


to:


```
var sharedBlacklist = [
  /node_modules[\/\\]react[\/\\]dist[\/\\].*/,
  /website\/node_modules\/.*/,
  /heapCapture\/bundle\.js/,
  /.*\/__tests__\/.*/
];
```
<br>

## react-native Can't find variable 오류


import information omission


ex) Can't find variable Component;
```
import React, {Component} from 'react';
```

ex) Can't find variable Fragment;
```
import React, {Fragment} from 'react';
```
<br>

## Unable to resolve module 'react-native-safe-area-context' from 'node_modules\react-navigation-stack\lib\module\vendor\views\Stack\StackView.js' 오류


```
yarn add react-navigation-stack@1.10.3
```
<br>

## react-native-icon

```
npm install react-native-vector-icons —save

npx react-native link react-native-vector-icons

npx react-native run-android
```

아래의 오류 무시
```
error React Native CLI uses autolinking for native dependencies, but the following modules are linked manually:
- react-native-vector-icons (to unlink run: "react-native unlink react-native-vector-icons")
```

https://ionicons.com/ 에서 아이콘의 이름 앞에  
android : md
```
import Icon from 'react-native-vector-icons/Ionicons'

<Icon name="md-arrow-round-up"/>
```
ios : ios
```
import Icon from 'react-native-vector-icons/Ionicons'

<Icon name="ios-arrow-round-up"/>
```
