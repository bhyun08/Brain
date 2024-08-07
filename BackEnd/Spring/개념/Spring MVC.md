Spring MVC는 Spring 프레임워크에서 MVC(Model-View-Controller) 형식으로 애플리케이션을 세 가지 핵심 구성 요소로 나누어 개발하는 방식이다.      

### 구성요소
1. **Controller**: 클라이언트의 요청을 받아 처리하고, 적절한 모델 데이터를 준비하여 뷰에 전달하는 역할을 한다. Controller는 @Controller 어노테이션을 사용하여 정의된다.
    
2. **Model**: 애플리케이션의 데이터와 비즈니스 로직을 포함하고 있다. Controller에서 준비한 모델 데이터는 뷰에 전달되어 화면에 표시된다.
    
3. **View**: 사용자 인터페이스를 담당하며, 모델 데이터를 기반으로 화면을 렌더링(구성)한다. 일반적으로 JSP, Thymeleaf, Freemarker 등의 템플릿 엔진을 사용하여 뷰를 구현한다.
    
4. **DispatcherServlet**: Spring MVC의 핵심 컨트롤러로, 클라이언트의 요청을 받아 적절한 Controller로 전달하고, 그 결과를 View에 렌더링하는 역할을 한다.
    
5. **HandlerMapping**: 클라이언트의 요청 URL을 Controller 메서드에 매핑하는 역할을 한다.
    
6. **ViewResolver**: 논리적인 뷰 이름을 실제 뷰 리소스로 변환하는 역할을 한다.
### 동작흐름

![](https://i.imgur.com/e2fNHkD.png)


1. 클라이언트가 요청을 보내면 DispatcherServlet이 해당 요청을 받는다.
2. DispatcherServlet은 HandlerMapping을 통해 적절한 Controller를 찾아낸다.
3. Controller는 요청을 처리하고, 모델 데이터를 준비하여 DispatcherServlet에 반환한다.
4. DispatcherServlet은 ViewResolver를 통해 적절한 View를 찾아내고, 모델 데이터를 View에 전달한다.
5. View는 모델 데이터를 기반으로 화면을 렌더링하여 클라이언트에게 응답을 보낸다.

- Spring MVC는 웹 애플리케이션 개발에 있어 많은 장점을 제공한다. 구조화된 접근 방식을 통해 개발 생산성을 높이고, 테스트 및 유지 보수가 효율적으로 작동할 수 있도록 한다. 