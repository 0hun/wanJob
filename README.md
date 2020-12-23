# wanJob
+ 구직 지원을 하고 구직 조회를 제공하는 서버입니다.
+ 회사 지원, 회사 조회 기능을 직접 구현함으로써 대규모 트래픽에도 견고한 어플레이션을 구현할 수 있도록 하고 있습니다.

## wanJob

## 기능

### 사용자
+ 이력서 등록, 수정, 삭제(이력서 양식에 맟춰 넣기 or 파일 업로드)
+ 회원 가입, 수정, 탈퇴
+ 회사 지원(회사 지원시 회사 및 지원자에게 메일 및 알림 전송)
+ 프로필 수정

### 회사
+ 회사 가입, 수정, 탈퇴
+ 회사 등록, 삭제, 검색
+ 채용 합격, 탈락(합격 및 탈락 처리시 지원자에게 메일 전송 및 알림 전송)

### 관리자
+ 사용자 추가, 등록, 삭제
+ 회사 등록, 삭제, 검색
+ 공지사항 및 이벤트 등록
+ 최종 합격 후(약 3개월이 지난 후에 보상금 받도록 처리)
+ 회사 및 지원자에게 매칭 시스템(분야 및 경력, 조건에 맞는 회사 및 지원자를 찾은 후 추천 메일 전송)

### 사용 기술
+ Spring Boot, Maven, jpa, mysql, Redis, Java11, rest-api, docker,kubernetes, jenkins

### 기술적인 집중 요소
+ 객체지향의 기본 원리와 spring의 IOC/DI , AOP, PSA 활용과 의미 있는 코드 작성
+ 라이브러리 및 기능 추가시 이유있는 선택과 사용 목적 고려

### 브렌치 관리 전략
Git Flow를 사용하여 branch를 관리   
모든 branch는 pull request 리뷰 완료후 merge   

![git-flow-strategy](https://user-images.githubusercontent.com/29122916/83837107-79166100-a730-11ea-8744-3761ad01ca96.png)

+ master: 개발, 테스트 완료후 검증이 완료된 코드가 있는 branch
+ develop: 개발이 끝난후 issue branch를 merge
+ issue(feature): develop에서 새로운 기능을 개발 진행
+ release: issue에서 develop으로 merge하여 master에 merge전 배포하여 테스트를 진행
+ hot-fix: release, master에서 발생한 버그를 수정

> #### 브렌치 관리 전략 참고 문헌
+ https://riptutorial.com/ko/git/example/4182/gitflow-%EC%9B%8C%ED%81%AC-%ED%94%8C%EB%A1%9C%EC%9A%B0

### ERD




