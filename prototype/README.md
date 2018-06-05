
## `prototype` 알아보기

`prototype`을 얘기하기 전에 우선 `상속`이란 개념에 대해 얘기해보자. `상속`이란 부모 객체의 로직을 그대로 물려 받는 자식 객체를 만드는 기능을 의미한다. 즉 부모 객체가 가지고 있는 프로퍼티와 메서드를 자식 객체에서 재정의 할 필요없이 물려받아 사용할 수 있는 것이다. 자바스크립트는 클래스가 없기 때문에 객체에 있는 `prototype`이라는 특수한 프로퍼티를 이용해서 `상속`을 구현할 수 있다.

### 1. `전역 변수`와 `지역 변수`  

자바스크립트에서 `전역 변수`는 어플리케이션 어디서나 접근할 수 있는 변수를 의미한다.

```js
var vscope = 'global';
function fscope(){
    alert(vscope);
}
fscope(); // 'global'
```

----------------

***참조***  

[유효범위 - 생활코딩](https://opentutorials.org/course/743/6495)