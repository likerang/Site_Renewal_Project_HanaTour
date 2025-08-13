# 하나투어 JavaScript 컨벤션 가이드

## 1. 문법 스타일
* **jQuery 기반** DOM 조작 및 이벤트 처리
* `const`, `let` 혼용 사용 (ES6+ 문법 일부 적용)
* 세미콜론(`;`) 일관성 있게 사용

## 2. 들여쓰기와 공백
* 들여쓰기는 **스페이스 2칸**
* jQuery 체이닝 시 적절한 줄바꿈
```javascript
$('.aside_btns a').removeClass('active');
$(this).addClass('active');
```

## 3. 네이밍 규칙
* 변수/함수: `camelCase` (`asideBtn`, `getCookie`)
* jQuery 객체: `$` 접두사 권장 (`$btns`, `$underline`)
* 상수: kebab-case 클래스명 그대로 사용

## 4. 함수 작성
* **함수 선언식** 주로 사용
* 이벤트 핸들러는 **익명 함수**로 작성
* 하나의 함수는 단일 책임 원칙 준수
```javascript
function setCookie(name, value, days) {
  const date = new Date();
  // 로직...
}
```

## 5. 이벤트 처리
* **jQuery 이벤트 메서드** 활용 (`.on()`, `.click()`)
* `preventDefault()` 적절히 사용
* 반응형 처리는 `resize` 이벤트 활용

## 6. 주석
* 기능별 섹션 구분 주석 사용
* 복잡한 로직에 대한 설명 주석 권장
```javascript
// 어사이드 탭버튼 클릭시 할일
$('.aside_btns a').click(function(e){
  // 로직...
});
```