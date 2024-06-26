JPQL은 Java Persistence Query Language의 약자로, JPA(Java Persistence API)에서 사용되는 객체 지향 쿼리 언어이다. JPQL은 SQL을 추상화했기 때문에 특정 데이터베이스 SQL에 의존하지 않는 장점이 있다. 

#### JPQL의 특징
1. 객체 지향 쿼리 언어
    - JPQL은 데이터베이스의 테이블이 아닌 엔티티 객체를 대상으로 쿼리를 작성한다.
    - 엔티티 클래스와 그 속성을 사용하여 쿼리를 작성할 수 있다.

2. SQL 추상화
    - JPQL은 SQL을 추상화하여 데이터베이스 독립성을 제공한다.
    - JPQL로 작성된 쿼리는 JPA 구현체가 실제 SQL로 변환하여 실행한다.

3. 엔티티 매핑 활용
    - JPQL은 JPA 엔티티 매핑 정보를 활용하여 엔티티 객체를 대상으로 쿼리를 작성할 수 있다.
    - 엔티티의 속성, 관계 등을 JPQL에서 활용할 수 있다.

4. 동적 쿼리 생성
    - JPQL은 프로그래밍 언어 내에서 동적으로 쿼리를 생성할 수 있다.
    - 조건에 따라 쿼리 내용을 유동적으로 변경할 수 있다.

- 즉, JPQL은 JPA가 자동으로 생성하는 쿼리로는 해결하기 어려운 복잡한 요구사항을 처리하기 위해 활용된다. 개발자는 JPQL을 통해 보다 세밀한 데이터 조회 및 조작을 수행할 수 있다.
[[SQL]]
[[JPQL 사용]]
