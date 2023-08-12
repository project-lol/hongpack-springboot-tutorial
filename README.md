- 스프링부트란 무엇인가?
  - 자바 프로그램을 만들기 위한 노하우, 레시피가 들어가 있다.

- MVC의 역할과 실행흐름
    - V -> C -> M -> V (화면에서 요청이오고, 컨트롤러에서 반응하면, 반응에 대한 모델의 값을 가지고, 뷰를 제작한다.)
    - 요청은 컨트롤러에서 받고,

- JPA :
    - JPA의 핵심 도구 : Entity, Repository
        - Entity : DB가 잘 이해할 수 있게 규격화한 데이터.
        - Repository : Entity를 DB에 전달한다. 

- 롬복 : 
  - 코드를 간소화시켜주는 라이브러리이다.

- 라이브러리 설치방법 :
  - build.gradle 파일안에 들어간다. 

```java
dependencies {
	// 롬복 추가 !
	compileOnly 'org.projectlombok:lombok'
	annotationProcessor 'org.projectlombok:lombok'

	implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
	implementation 'org.springframework.boot:spring-boot-starter-mustache'
	implementation 'org.springframework.boot:spring-boot-starter-web'
	runtimeOnly 'com.h2database:h2'
	testImplementation 'org.springframework.boot:spring-boot-starter-test'
}
```