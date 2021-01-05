## Redux-Saga

Redux-Saga는 react / redux 앱의 사이드 이펙트, 비동기 동작들을 더 쉽고, 더욱 편리하게 사용하게하는 것이다.

그렇다면 ES6의 async, await과 다른점은 무엇인가 ?

실제로 시스템적으로는 같은 동작이라고 이야기를 할 수 있으나 Redux-Saga의 경우 실 동작에 있어 세분화를 하여 작동시킬 수 있다는 점이 유리한 부분이다.

하지만 코드양이 급격히 늘고, 코드를 관리해야하는 부분도 늘기에 Redux-Saga가 세분화해서 사용을 할 수있기에 무조건적으로 유리하다 말할 수 없다.



##### Generator

- *:함수 뒤에 *를 선언하여 Generator함수 라는 것을 선언
- yield: 키워드 뒤에 있는 값들을 순서대로 넘겨준다.
- next: 이 메소드는 다음 두 속성을 갖는 객체를 반환해야한다.
- done: 반복이 끝났는 지 나타냄
- value: 현재 순서의 값을 나타냄
- call: 첫 번째 파라미터로 전달한 함수에 그 뒤에 있는 파라미터들은 전달하여 호출해준다. 테스트 작성에 용이
- delay: 해당 메소드를 실행하기 전에 대기하는 메소드
- takeEvery: 특정 액션을 모니터링을 하고, 발생하면 특정 함수를 발생시킨다. takeEvery를 통해 액션을 바라보고 액션이 dispatch 될때마다 action을 실행하기 위해 takeEvery핼퍼 함수를 사용한다.
- all: Redux-Saga를 여러 개를 묶어서 사용할 때 all effect를 사용한다.
- put: 우리가 이펙트라고 부르는 예중 하나이다. 이펙트는 미들웨어에의해 수행되는 명령을 담고 있는 간단한 객체이다.

##### Thunk 와 Saga

둘 다 미들웨어 라이브러리이다.

> Redux 미들웨어는 dispatch() 메소드를 통해 store로 가고 있는 액션을 가로 채는 코드 
>
> action은 literally하게 될 수 있다.

##### Redux-Thunk

추가적으로 표준 액션들을 디스패치할 때, Redux-Thunk 미들웨어는 당신이 thunks라고 불리는 특별한 함수를 디스패치하는 것을 허락한다. Thunks는 일반적으로 다음 구조를 가진다.

```react
export const thunkName = parameters => (dispatch, getState) => {
  // 당신의 어플리케이션 로직을 여기에 적으세요
};
```

thunk는 몇가지의 parameters를 인수로 취하고 또 다른 함수를 return하는 함수다. 내부 함수는 dispatch 함수와 getState함수를 사용한다. 두 함수다 Redux-Thunk 미들웨어에서 제공받는 다.

##### Redux-Saga

redux-saga 미들웨어는 sagas라고 불리는 순수함수로 복잡한 어플리케이션 로직을 표현할 수 있다. sagas는 generator라고 불리는 특별한 함수로 구성되어져 있다. 



##### Thunk와 Saga의 차이점

Thunks는 action에 응답을 줄 수 없다. 하지만 redux-saga는 store를 subscribe하고 특정 작업이 dispatch될 때 saga가 실행되도록 할 수 있다.