# 코르도바(Cordova)를 이용한 앱 개발 수업

## 1. 수업 개요
Apache Cordova는 **HTML, CSS, JavaScript**를 활용하여 모바일 애플리케이션을 개발할 수 있게 해주는 오픈소스 프레임워크입니다.  
하이브리드 앱 개발 방식을 통해 한 번의 코드 작성으로 **iOS, Android, Windows** 등 다양한 플랫폼에서 실행 가능합니다.

---

## 2. 학습 목표
- Cordova의 개념 및 특징 이해
- 개발 환경 설정 및 프로젝트 생성 방법 습득
- 기본 플러그인 활용 방법 학습
- 간단한 하이브리드 앱 제작 및 실행

---

## 3. 개발 환경 준비
1. **Node.js 설치**
   - Cordova는 Node.js 기반으로 동작
   - [Node.js 공식 사이트](https://nodejs.org/)에서 설치

2. **Cordova 설치**
   ```bash
   npm install -g cordova
   ```

3. **Android/iOS 개발 환경 설정**
   - Android Studio 또는 Xcode 설치 필요
   - 환경 변수 설정 (ANDROID_HOME 등)

---

## 4. 프로젝트 생성 및 실행
1. 프로젝트 생성
   ```bash
   cordova create MyApp com.example.myapp MyApp
   ```

2. 플랫폼 추가
   ```bash
   cd MyApp
   cordova platform add android
   cordova platform add ios
   ```

3. 앱 실행
   ```bash
   cordova run android
   cordova run ios
   ```

---

## 5. Cordova 기본 구조
- **www/** : HTML, CSS, JS 파일 위치
- **config.xml** : 앱 설정 파일 (앱 이름, 버전, 권한 등)
- **platforms/** : 각 플랫폼(Android/iOS) 빌드 결과물
- **plugins/** : Cordova 플러그인 모음

---

## 6. 플러그인 활용 예시
### (1) 카메라 플러그인
```bash
cordova plugin add cordova-plugin-camera
```

```javascript
navigator.camera.getPicture(onSuccess, onFail, {
    quality: 50,
    destinationType: Camera.DestinationType.DATA_URL
});

function onSuccess(imageData) {
    document.getElementById('myImage').src = "data:image/jpeg;base64," + imageData;
}

function onFail(message) {
    alert('Failed because: ' + message);
}
```

### (2) 디바이스 정보 확인
```bash
cordova plugin add cordova-plugin-device
```

```javascript
document.addEventListener("deviceready", function() {
    console.log(device.platform);
    console.log(device.version);
}, false);
```

---

## 7. 실습 예제
- **Hello World 앱 제작**
- 버튼 클릭 시 카메라 실행
- 디바이스 정보 화면에 출력

---

## 8. 수업 정리
- Cordova는 웹 기술을 이용해 **크로스플랫폼 앱** 개발을 지원
- 플러그인을 통해 네이티브 기능(카메라, 센서, 저장소 등) 활용 가능
- 빠르게 프로토타입 앱을 제작하고 배포할 수 있는 장점이 있음

---

## 9. 추가 학습 자료
- [Cordova 공식 문서](https://cordova.apache.org/docs/en/latest/)
- [Apache Cordova GitHub](https://github.com/apache/cordova)
