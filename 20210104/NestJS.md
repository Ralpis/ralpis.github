## Nest.js

- express 기반으로 node.js에 백엔드를 구성할 수 있도록 도와준다
- typescript를 지원하며 javascript로 어플리케이션을 작성할 수 있다.
- node.js의 프레임워크에는 없는 구조를 가지고 있다.
- nest.js는 구조를 갖고 있으며 이를 활용하기때문에 백엔드를 쉽게 만들 수 있다.
- node.js 어플리케이션을 빌드하는 데 유용하며, 객체지향프로그래밍과 함수형프로그래밍, 함수반응형 프로그래밍의 요소도 일부분 사용한다.



#### Nestjs Setting 

```null
npm i -g @nestjs/cli
```



#### nest-cli

- 커맨드 라인으로 필요한 것을 생성하고 모두 import 해준다.
- ![img](https://media.vlpt.us/images/zoeyul/post/cae789bc-1753-4170-aff1-0ddb51de5951/Screen%20Shot%202020-11-03%20at%2010.55.22%20PM.png)

#### Controllers

- nest.js 어플리케이션은 main.ts에서 시작한다. 하나의 모듈에서 어플리케이션을 생성
- controller는 기본적으로 url을 가져오고 함수를 실행한다. (express router의 역할)

##### main.ts

- 이름변경시 시작을 할 수 없다
- Nest Application 인스턴스를 만드는 core 함수인 NestFactory를 사용하는 application의 entry file이다.
- NestFactory는 어플리케이션 인스턴스를 만들 수 있게 해주는 몇몇의 static method들을 노출시켜준다
- create() 메서드는 INestApplication Interface를 수행하는 application object를 반환하며, 해당 오브젝트는 다양한 methods set을 제공한다.
- 

