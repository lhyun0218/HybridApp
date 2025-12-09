# 🌟 금연 도우미

> 건강한 내일을 위한 첫걸음, 스마트한 금연 관리 앱

<div align="center">

![Version](https://img.shields.io/badge/version-2.2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Web%20%7C%20Mobile-orange.svg)

[데모 보기](#) · [버그 제보](../../issues) · [기능 제안](../../issues)

</div>

---

## ✨ 주요 기능

### 📊 실시간 통계
- ⏱️ **금연 시간** 실시간 추적
- 💰 **절약 금액** 자동 계산
- 🚭 **미흡연 담배** 개비수 확인
- ❤️ **늘어난 수명** 시각화

### 🏆 게이미피케이션
- 🎯 **24단계 레벨 시스템** - 1분부터 10년까지
- 🏅 **업적 시스템** - 건강 회복 마일스톤
- 💎 **절약 목표** - 15가지 달성 가능한 목표
- 🎉 **실시간 알림** - 레벨업 & 달성 축하

### 🆘 위기 관리
- 🫁 **심호흡 가이드** - 흡연 욕구 대응
- 💬 **동기부여 메시지** - 강력한 명언 제공
- 💌 **나에게 쓴 편지** - 개인 맞춤 메시지
- 🔔 **일일 격려 알림** - 하루 3회 자동 알림

### 🎨 사용자 경험
- 🌙 **다크모드** 지원
- 📱 **모바일 최적화** 반응형 디자인
- ⚡ **빠른 성능** 로컬 데이터 저장
- 🔄 **자동 백업** 다중 저장소 시스템

---

## 🚀 빠른 시작

### 웹 버전
```bash
# 1. 저장소 클론
git clone https://github.com/yourusername/quit-smoking-helper.git

# 2. 디렉토리 이동
cd quit-smoking-helper

# 3. index.html 실행
# 브라우저에서 index.html 파일을 열기만 하면 됩니다!
```

### Cordova 모바일 앱
```bash
# 1. Cordova 설치
npm install -g cordova

# 2. 플랫폼 추가
cordova platform add android
cordova platform add ios

# 3. 플러그인 설치
cordova plugin add cordova-plugin-local-notification
cordova plugin add cordova-sqlite-storage

# 4. 빌드 및 실행
cordova build android
cordova run android
```

---

## 📱 스크린샷

<div align="center">

| 홈 화면 | 레벨 시스템 | 절약 추적 |
|:---:|:---:|:---:|
| ![Home](https://via.placeholder.com/250x500?text=Home) | ![Level](https://via.placeholder.com/250x500?text=Level) | ![Savings](https://via.placeholder.com/250x500?text=Savings) |

| 진행 상황 | SOS 기능 | 설정 |
|:---:|:---:|:---:|
| ![Progress](https://via.placeholder.com/250x500?text=Progress) | ![SOS](https://via.placeholder.com/250x500?text=SOS) | ![Settings](https://via.placeholder.com/250x500?text=Settings) |

</div>

---

## 🛠️ 기술 스택

- **Frontend**: Vanilla JavaScript (ES6+)
- **Styling**: CSS3 (Custom Properties, Flexbox, Grid)
- **Storage**: LocalStorage, SessionStorage, SQLite (Cordova)
- **Mobile**: Apache Cordova
- **Notifications**: Cordova Local Notification Plugin

---

## 📂 프로젝트 구조
```
new_hero/
│
├── index.html          # 메인 HTML 파일 (올인원)
├── config.xml          # Cordova 설정 파일
├── package.json        # NPM 패키지 정보
│
├── www/                # Cordova 웹 리소스
│   └── index.html      # 동일한 index.html 복사본
│
├── res/                # 앱 리소스
│   ├── icon/          # 앱 아이콘
│   └── screen/        # 스플래시 화면
│
└── platforms/          # Cordova 플랫폼 (빌드 시 자동 생성)
```

---

## 💡 사용 방법

### 1️⃣ 첫 설정
1. 앱 실행 후 **"시작하기"** 탭
2. 개인 정보 입력 (이름, 생년월일)
3. 과거 흡연 정보 입력 (기간, 하루 흡연량, 가격)
4. 담배 생각나는 상황 선택
5. 금연 시작 시간 설정

### 2️⃣ 일상 사용
- **홈**: 금연 시간 및 통계 확인
- **레벨**: 현재 레벨과 다음 목표 확인
- **절약**: 절약 금액으로 살 수 있는 것들
- **진행**: 전체 건강 회복 과정 보기
- **설정**: 알림 설정 및 테마 변경

### 3️⃣ 위기 상황
1. 홈 화면의 **"🆘 위기 상황 도움"** 버튼 클릭
2. 필요한 도구 선택:
   - 🫁 심호흡 가이드 (4초 들이쉬기-참기-내쉬기)
   - 💬 강력한 동기부여 명언
   - 💌 나에게 쓴 편지 읽기

---

## 🎯 핵심 레벨 시스템

| 레벨 | 시간 | 변화 |
|:---:|:---|:---|
| 🌱 Lv.1 | 1분 | 심박수·혈압 정상화 시작 |
| ⚡ Lv.7 | 1주 | 금단 증상 완화 |
| 💪 Lv.10 | 1개월 | 기침·숨가쁨 감소 |
| 🏆 Lv.16 | 6개월 | 만성 기침·가래 크게 감소 |
| ❤️ Lv.18 | 1년 | 심장병 위험 50% 감소 |
| 🌟 Lv.24 | 10년 | 폐암 사망 위험 50% 감소 |

---

## 🔐 데이터 저장

### 3중 백업 시스템
1. **LocalStorage** - 기본 저장소
2. **SessionStorage** - 임시 백업
3. **SQLite** - Cordova 환경 영구 저장

### 자동 저장
- 5초마다 자동 저장
- 페이지 닫기 전 저장
- 앱 백그라운드 전환 시 저장

---

## 🤝 기여하기

기여를 환영합니다! 다음 단계를 따라주세요:

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 라이선스

이 프로젝트는 MIT 라이선스 하에 있습니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

---

## 📧 문의

프로젝트 링크: [https://github.com/yourusername/quit-smoking-helper](https://github.com/yourusername/quit-smoking-helper)

이슈 제보: [https://github.com/yourusername/quit-smoking-helper/issues](https://github.com/yourusername/quit-smoking-helper/issues)

---

## 🌈 로드맵

- [ ] PWA 지원 (오프라인 모드)
- [ ] 소셜 공유 기능
- [ ] 금연 친구 챌린지
- [ ] AI 기반 맞춤 조언
- [ ] 건강 데이터 연동 (Apple Health, Google Fit)
- [ ] 다국어 지원

---

<div align="center">

**금연은 당신이 자신에게 줄 수 있는 최고의 선물입니다** 💝

Made with ❤️ by [Your Name]

⭐ 이 프로젝트가 도움이 되었다면 Star를 눌러주세요!

</div>
