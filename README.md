# ui-practice

오늘의집 클론코딩을 통한 UI 개발 연습

> .scss-lint.yml, .prettierrc 설정 파일이 적용되도록 린터와 포맷터 설정을 제대로 해주어야 한다.

## Assets 준비하기

### 폰트

### 이미지

- 확대를 해서 깨지면 래스터 이미지, 확대를 해도 깨지지 않으면 벡터 이미지다.
- jpeg(jpg)는 압축을 잘해서 용량이 낮은 대신 퀄리티가 낮아진다.
  - 애플 사이트에서 사용되는 랜딩 이미지들은 2배 크기의 jpeg를 사용한다.
- png는 투명 배경을 지원한다. 또한 이미지 손실이 적은 대신 용량이 크다.
- 하나의 웹사이트가 차지하는 리소스 용량의 60~65%를 이미지가 차지한다고 한다.
  - 즉, 브라우저의 리소스 로드 시간이 길어지고, 결과적으로 렌더링이 느려진다.
- 구글에서 만든 webp 이미지 파일 포맷은 퀄리티 대비 낮은 용량을 지원하는 jpeg와 png의 중간 녀석이라고 볼 수 있다.
- 벡터 이미지는 이미지를 연산으로 그려내며, export할 경우는 무조건 svg 포맷이다.
- 벡터 이미지는 픽셀 사이즈에 상관없이 일정한 파일 사이즈를 가진다. 즉 이미지가 커져도 파일 사이즈의 용량은 일정하다.
- 반면 png나 jpeg 같은 비트맵, 래스터 이미지는 픽셀 사이즈에 비례해서 파일 사이즈가 커진다.
- 아이콘, 로고는 주로 svg로 뽑는다.(ie 6, 7, 8을 지원하지 않아도 되는 경우에 한함)

> 💡 Tip! 피그마에서 이미지를 Export하기 전에 `cmd + R` 단축키를 사용하여 이미지 파일명을 일괄적으로 수정하도록 하자.

- svg 코드는 더럽고 감당이 되지 않을 정도로 길기 때문에 아이콘 폰트로 컨버팅해서 사용한다.

### CSS 리셋

- Reset CSS는 완전 빈 도화지 같이 초기화시켜준다.
- Normalize.css는 하위 브라우저를 기준으로 모든 브라우저의 디자인을 동일하게 변경해준다.(다운그레이드)

## 참고 링크

### SCSS

- [SCSS 커맨드라인](https://sass-lang.com/documentation/cli/dart-sass)

### 기타

- [HTML EntityCode](https://dev.w3.org/html5/html-author/charref)
- [Convert svg to i](https://icomoon.io/app/#/select)
- [Favicon Generator](https://realfavicongenerator.net/)
