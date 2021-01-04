

## REACT 17

리엑트 버전 간의 임베딩을 안전하게 이뤄지게 만들고, 다른 기술로 작성된 앱으로의 임베딩 또한 손쉽게 만든다.

Document 레벨에 이벤트를 바인딩하지 않고, React트리가 렌더링되는 root DOM 컨테이너에 바인딩되도록 변경 



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
- Nest Application [인스턴스를](https://d2.naver.com/helloworld/7804182) 만드는 core 함수인 NestFactory를 사용하는 application의 entry file이다.
- NestFactory는 어플리케이션 인스턴스를 만들 수 있게 해주는 몇몇의 static method들을 노출시켜준다
- create() 메서드는 INestApplication Interface를 수행하는 application object를 반환하며, 해당 오브젝트는 다양한 methods set을 제공한다.



## SSR(Server-Side Rendering) 

Node.js 기반의 아키텍처로 서버에서 사용자에게 보여줄 페이지를 모두 구성하여 사용자에게 페이지를 보여주는 방식이다. 즉, 모든 데이터가 매핑된 서비스 페이지를 클라이언트에게 보여줄 수 있으며 서버를 이용해서 페이지를 구성하기 때문에 CSR(Client-Side Rendering)보다 페이지를 구성하는 속도는 늦어지지만 전체적으로 사용자에게 보여주는 콘텐츠 구성이 완료되는 시점은 빨라진다는 장점이 있다. 더불어 SEO(Search Engine Optimization)을 구성하는 데 더욱 편리해진다. 



##### SSR을 이용하면 좋은 이유

- 고객에게 더욱 빠르게 제공할 수 있다. 
- SEO를 구성을 유지하는 데 좋다
- 프론트엔드 영역과 백엔드 영역을 분리할 수 있다
- Javascript를 최대한 활용할 수 있다
- 다른 여러 가지 대안을 활용할 수 있는 토대가 된다



##### SSR의 단점

- 초기 구축 비용이 무척이나 크다 



> **SPA(single-page application)**
>
> 단일 페이지 애플리케이션으로, 현재의 페이지를 동적으로 작성함으로써 사용자와 소통하는 웹 애플리케이션이다. 연속되는 페이지 간의 사용자 경험을 향상시키고, 웹 애플리케이션이 데스크톱 애플리케이션처럼 동작하도록 도와준다. 

