# Weekly Question – Week 2

- 학번: 22101046
- 이름: 신태현
- 주차: 2주차
- 출제 방식: 수업 필기 내용을 바탕으로 AI 활용

## 문제 1 — 객관식

### 문제
HTML 문서에서 문자 인코딩 등 메타데이터를 작성하는 영역은 어디인가?

### 보기
① `<head>`
② `<body>`
③ `<main>`
④ `<aside>`

### 정답
① `<head>`

### 해설
`<head>`에는 문서 제목, 문자 인코딩 등 문서에 관한 정보를 작성한다. `<body>`에는 화면에 표시할 내용을 작성한다.

## 문제 2 — 주관식

### 문제
`<main>` 안에 `<aside>`가 있다. aside에 다음 CSS를 적용하여 main의 오른쪽 위에 붙이려고 한다.

```css
aside {
    position: absolute;
    top: 0;
    right: 0;
}
```

main에 추가해야 할 CSS를 쓰고, 그 CSS가 필요한 이유를 설명하시오.

### 예시 정답
main에 position: relative;를 추가해야 한다. absolute로 지정된 aside의 위치 기준을 부모인 main으로 만들기 위해서이다. 그러면 top: 0; right: 0;이 main을 기준으로 적용된다.

### 해설
absolute 요소는 일반적으로 position이 static이 아닌 가장 가까운 조상을 기준으로 배치된다. 따라서 HTML에서 부모 안에 넣는 것만으로는 부족하며, 부모가 위치 기준이 되도록 설정해야 한다.

제출 폼: https://forms.gle/QoxoyWP8ZiJTyJu67
