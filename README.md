## 🔗 빠른 링크
- 📑 기획서(피그마 슬라이드): https://www.figma.com/design/frdj3RVv4YaQB0MXHrSj0V/2%EC%B0%A8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8_design?node-id=1-3&t=bPGnOCQ79In0j33j-1
- 🎨 디자인 원본(피그마): https://www.figma.com/slides/HtA3UUvRiurlZiIL4hyUQ3/2%EC%B0%A8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8?node-id=53-34&t=oAqugnKRPfT7apW6-1

---

# HanaTour 사이트 리뉴얼 프로젝트

> 기존 하나투어 웹사이트를 사용자 중심으로 디자인하고, **프론트엔드 + 백엔드**가 연동되는 **반응형 웹**으로 구현한 프로젝트입니다.

---

## 📑 목차
- [프로젝트 개요](#프로젝트-개요)
- [기술 스택](#기술-스택)
- [폴더 구조](#폴더-구조)
- [주요 기능 & 페이지 구성](#주요-기능--페이지-구성)
- [역할 분담](#역할-분담)
- [개발 환경 & 실행 방법](#개발-환경--실행-방법)
- [배포 환경](#배포-환경)
- [추가 계획 & 확장 아이디어](#추가-계획--확장-아이디어)
- [크레딧 & 버전](#크레딧--버전)

---

## 프로젝트 개요
HanaTour 기존 사이트는 반응형 설계와 동적 요소가 부족했어요.  
그래서 **UX 중심 리뉴얼**, **일관된 디자인 시스템**, **반응형 레이아웃(모바일/태블릿 대응)**, **현대 웹 기술 도입(HTML5, CSS3, JS, PHP, MySQL 등)**을 목표로 프로젝트를 진행했습니다.  
디자인은 **Figma**로, 개발과 테스트는 **VS Code + XAMPP** 환경에서 이루어졌습니다.

---

| 이름 | 역할 | 주요 담당 | GitHub | 연락 |
| --- | --- | --- | --- | --- |
| 조아랑 | 팀장 · BE 리드 | 	Weather API<br>Section Slide<br>Login Page<br>서브페이지 DB 연동<br>백엔드 구축 | [@likerang](https://github.com/likerang) | like_rang@naver.com |
| 장원석 | FE 리드 · BE | Main Section<br>반응형<br>Event Page<br>서브페이지 DB 연동<br>백엔드 구축 | [@garam-dev](https://github.com/garam-dev) | garam@example.com |
| 정진욱 | FE | 	Footer<br>Section Slide<br>FAQ Page | [@jiwoo-park](https://github.com/jiwoo-park) | jiwoo@example.com |


---

## 기술 스택
- **Design**: Figma  
- **Frontend**: HTML5, CSS3, JavaScript, jQuery  
- **Backend**: PHP, MySQL  
- **개발 도구**: VS Code, XAMPP  

---

## 폴더 구조
```
/
├─ .vscode/
├─ css/              # 스타일 시트
├─ image/            # 이미지 에셋
├─ inc/              # 공통 include 모듈
├─ js/               # JavaScript 코드
├─ json/             # JSON 데이터
├─ sql/              # DB 스크립트
├─ uploads/          # 업로드 파일
├─ view/             # 뷰 템플릿
├─ *.php             # 주요 페이지 (index.php, login.php 등)
└─ readMe.md         # 기존 README
```

---

## 주요 기능 & 페이지 구성
- **메인 페이지**
  - 헤더, 메인 배너 (장원석 담당)
  - 상품 슬라이드, 푸터 (정진욱 담당)
  - Shorts/Youtube 슬라이드, 날씨 API 통합 (조아랑 담당)
- **FAQ 페이지**
  - 검색창, 카테고리 필터 (정진욱 담당)
- **로그인/회원가입 페이지**
  - 비회원 조회 기능, DB 연동 (조아랑 담당)
- **이벤트 & 관리자 페이지**
  - 이벤트 콘텐츠 및 관리자 기능 (장원석 담당)

---

## 개발 환경 & 실행 방법
1. **클론**
   ```bash
   git clone https://github.com/likerang/Site_Renewal_Project_HanaTour.git
   cd Site_Renewal_Project_HanaTour
   ```
2. **XAMPP 연결**
   - 프로젝트 폴더를 `htdocs/` 안에 복사
   - **MySQL** 실행, DB 세팅 (`sql/` 폴더 참고)
3. **웹 브라우저로 접근**
   - 로컬: `http://localhost/Site_Renewal_Project_HanaTour/`
   - 배포: `http://dkfkd.dothome.co.kr/Site_Renewal_Project_HanaTour/`
4. **VS Code Live Server**
   - HTML/CSS/JS 테스트 시 사용 가능

---

## 배포 환경
- **호스팅**: Dothome  
- **배포 URL**: [http://dkfkd.dothome.co.kr/Site_Renewal_Project_HanaTour/](http://dkfkd.dothome.co.kr/Site_Renewal_Project_HanaTour/)  
- **배포 방식**: FTP 업로드 (FileZilla 등)

---

## 추가 계획 & 확장 아이디어
- 반응형 개선: 모바일/태블릿 최적화 강화
- 사용자 피드백 기반 A/B 테스트
- 접근성 향상: ARIA, 키보드 내비게이션, 명도 대비 체크
- 배포 자동화: GitHub Actions + FTP

---

## 크레딧 & 버전
- 디자인: Figma  
- 개발: 조아랑, 정진욱, 장원석  
- 작업 기간: *2025-05-12 ~ 2025-07-14*
