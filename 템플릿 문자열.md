### REACT es6 문법 액기스
- 자바스크립트 es6의 주요문법 공부
1. 템플릿 문자열
  - 문자열 + 문자열, 문자열+변수 연결은 병합연산자(+)를 사용해야 한다.
  ```
  var string1 = "안녕하세요";
  vat string2 = "반갑습니다";
  var greeting = string1 + ' ' + string2;
  var product = {name:'도서',price:'4200원'};
  var message = '제품'+product.name + '의 가격은' + product.price + '입니다.';
  var multiLine = '문자열1\n문자열2`;
  var value1 = 1;
  var value2 = 2;
  var boolValue = false;
  var operator1 = '곱셈값은 '+(value1*value2) +'입니다';
  var operator2 = '불리언값은 '+{boolValue ? '참':'거짓')+'입니다.';
  ```
  - 병합 연산자를 사용해서 문자열과 문자열을 연결 + 문자열과 변수도 연결할 수 있다
  - 줄바꿈을 할 때는 이스케이프 시퀀스(\n)를 문자열에 포함시킨다.
  - 연산 결과를 괄호로 묶어 연산 구문으르 먼저 실행하기도 한다.
- 병합연산자를 사용하니 코드가 복잡해 보인다. -> 이를 개선하기위해 템플릿 문자열을 도입했다. 
  -  how? 작은따옴펴대신 백틱으로 문자열을 표현한다.
  -  템플릿 문자열에 특수기호 `$`를 사용해서 변수 또는 식을 포함할 수 있다.  
#### exercise 01
다음은 병합연산자로 표현된 코드다. 템플릿 문자열을 적용하여 바꿔봐라
```
var cart = {name:'도서',price:1500}
var getTotal = function(cart){
  return cart.price + '원';
};
var myCart = '장바구니에' + cart.name + '가 있습니다. 총 금액은 '+getTotal(cart)+'입니다.';
// => var myCart = `장바구니에 ${cart.name}가 있습니다. 총 금액은 ${getTotal(cart)}입니다.`; : 템플릿 문자열 적용하기
```
