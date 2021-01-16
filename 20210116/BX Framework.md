# BX Framework 

### Class Hot Deploy 

- WAS로 배포를 하는 중에는 JVM의 멈춤 현상이 발생할 수 있는 데 
BX Framework은 자체 구현한 Class Loader의 기능을 이용하여 
중단 없는 Class Hot deploy를 지원한다? 

### PURE POJO (개발 생산성)

- 오래되고 간단한 오브젝트로 구성된 순수 자바 프레임워크 
  즉, 무겁지 않고 POJO의 설계 개념인

  -  미리 지정된 클래스를 extends하는 것
  - 미리 정의된 인터페이스를 implement 하는 것
  - 미리 정의된 Annotation을 포함하는 것

  을 잘 지켜 프레임워크를 만들었다는 소리 ! 

  전자정부 프레임워크 eGov랑 호환 인증 

### 사용자 프로그램 품질 보장

Code Inspection Tool로 코드가 표준을 준수하는 지, 잠재적 메모리 누수가 발생할 수 있는 지, 표준에 위배사항은 없는 지를 확인할 수 있다

또한, 물리적인 관계뿐 아니라 논리적 관계도 분석을 할 수 있다.