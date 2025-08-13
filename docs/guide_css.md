# CSS 컨벤션 가이드

## 1. 기본 원칙
- CSS3 표준 속성 우선
- 불필요한 중복 스타일 제거

## 2. 코드 스타일
- 들여쓰기는 스페이스 2칸
- 속성 선언 순서: 레이아웃 → 박스모델 → 타이포그래피 → 시각적 효과
```
.selector {
  display: flex;
  width: 100%;
  font-size: 16px;
  color: #333;
}
```

## 3. 네이밍 규칙
- 컴포넌트: .main-header, .nav-menu, .product-card (kebab-case, 2단어 이상)
- 파트: .main-header__logo, .nav-menu__item, .product-card__title (__)
- 변형: .btn-tab--primary, .badge--sale, .popup--center (--)
- 상태: .nav-menu.is-active, .popup.is-visible, .btn-tab.is-hover (.is-)

## 4. 단위
- 폰트: `rem` 또는 `em`
- 여백/크기: `px` 또는 `%`
- 색상: HEX 또는 RGBA

## 5. 주석
```
/* Header 영역 스타일 */
header { ... }
```