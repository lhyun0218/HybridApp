# 🌟 Samsung Electronics - Innovation Never Stops (모바일 웹사이트)

## 📄 파일 개요
본 `index.html` 파일은 **jQuery Mobile (1.4.5)** 및 **jQuery (1.11.1)**를 기반으로 구축된 삼성전자(Samsung Electronics)의 모바일 웹페이지입니다. CSS를 통해 삼성 브랜드 아이덴티티를 강조하고, 여러 `data-role="page"`를 활용하여 단일 페이지 애플리케이션(SPA) 구조를 구현했습니다.

---

## 🎨 주요 디자인/스타일 특징

* **브랜드 컬러:** `--samsung-blue: #1428A0`, `--samsung-gray: #f8f9fa` 사용.
* **애니메이션:** 헤더 (`.samsung-hero`)에 `pulse` 효과, 로고 (`.animated-logo`)에 `float` 효과 적용.
* **UI 강조:** `.product-card` (좌측 파란색 경계), `.stat-box` (그라디언트 배경) 등을 활용하여 모바일 가독성 및 시각적 흥미도 제고.

---

## 📱 페이지 구조 (jQuery Mobile)

| ID | 제목 | 핵심 내용 | 핵심 컴포넌트 |
| :--- | :--- | :--- | :--- |
| `home` | **홈** | 메인 메뉴, **Galaxy S24 AI 뉴스 티커**, 주요 성과 배지. | `listview`, `animated-logo` |
| `intro` | **회사 소개** | 기업 개요, 핵심 가치, **2024년 주요 실적** (스마트폰/반도체 세계 1위). | `collapsible-set`, `stat-box` |
| `products` | **주요 제품** | Galaxy S24/Z Fold, Neo QLED/OLED TV, **비스포크 AI 가전**, GAA 3nm 반도체. | `product-card` |
| `innovation` | **혁신 기술** | **Galaxy AI** (실시간 통역), **GAA 3nm 공정**, 무풍 기술, RE100 지속가능 경영. | `innovation-badge` |
| `media` | **미디어** | YouTube 영상 (`iframe`) 임베드 (Galaxy S24 Ultra). | `video-container` |
| `history` | **연혁** | 기업 이정표. | `timeline-item` |

---

## ✨ 기술 하이라이트

1.  **AI 집중:** `home`, `products`, `innovation` 페이지 전반에 걸쳐 **Galaxy AI**를 최신 및 핵심 기술로 가장 중요하게 다룹니다.
2.  **산업 리더십 강조:** **세계 1위 스마트폰**, **세계 1위 반도체** 성과를 수치와 배지로 명확히 제시.
3.  **외부 리소스:** Font Awesome 6.4.0을 사용하여 다양한 아이콘을 적용.
