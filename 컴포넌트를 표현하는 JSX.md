## 컴포넌트를 표현하는 jsx
- jsx : javascript XML -> 자바스크립트에 XML을 추가한 확장형 문법
- XML또한 HTML의 표현법을 확장한 문법이므로 자바스크립트와 HTML을 안다면 쉽게 이해할 수 있따. 
- 기존에는 html과 자바스크립트를 분리해서 작성했어야 했음 -> 하나의 파일에 자바스크립트와 html을 동시에 작성할 수 있어서 편리하다.

1. JSX 사용해보기
- `create-react-app`으로 `do-it-example`이라는 리액트 만들었음 -> src폴더 안에 App.js라는 파일이 있다.
```
import React from 'react';

class App extends React.Component{
  render()
    return(
      <div>
        <img src="http://www.easypub.co.kr/images/logo_footer.png"/>
        <div>안녕하세요</div>
      </div>
      );
     }
    }
   export default App;
```
- render() 함수의 반환값 : html과 거의 비슷하다. 
- 차이점 : img element 끝에 마침표시`/>`가 있다는 차이점이 있다. 
- jsx는 html이 아니라 xml마크업 규칙을 따르기 때문에 이러한 표시를 자주 볼 수 있다. -> if 짝이 맞지 않으면 분석과정에서 오류가 발생한다.
```
<img src="http://www.easypub.co.kr/images/logo_footer.png"/> //정상
<img src="http://www.easypub.co.kr/images/logo_footer.png"> //error
```

2. jsx와 기존 개발 방법의 차이점은?
- 비교를 위해 jsx없이 화면을 구성해 보겠다.
  1. App 컴포넌트를 사용하지 앟고 화면을 구성한다.
    - index.js파일은 yarn start 명령어로 리액트 서버를 구동했을 때 최초로 실행된다.
    - 리액트 컴포넌트를 출력하는 코드를 별도의 색으로 표시했다. 
    ```
    // 필수 리액트 구동 모듈
    import React from 'react';
    import ReactDOM from 'react-dom';
    
    //초기 화면을 구성하는 사용자코드
    import `./index.css`;
    import App from `./App`;
    import * as serviceWorker form './serviceWorker';
    
    //react 엔진이 화면을 출력하는 코드
    //id=root인 element를 component에 출력한다.
    ReactDOM.render(<App/>,document.getElementById('root'));
    ```
- 어쩌고저쩌고 그래서 결론은 jsx 효율적이고 간단하고 짱이라는 거...
- 난 빨리 웹만들고 싶으니까 나중에 돌아와서 공부할거임 bye~
    
    
