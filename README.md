# OSS Assignment 02 — HTML / CSS / Bootstrap

- **학번 / 이름**: 22500349 / 선승범
- **학과**: 한동대학교 AI컴퓨터공학부 (전산심화)

동일한 HTML 문서에 서로 다른 CSS를 적용해 보고, Bootstrap 예제를 참고하여 웹페이지를 제작한 뒤 여러 페이지를 하나의 사이트로 연결한 실습입니다.

**Practice Flow:** HTML → CSS → Bootstrap → Page Link → GitHub → Vercel

---

## Assignment 02 수행 내용

| STEP | 내용 |
|---|---|
| 1 | `nostyle.html` — CSS 없이 HTML 구조만으로 기본 페이지 제작 (h1~h3, p, div, ul/li, a 포함) |
| 2 | `style1.html`, `style2.html` — 동일한 HTML에 서로 다른 CSS 적용 (대조적인 두 스타일) |
| 3 | 세 페이지를 브라우저와 DevTools로 비교 (HTML 구조는 같고 CSS만 다름) |
| 4 | `bootstrap_ex.html` — Bootstrap 5.3 **Album** 예제를 참고하여 제작 (CDN 사용) |
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
| `style1.html` | CSS Style #1 (밝은 테마 · 상단 가로 네비) | https://assign02-c02-22500349.vercel.app/style1.html |
| `style2.html` | CSS Style #2 (다크 테마 · 좌측 사이드바) | https://assign02-c02-22500349.vercel.app/style2.html |
| `bootstrap_ex.html` | Bootstrap Album 예제 재현 | https://assign02-c02-22500349.vercel.app/bootstrap_ex.html |

> **Vercel Deploy URL**: https://assign02-c02-22500349.vercel.app/
> (실제 서브도메인은 Vercel 프로젝트 이름에 따라 달라질 수 있으니 배포 후 확인·수정)

---

## Weekly Review — Week 2

### Key Learning — 이번 주 배운 핵심 3가지
1. **HTML과 CSS의 분리**: 문서의 구조(HTML)와 표현(CSS)이 분리되어 있어, 같은 HTML이라도 CSS만 바꾸면 완전히 다른 화면이 된다는 것을 직접 확인했습니다.
2. **CSS 핵심 속성**: `color`/`background`, `font`, `margin`/`padding`, `border`, `width`/`height`, `display`(flex 등) 속성으로 레이아웃과 디자인을 제어하는 법을 익혔습니다.
3. **Bootstrap 컴포넌트**: CDN으로 Bootstrap을 불러와 카드·그리드·버튼 같은 준비된 컴포넌트를 조합하면 빠르게 반응형 페이지를 만들 수 있다는 것을 배웠습니다.

### HTML vs CSS
- **HTML**은 페이지의 *뼈대(구조·내용)* 를 정의합니다. 제목, 문단, 목록, 링크 같은 요소가 무엇인지 표시합니다.
- **CSS**는 그 뼈대의 *겉모습(표현)* 을 담당합니다. 색, 글꼴, 간격, 배치를 지정해 같은 구조를 다르게 보이게 합니다.
- 이번 과제의 `nostyle` / `style1` / `style2`는 HTML은 똑같고 CSS만 다른, 이 원리를 그대로 보여주는 예입니다.

### Bootstrap 사용법
- **이유**: 자주 쓰는 UI(네비바, 카드, 버튼, 그리드)와 반응형 처리를 미리 만들어 두었기 때문에, 클래스만 붙이면 일관된 디자인을 빠르게 적용할 수 있습니다.
- **사용법**: `<head>`에 Bootstrap CSS CDN 링크를 추가하고, `container` / `row` / `col` / `card` / `btn` 같은 정해진 클래스를 HTML 요소에 붙여 사용합니다. 동작 컴포넌트가 필요하면 Bootstrap JS 번들도 함께 불러옵니다.

### Problem & Solution
- **문제**: <!-- TODO: 실습 중 실제로 겪은 문제 1가지로 교체하세요. 예: style2에서 사이드바와 본문이 세로로 쌓여 가로 배치가 안 됨 -->
- **해결**: <!-- TODO: 어떻게 해결했는지. 예: body에 display:flex와 flex-wrap을 주고 .navbar에 고정 width, .main에 flex:1을 줘서 가로 2단 레이아웃을 완성 -->

### AI Usage
- AI(Claude)를 활용해 페이지의 기본 골격과 CSS 초안을 생성했습니다.
- 생성된 코드는 <!-- TODO: 본인이 직접 확인/수정한 부분을 구체적으로 --> 브라우저와 DevTools로 렌더링 결과를 확인하고, 색상·문구·레이아웃을 직접 조정해 마무리했습니다.

### Reflection
- <!-- TODO: 새롭게 알게 된 점 또는 궁금한 점 1가지. 예: 같은 HTML에 CSS만 바꿔도 이렇게 달라진다는 게 인상 깊었고, Bootstrap의 그리드가 내부적으로 어떻게 flex로 동작하는지 더 알아보고 싶다 -->

---

## 최종 파일 구성
```
index.html          # 대표 페이지 (전체 링크)
nostyle.html        # HTML만 있는 기본 페이지
style1.html         # CSS Style #1
style2.html         # CSS Style #2
bootstrap_ex.html   # Bootstrap Album 예제
README.md           # 과제 및 Weekly Review
```
