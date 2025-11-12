
# 삼진어묵 공식 웹사이트

> 1953년부터 3대째 이어온 대한민국 대표 어묵 브랜드, 삼진어묵의 공식 웹사이트입니다.

## 📋 프로젝트 소개

삼진식품의 어묵 브랜드를 소개하는 반응형 모바일 웹 애플리케이션입니다. 
jQuery Mobile 프레임워크를 활용하여 구축되었으며, 회사 소개부터 제품 정보, 체험관 안내까지 
모든 정보를 직관적으로 제공합니다.

## ✨ 주요 기능

### 🏠 메인 페이지 (#hero)
- 브랜드 히어로 섹션
- 주요 메뉴 네비게이션 (회사소개, 홍보영상, 베스트상품, 체험관)
- 회사 연락처 및 사업자 정보

### 🏢 회사 소개 (#company)
- 인사말씀
- 회사 역사 및 비전
- R&D 투자 및 스마트 팩토리 구축 소개

### 🎬 홍보 영상 (#youtube)
- YouTube 영상 갤러리
- 삼진어묵 소개 영상
- 공장 생산 공정 영상

### 🛍️ 베스트 상품 (#best)
- 제품 카드 그리드 레이아웃
- 7개 베스트 상품 소개
  - 삼진프리미엄세트 1호, 2호
  - 1953세트 1호, 2호
  - NEW꼬치사각, 알찬모듬어묵, 실속모듬어묵
- 공식몰 링크 연결

### 🎨 체험관 (#experience, #experience-gallery)
- 체험관 운영시간 안내
- 체험 신청 정보
- 체험관 갤러리 (6장의 사진)

## 🛠️ 기술 스택

### Frontend
- **HTML5** - 시맨틱 마크업
- **CSS3** - 커스텀 스타일링
  - CSS Grid Layout
  - Flexbox
  - CSS Variables (`:root`)
  - 반응형 디자인 (@media queries)
- **JavaScript** - jQuery 1.11.1
- **jQuery Mobile 1.4.5** - 모바일 UI 프레임워크

### 디자인 패턴
- 싱글 페이지 애플리케이션 (SPA) 구조
- 페이지 전환 애니메이션
- 반응형 그리드 시스템
- 모바일 퍼스트 접근

## 📁 파일 구조

```
project-root/
│
├── index.html                    # 메인 HTML 파일 (SPA 구조)
├── readme.md                     # 프로젝트 문서
│
├── assets/
│   ├── branding/
│   │   ├── samjin.png           # 삼진어묵 로고
│   │   └── story.jpg            # 회사 스토리 이미지
│   │
│   ├── intro/
│   │   └── samjinintro.jpg      # 메인 소개 이미지
│   │
│   ├── products/
│   │   ├── 1.jpg                # 삼진프리미엄세트 1호
│   │   ├── 2.jpg                # 삼진프리미엄세트 2호
│   │   ├── 3.jpg                # 1953세트 1호
│   │   ├── 4.jpg                # 1953세트 2호
│   │   ├── 5.jpg                # NEW꼬치사각
│   │   ├── 6.jpg                # 알찬모듬어묵
│   │   └── 7.jpg                # 실속모듬어묵
│   │
│   └── experience/
│       ├── experience1.jpg       # 체험관 메인 이미지
│       ├── experience2.jpg       # 운영시간 안내
│       ├── experience3.jpg       # 체험신청 안내
│       ├── experience gallery1.jpg  # 갤러리 사진 1
│       ├── experience gallery2.jpg  # 갤러리 사진 2
│       ├── experience gallery3.jpg  # 갤러리 사진 3
│       ├── experience gallery4.jpg  # 갤러리 사진 4
│       ├── experience gallery5.jpg  # 갤러리 사진 5
│       └── experience gallery6.jpg  # 갤러리 사진 6
│
└── external/
    ├── jquery-1.11.1.min.js      # CDN
    ├── jquery.mobile-1.4.5.min.js # CDN
    └── jquery.mobile-1.4.5.min.css # CDN
```

## 🎨 디자인 시스템

### 컬러 팔레트
```css
--accent: #ff7a00;        /* 메인 오렌지 */
--accent-2: #ffd6a5;      /* 서브 오렌지 */
--glass: rgba(255,255,255,0.06);  /* 글래스모피즘 */
```

### 타이포그래피
- 본문: 'Nanum Gothic', system-ui
- 제목: 'Playfair Display', serif

### 반응형 브레이크포인트
- 모바일: < 480px
- 태블릿: 480px ~ 900px
- 데스크톱: > 900px

## 🚀 설치 및 실행

### 1. 프로젝트 클론
```bash
git clone [repository-url]
cd samjin-eomuk-website
```

### 2. 파일 구조 확인
모든 이미지 파일이 올바른 위치에 있는지 확인하세요.

### 3. 실행
```bash
# 간단한 HTTP 서버 실행 (Python 3)
python -m http.server 8000

# 또는 Live Server 확장 프로그램 사용 (VS Code)
# index.html 우클릭 → Open with Live Server
```

### 4. 브라우저에서 확인
```
http://localhost:8000
```

## 📱 페이지 네비게이션

웹사이트는 jQuery Mobile의 data-role="page" 속성을 사용하여 
페이지 간 부드러운 전환을 제공합니다.

```html
<!-- 메인으로 이동 -->
<a href="#hero">메인으로</a>

<!-- 회사소개로 이동 -->
<a href="#company">회사 소개</a>

<!-- 홍보영상으로 이동 -->
<a href="#youtube">홍보 영상</a>

<!-- 베스트상품으로 이동 -->
<a href="#best">베스트상품</a>

<!-- 체험관으로 이동 -->
<a href="#experience">체험관</a>

<!-- 체험관 갤러리로 이동 -->
<a href="#experience-gallery">체험관 갤러리</a>
```

## 🔗 외부 링크

- **공식 쇼핑몰**: https://www.samjinfood.com/goods/best.php
- **YouTube 영상 1**: https://www.youtube.com/watch?v=490Y2iBK2EE
- **YouTube 영상 2**: https://www.youtube.com/watch?v=0l1DCH7GO9g

## 📞 회사 정보

**삼진식품㈜**
- 주소: 부산광역시 영도구 태종로99번길 36
- 전화: 051-412-5468
- 팩스: 051-980-5468
- 이메일: samjinorder@daum.net
- 사업자등록번호: 360-86-00207
- 통신판매업신고번호: 제2016-부산영도-00107호

## 🔧 개선 사항 및 TODO

### 현재 이슈
- [ ] HTML 인코딩 문제 (한글 깨짐 현상)
- [ ] 이미지 파일명 공백 처리 (예: `experience gallery1.jpg` → `experience-gallery1.jpg`)

### 향후 개선 계획
- [ ] 모던 프레임워크로 리팩토링 (React, Vue.js)
- [ ] 성능 최적화 (이미지 lazy loading)
- [ ] SEO 최적화
- [ ] 접근성 개선 (ARIA 라벨 추가)
- [ ] PWA 전환
- [ ] 다국어 지원 (영어, 일본어)

## 📄 라이선스

© 2024 삼진식품㈜ All rights reserved.

## 🤝 기여

프로젝트 개선을 위한 제안은 언제든 환영합니다.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 문의

프로젝트 관련 문의사항은 samjinorder@daum.net으로 연락주세요.

---

**Made with ❤️ by Samjin Food
