# spring-exception
스프링 어노테이션을 활용한 예외처리

# ControllerAdvice, HandlerMapping
1. 전역 예외 처리 가능
2. try-catch 코드보다 간결하게 표현가능

# 구현 방법
- ErrorCode : 에러코드를 enum으로 정의
- EnumModel : 에러코드를 key, value 값으로 가져오기 위한 interface
- ErrorResponse : 에러 vo
- ErrorControllerAdvice : 특정 예외 클래스마다 메소드 지정 > 상세한 에러 핸들링

# 비고
- 적용하려는 프로젝트에 적용불가하여 폐기
- 기존 프로젝트에서 가능한 예외 처리는 3종류
  - return xxx.jsp 직접 에러 페이지 호출
  - dispatcher-servlet에서 resolver
  - web.xml에서 404, 500 등 마지노선 예외 처리 
