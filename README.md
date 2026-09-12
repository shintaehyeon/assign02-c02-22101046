# Assignment 02 — HTML & CSS Practice

- 이름: 신태현 (Shin Tae Hyeon)
- 학번: 22010146
- 과목: Open Source Studio 02분반
- GitHub Repository: https://github.com/2026-2-OSS/assign02-c02-22101046
- Vercel Deploy URL: https://assign02-c02-22101046.vercel.app

## Assignment 02 수행 내용

Week 2의 HTML 초안을 정리하여 `h1`~`h3`, `p`, `div`, `ul`, `li`, `a`를 사용했다. 세 실습 페이지는 동일한 body 구조와 내용을 가지며, 스타일 페이지의 head에만 CSS를 추가했다. W3Schools CSS Demo의 Stylesheet 1과 2를 참고했다. 원본의 글꼴·색상·여백·float/position 배치를 기준으로 구현했다. 원본의 메뉴 클릭 동작은 별도 HTML 파일로 이동하는 링크로 바꾸었으며, Stylesheet 3·4 대신 선택한 두 스타일, No Stylesheet, Home을 연결했다. Stylesheet 2에는 작은 화면에서 긴 이름·학번 제목과 메뉴가 넘치지 않도록 미디어 쿼리를 추가했다.

## 각 페이지

| 페이지 | 설명 | 링크 |
| --- | --- | --- |
| index.html | 과제 기본 페이지 및 페이지 목록 | [Home](https://assign02-c02-22101046.vercel.app/index.html) |
| nostyle.html | CSS가 없는 HTML 기본 구조 | [No Style](https://assign02-c02-22101046.vercel.app/nostyle.html) |
| style1.html | 초록색 헤더, 왼쪽 메뉴, 파란색 사이드바 | [Style 1](https://assign02-c02-22101046.vercel.app/style1.html) |
| style2.html | 빨간색 배경, 오른쪽 메뉴, 흰색 본문 | [Style 2](https://assign02-c02-22101046.vercel.app/style2.html) |

각 실습 페이지에는 index.html로 돌아가는 Home 링크가 있다.

## Weekly Review – Week 2

### Key Learning

1. HTML은 요소가 부모와 자식 관계를 이루는 트리 구조이다. head에는 문서 제목과 문자 인코딩 같은 메타데이터를 넣고, body에는 화면에 표시할 내용을 넣는다.
2. HTML의 구조와 내용이 같아도 CSS의 color, background, font, margin, padding, border, width, display 등에 따라 화면이 달라진다.
3. position: absolute인 요소는 일반적으로 position이 static이 아닌 가장 가까운 조상을 기준으로 배치된다. 수업 예제처럼 main 안에 aside를 넣고 main에 position: relative를 주면, aside의 top과 right를 main 기준으로 지정할 수 있다. 이번 Stylesheet 1에서는 같은 원리로 .wrapper를 기준으로 #sidebar를 배치했다.

### HTML vs CSS

HTML은 제목, 본문, 메뉴처럼 페이지에 무엇이 들어가는지와 그 구조를 정한다. CSS는 그 내용의 색, 크기, 여백, 위치를 정한다. CSS가 없어도 내용과 링크는 남지만, 화면의 배치는 달라진다.

### Problem & Solution

초안의 nostyle.html에 헤더 CSS가 들어 있어 No Style 조건과 맞지 않았고, new.html에는 `padding: 10 px`처럼 숫자와 단위 사이에 공백이 있었다. AI의 도움으로 No Style 페이지에서는 CSS를 제거하고 스타일은 별도 페이지에 적용했다. CSS 길이는 `10px`처럼 붙여 썼다. 잘못 배치된 body/footer 종료 태그도 정리했다.

### AI Usage

Codex를 요구사항 정리와 코드·문서 초안 작성에 활용하고, W3Schools 예제와 비교해 수정했다.

### Reflection

aside를 main 안에 넣는 것만으로는 위치 기준이 정해지지 않고, 부모의 position 설정도 중요하다는 점을 배웠다. 기준이 되는 조상이 없을 때 absolute 요소가 어디를 기준으로 배치되는지도 더 알아보고 싶다.

## HTML/CSS 확인 방법

1. 세 실습 페이지를 각각 연다.
2. 브라우저 개발자 도구의 Elements에서 `div#top`을 선택한다.
3. Styles와 Computed에서 background, padding, font를 비교한다.
4. nostyle.html에는 작성한 CSS가 없고 브라우저 기본 스타일만 있는지 확인한다.
5. 화면 너비를 줄여 메뉴, 본문, 사이드바의 배치를 비교한다.

## 검증 기록

Codex로 필수 요소, 페이지 링크와 스타일 적용에 누락이 없는지 교차검증했다.

## 참고

- [W3Schools CSS Demo](https://www.w3schools.com/css/demo_default.htm)

## GitHub 및 배포 구성

- 제출 저장소: https://github.com/2026-2-OSS/assign02-c02-22101046
- Vercel 연결 저장소: https://github.com/shintaehyeon/assign02-c02-22101046
- Vercel Deploy URL: https://assign02-c02-22101046.vercel.app

수업 저장소에는 과제 코드와 작업 단계별 커밋을 기록했다. Vercel Hobby는 비공개 조직 저장소를 직접 배포할 수 없으므로, 기존 개인 과제 저장소에 동일한 최종 파일을 반영하고 해당 저장소의 main Push로 자동 배포한다. 제출용 저장소와 배포용 저장소의 최종 HTML, README, 퀴즈 파일은 동일하게 유지한다.

### 작업 단계별 커밋

1. `815beb3` — CSS 없는 HTML 기본 페이지 완성
2. `389e683` — W3Schools Stylesheet 1·2 구현
3. `810b1c3` — 첫 화면, Weekly Review, 퀴즈 완성

### 참고: 배포 제한

[Vercel Hobby와 비공개 조직 저장소](https://vercel.com/docs/git#using-hobby-teams)
