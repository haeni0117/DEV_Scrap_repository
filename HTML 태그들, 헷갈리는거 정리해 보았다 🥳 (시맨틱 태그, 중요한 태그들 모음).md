# HTML 태그들, 헷갈리는거 정리해 보았다 🥳 (시맨틱 태그, 중요한 태그들 모음)
### 20210826

### HTML
- 웹사이트,웹어플리케이션(웹앱),모바일 앱까지 구현가능하다.
- 다른 본격적인 프로그래밍 언어에 비해 진입장벽이 낮은 mark-up 언어
### semantic tags(semantic markup)
- semantic : 의미의, 의미가 있는, 의미론적인
- html태그도 저마다의 의미가 있다는 것 -> 제목의 크기를 키우고 싶다고 단순히 텍스트를 키우기보다는 title이라는 heading을 선택하는 것이 더 낫다.
- ex) `<h1></h1>` : 태그만 봐도 제목이라는 것을 알 수 있다. -> div만으로 페이지를 만들 수는 있지만 추천하지 않는다.
- why? 왜 우리는 semantic tag를 사용해야 하는 걸까? 
  - SEO
  - Accessibility
  - Maintainability : 구조를 한눈에 알아볼 수 있다 + 유지보수 수월성
- How? div떡칠을 하기보다는 semantic tag(ex.header,nav,footer,main,article,section,aside, etc...)를 사용하는 게 좋다.
