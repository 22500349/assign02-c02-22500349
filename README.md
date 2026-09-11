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
> (실제 서브도메인은 Vercel 프로젝트 이름에 따라 달라질 수 있으니 배포 후 확인·수정)

세 페이지(`nostyle` / `style1` / `style2`)의 `<body>` 내용은 **완전히 동일**하며 `<style>`(CSS)만 다릅니다. 시맨틱 태그(`<header> <nav> <main> <div> <footer>`)로 영역을 나누고, 태그 선택자로 각 영역을 꾸몄습니다.

---

## Weekly Review — Week 2

### Key Learning — 이번 주 배운 핵심 3가지
1. **HTML과 CSS의 분리**: 같은 HTML이라도 CSS만 바꾸면 화면이 완전히 달라진다는 것을, `nostyle` / `style1` / `style2`를 직접 만들어 보며 확인했습니다.
2. **CSS 핵심 속성**: `color`/`background`로 색을, `margin`/`padding`/`border`로 여백과 테두리를, `width`/`display`로 배치를 조절하는 법을 익혔습니다. 특히 `margin`(바깥 여백)과 `padding`(안쪽 여백)의 차이를 알게 됐습니다.
3. **시맨틱 태그와 선택자**: `<header> <nav> <main> <footer>` 같은 의미 태그로 영역을 나누고, `header { }`처럼 태그 이름으로 골라 꾸미는 법을 배웠습니다. 선택자가 실제 HTML 구조와 맞아야 스타일이 적용된다는 것도 알게 됐습니다.

### HTML vs CSS
- **HTML**은 페이지의 뼈대(구조·내용)를 정의합니다. 제목, 문단, 목록, 링크 같은 요소가 무엇인지 표시합니다.
- **CSS**는 그 뼈대의 겉모습(표현)을 담당합니다. 색, 글꼴, 간격, 배치를 지정해 같은 구조를 다르게 보이게 합니다.
- `nostyle` / `style1` / `style2`는 HTML(body)은 똑같고 CSS만 다른, 이 원리를 그대로 보여주는 예입니다.

### Style 비교 — style1 vs style2 주요 차이
- **테마 색**: style1은 초록(배너 `#04aa6d`), style2는 빨강(`#d14836`)으로 완전히 대조되게 구성
- **메뉴 모양**: style1은 흰 박스에 회색 테두리, style2는 흰 테두리를 두른 둥근 알약 버튼(`border-radius: 40px`)
- **사이드바(div)**: style1은 파란 박스(흰 글씨), style2는 연분홍 박스(빨간 글씨)
- **본문**: style2는 빨강 배경 위에 흰 본문 박스를 얹어 대비 확보

### Problem & Solution
- **문제**: W3Schools의 Stylesheet 원본 CSS를 그대로 복사해 붙였는데, 제 페이지에는 스타일이 거의 적용되지 않았습니다.
- **해결**: 원본 CSS는 `#top`, `.menuitem` 같은 id/class 선택자로 W3Schools의 HTML을 겨냥한 것이었는데, 제 페이지는 `<header> <nav> <li>` 같은 시맨틱 태그로 만들어 이름표(id/class)가 없었습니다. AI의 도움으로 원인을 파악하고, 원본의 색은 살리되 선택자를 `header`, `li` 같은 태그 선택자로 바꿔 제 HTML에 맞게 다시 작성해 해결했습니다.

### AI Usage
- CSS 속성 개념(박스 모델, `display` 등) 이해와, W3Schools 원본 CSS를 제 시맨틱 태그에 맞게 변환하는 데 AI(Claude)를 활용했습니다.
- 받은 CSS는 그대로 쓰지 않고 VS Code Live Preview로 렌더링을 직접 확인하며, 색상·테두리(`border-radius`, 알약 버튼 모양 등)를 제 취향대로 수정해 마무리했습니다.

### Reflection
- 같은 HTML에 CSS만 바꿔도 초록(style1)과 빨강(style2)처럼 완전히 다른 화면이 되는 게 인상 깊었습니다.
- 이번에는 세로 1단으로 배치했는데, 원본처럼 좌우로 여러 칸을 나란히 놓는 `float` / `flex` 레이아웃을 다음에 더 배워보고 싶습니다.

---

## 최종 파일 구성
```
index.html          # 대표 페이지 (전체 링크)
nostyle.html        # HTML만 있는 기본 페이지
style1.html         # CSS Style #1 (Stylesheet 1 기반 · 초록)
style2.html         # CSS Style #2 (Stylesheet 2 기반 · 빨강)
README.md           # 과제 및 Weekly Review
```
