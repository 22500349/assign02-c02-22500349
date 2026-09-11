# OSS Assignment 02 — HTML / CSS

- **학번 / 이름**: 22500349 / 선승범
- **학과**: 한동대학교 AI컴퓨터공학부 (전산심화)

동일한 HTML 문서에 서로 다른 CSS를 적용해 화면이 어떻게 달라지는지 비교하고, 여러 페이지를 하나의 사이트로 연결한 실습입니다.

**Practice Flow:** HTML → CSS → Page Link → GitHub → Vercel

---

## Assignment 02 수행 내용

| STEP | 내용 |
|---|---|
| 1 | `nostyle.html` — CSS 없이 HTML 구조만으로 기본 페이지 제작 (h1~h3, p, div, ul/li, a 포함) |
| 2 | `style1.html`, `style2.html` — 동일한 HTML에 서로 다른 CSS 적용 (W3Schools Stylesheet 1·2 참고, 대조적인 두 스타일) |
| 3 | 세 페이지를 브라우저와 DevTools로 비교 (HTML 구조는 같고 CSS만 다름) |
| 5 | `index.html` — 제작한 모든 페이지를 링크로 연결, 각 페이지에 Home 링크 추가 |
| 6 | Git으로 단계별 Commit + GitHub Push (3회 이상) |
| 7 | Vercel 자동 배포 확인 |
| 8~9 | README 작성 + Weekly Review – Week 2 |

---

## 각 페이지 설명 및 URL

| 페이지 | 설명 | URL (배포 후) |
|---|---|---|
| `index.html` | 과제 대표 페이지 — 전체 페이지 링크 모음 | https://assign02-c02-22500349.vercel.app/ |
| `nostyle.html` | CSS 없는 기본 HTML 페이지 | https://assign02-c02-22500349.vercel.app/nostyle.html |
| `style1.html` | CSS Style #1 — W3Schools **Stylesheet 1** 기반 (초록 테마) | https://assign02-c02-22500349.vercel.app/style1.html |
| `style2.html` | CSS Style #2 — W3Schools **Stylesheet 2** 기반 (빨강 테마) | https://assign02-c02-22500349.vercel.app/style2.html |

> **Vercel Deploy URL**: https://assign02-c02-22500349.vercel.app/

세 페이지(`nostyle` / `style1` / `style2`)의 `<body>` 내용은 **완전히 동일**하며 `<style>`(CSS)만 다릅니다. 시맨틱 태그(`<header> <nav> <main> <div> <footer>`)로 영역을 나누고, 태그 선택자로 각 영역을 꾸몄습니다.

---

## Weekly Review — Week 2

### Key Learning — 이번 주 배운 핵심 3가지
1. HTML과 CSS: 문서의 구조(HTML)와 표현(CSS)이 분리되어 있어, 같은 HTML이라도 CSS만 바꾸면 완전히 다른 화면이 된다는 것을 직접 배웠습니다.
2. CSS 의 태그들: `color`/`background`, `font`, `margin`/`padding`, `border`, `width`/`height`, `display` 속성으로 색·여백·박스·배치를 제어하는 법을 익혔습니다.
3. 각 태그들의 스타일: `<header> <nav> <main> <footer>` 같은 의미 태그로 영역을 나누고,`Style{}`을 통해 각 태그의 영역별로 꾸밀수 있다는걸 알았습니다.

### HTML vs CSS
- HTML 은 페이지의 뼈대 입니다. 제목, 문단, 목록, 링크 같은 요소가 무엇인지 표시합니다.
- CSS는 그 뼈대의 겉모습 입니더. 색, 글꼴, 간격, 배치를 지정해 같은 구조를 다르게 보이게 합니다.
- 이번 과제의 `nostyle` / `style1` / `style2`는 HTML은 똑같고 CSS만 다릅니다

### Problem & Solution
- **문제**: CSS의 태그들을 사용해 여백이나 그곳의 색,배치등을 조정 하려했으나 제대로 되지 않았다
- **해결**: 띄어쓰기, 순서변경, 지우고 다시 쓰기 등등 별의 별 방법을 사용하던 중 갑자기 해결 되었다

### AI Usage
- 기본적인 HTML 과 CSS 를 제작해달라 부탁한뒤 이것들을 다시 지우고 내가 작성해본뒤 무슨 차이가 있나 비교해 봤다, 동시에 여러 태그들의 기능과 설명을 정리 받았다

### Reflection
- 이전의 바이브 코딩에서 궁금하거나 이러지 않을까 했던 부분들을 실제로 제작해 보며 깨닫고 좀더 내가 원하는 방식으로 다룰수 있게 되었다

---

## 최종 파일 구성
```
index.html          # 대표 페이지 (전체 링크)
nostyle.html        # HTML만 있는 기본 페이지
style1.html         # CSS Style #1 (Stylesheet 1 기반 · 초록)
style2.html         # CSS Style #2 (Stylesheet 2 기반 · 빨강)
README.md           # 과제 및 Weekly Review
```
