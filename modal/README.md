
## modal
loadingModal is a simple yet customizable jQuery loading indicator plugin
<br>
<br>
## lottie
Lottie is a high-quality animation library created by Airbnb and operated on iOS, Android and React Native in real time, rendering After Effect animation in real time.
<br>
<br>
[about lottie](https://airbnb.design/lottie/)
<br>
<br>
## installation
modal
```
npm install react-native-extra-dimensions-android
npm install react-native-modal
npm install react-native-reanimated
```
<br>

lottie
```
yarn add lottie-react-native
```
or
```
npm install --save lottie-react-native
```
<br>

## Project
### modal 구현 js
기능
<br>
<br>
![modal1](https://user-images.githubusercontent.com/58720791/73995623-8c8d0780-499c-11ea-8b46-0eee2cabb017.PNG)
<br>
<br>
스타일
<br>
<br>
![modal2](https://user-images.githubusercontent.com/58720791/73995625-8dbe3480-499c-11ea-9342-2c5691081105.PNG)
### Home js에서의 modal 사용
![modal3](https://user-images.githubusercontent.com/58720791/73995627-8e56cb00-499c-11ea-8a35-689dcffd4fec.PNG)
### app gradle dependencies 추가
![modal4](https://user-images.githubusercontent.com/58720791/73995630-8e56cb00-499c-11ea-8e17-27bc599ff637.PNG)
### modal gif
![modal5](https://user-images.githubusercontent.com/58720791/73995631-8eef6180-499c-11ea-8d4e-63c12fd6d39d.PNG)
<br>
<br>

## Project result
![Android-Emulator-Pixel_2_API_28_5554-2020-02-12-17-46-43](https://user-images.githubusercontent.com/58720791/74318365-6b734f00-4dc0-11ea-8beb-79eece77baf9.gif)

<br>
<br>

## modal loading gif 작동 오류 시
build.gradle(app)의
dependencies에
implementation 'com.facebook.fresco:fresco:2.0.0' implementation 'com.facebook.fresco:animated-gif:2.0.0' 추가해야 gif가 돌아갑니다.

