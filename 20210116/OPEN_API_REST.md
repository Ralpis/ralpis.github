### OPEN API 

하나의 웹 사이트에서 기능을 공개한 프로그래밍 인터페이스이다.

이를 이용할 때는 기능마다 부여된 권한에따라 기능을 이용할 수 있거나 못하거나 둘 중 하나이다. 

대표적으로 구글 맵의 경우에 부분적으로 유료로 적용하여 제공을 하는 것을 볼 수 있다.

OPEN API 서비스는 대내외 연계를 하는 데 도움이 된다



### REST 

REST는 아키텍처 스타일이며 자원 지향 구조(ROA:Resource Oriented Architecture)로 웹 사이트의 컨텐츠를 전부 하나의 자원으로 파악하여 URI(Uniform Resource Indentifier)를 부여하고, 해당 자원에 대한 CRUD작업을 HTTP의 기본 명령어인 POST, GET, PUT, DELETE를 통해서 처리한다.

REST의 기본 개념에 충실하게 설계된 서비스를 RESTful하다고 할 수 있다.



### RESTful한 서비스 구축의 원칙

오픈하고자 하는 자원을 정의한다.

그리고 그 자원에 관하여 조회, 변경과 같은 CRUD의 기능을 부여할 지 정한다.단순히 조회만 부여하는 경우 GET만 허용하면 된다.



### RESTful Open API 사례 

| 기업   | 사이트 가이드                                                | Open API 종류     |
| ------ | ------------------------------------------------------------ | ----------------- |
| NAVER  | https://developers.naver.com/docs/common/openapiguide/       | 데이터랩, 검색 등 |
| 11st   | https://openapi.11st.co.kr/openapi/OpenApiServiceIntroduce.tmall | 상품 조회 등      |
| 카카오 | https://developers.kakao.com/                                | 개발툴 등         |

