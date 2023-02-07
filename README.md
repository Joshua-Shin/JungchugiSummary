정보처리기사 요약 정리
-----------
#### 시험개요
- 시험개요 <br> <img width="740" alt="스크린샷 2023-01-29 오후 4 56 51" src="https://user-images.githubusercontent.com/93418349/216806261-712d63eb-37fd-4c86-926e-a8edd7e87c5f.png">
- 14:10 삼육보건대학교H관 CBT2실
- 연습장 달라하면 주는듯 샤프 가져가자.
- 모르는 개념 나오면 유튜브에 "시나공 ㅇㅇㅇ" 이라 치면 잘 나옴

#### 1과목 소프트웨어 설계
- UML 다이어그램, 순차 다이어그램 : 동적임
- 메시지 지향 미들웨어 : 비동기형.
- 비동기형 : 시험지 풀고 체점 하는 방식처럼 주고 받는거.
- 동기형 : 동시에 일어나는.
- 익스트림 프로그래밍 : 애자일 방법론
- 비기능적 요구사항 : 성능, 보안, 품질, 안정..
- 미들웨어 : 클라이언트와 서버 간의 통신을 담당하는 시스템 소프트웨어, 운영체제와 애플리케이션 사이에서 **중간 매개** 역할도.
- 컴포넌트 : 재사용이 가능한 각각의 독립된 **모듈**
- OUI : Organic User Interface. 모든 사물과 사용자 간의 상호작용을 위한 인터페이스
- 액터 : 시스템과 상호작용하는 모든것(사람, 기계, 시스템 등)
- **UML** : 모델링 언어. 요구사항분석과 설계 단계에서 개발자간 의사소통을 위해 사용함. 그 중 유저케이스 다이어그램을 많이 사용.
- 유저케이스 : 구현할 기능, 서비스를 나타냄. 
- 유저케이스간에 점선과 실선으로 **확장관계, 포함관계, 일반화관계**를 표시함.
- ~~일반화관계: 트랜잭션 // 예금, 계좌조회, 인출~~
- ~~포함관계 : 사용자인증 // 시스템 가동, 시스템 종료~~
- ~~확장관계 : 글 작성 // 게시글에 그림 첨부~~
- 디자인 패턴 
  - 객체 지향 프로그래밍 설계를 할 때 자주 발생하는 문제들을 피하기 위해 사용되는 패턴.
  - 생성패턴 : 팩토리, 빌더, 싱글톤, 프로토타입 <br> <img width="640" alt="스크린샷 2023-02-05 오후 4 07 09" src="https://user-images.githubusercontent.com/93418349/216806348-a1c0c417-f2de-457d-a856-19770d1a16e7.png">
- 하향식 vs 상향식 <br> <img width="634" alt="스크린샷 2023-02-06 오후 7 29 03" src="https://user-images.githubusercontent.com/93418349/216948498-90a40f7a-22de-4e91-a7b9-829d9476e301.png">
  - 하향식 설계에서 레벨이 낮은 데이터 구조의 세부 사항은 설계초기 단계에서 필요
  - 기존 컴포넌트들을 조합하여 시스템을 개발하는 경우에는 상향식이 적합
  - 시스템 명세가 명확한 경우와 모든 것을 새로 개발하는 작업에는 하향식이 적합
  - 테스트 드라이버 : 필요한 데이터를 인자를 통하여 넘겨주고, 테스트가 완료된 후 그 결과 값을 받는 역할을 하는 가상의 상위 모듈
  - 테스트 스텁(stub) : a test stub replaces a component during testing to provide controlled and predictable responses.
- 자료 흐름도 <br> <img width="476" alt="스크린샷 2023-02-06 오후 7 33 14" src="https://user-images.githubusercontent.com/93418349/216949363-b45ddba1-deb4-415b-b387-7aa9dff6ddfd.png">
- 목업 vs 프로토타입 : 목업은 실제 작동 안되는거야. 진짜 그냥 시각적인 모형.
- 클래스 설계 원칙 <br> <img width="684" alt="스크린샷 2023-02-06 오후 7 42 59" src="https://user-images.githubusercontent.com/93418349/216951396-409dc329-7eca-4d9c-9eff-4174bda0900e.png">
- 아키텍처 설계과정 : 설계 목표 설정 -> 시스템 타입 결정 -> 아키텍쳐 패턴 적용 (스타일 적용 및 커스터마이즈) -> 서브시스템의 기능, 인터페이스 동작 작성 -> 아키텍처 설계 검토
- 럼바우 방법 <br> <img width="630" alt="스크린샷 2023-02-06 오후 7 51 17" src="https://user-images.githubusercontent.com/93418349/216953125-a34908ba-be92-48f6-ad87-29da8c69f151.png"> <br> 객 동 기
- FEP : Front-End Processor. 입력되는 데이터를 컴퓨터의 프로세서가 처리하기 전에 미리 처리하여 프로세서가 차지하는 시간을 줄여주는 프로그램이나 하드웨어

#### 2과목 소프트웨어 개발
- 워크스루 : 요구사항 명세서 작성자를 포함하여 **사전** 검토한 후에 짧은 검토 회의를 통해 결함을 발견
- 인스펙션 : 요구사항 명세서 작성자를 제외한 다른 검토 전문가들이 요구사항 명세서를 확인하면서 결함을 발견
- 소프트웨어 버전 관리 도구 RCS(revision control system) : 다수의 사용자가 동시에 수정을 할 수 없도록 파일 잠금 방식으로 버전을 관리하는 도구. 다른 방향으로 진행된 개발 결과를 합치거나 변경 내용을 추적 할 수 있다. CVS와의 차이점은 소스파일의 수정을 한 사람만으로 제한한다.
- 블랙박스 테스트 : 프로그램 구조를 고려하지 않는 테스트. 반대는 
- 화이트박스 테스트 : 흐름, 구조, 이런걸 테스트
- 블랙박스 vs 화이트박스 <br> <img width="251" alt="스크린샷 2023-02-06 오후 8 36 38" src="https://user-images.githubusercontent.com/93418349/216961668-3be4c0cb-b5bc-4691-9e8c-16ef5f8cf7e2.png">
- IDE : 배포도 가능
- HttpUnit : 웹 브라우저 없이 **웹 사이트 테스트**를 수행하는데 사용되는 오픈 소스 소프트웨어 테스트 프레임워크
- 스택 : 인터럽트 처리, 서브루틴 호출 작업 등에 응용.
- NS Chart <br> <img width="284" alt="스크린샷 2023-02-06 오후 8 18 45" src="https://user-images.githubusercontent.com/93418349/216958498-37be20d6-9075-4673-9f37-33d062e4ac20.png">
  - 화살표나 goto 사용 안해, 읽기는 쉬운데 작성이 어려워
- 퀵정렬 : 피벗 사용
- 선택정렬 : 배열 내에서 최소값을 찾은 다음 정렬 되지 않은 맨 앞 값과 교환을 하며 정렬을 해 나아가는 방법
- 프로시저 : 일련의 쿼리를 마치 하나의 함수처럼 실행하기 위한 쿼리의 집합
- ISO/IEC 25000 <br> <img width="472" alt="스크린샷 2023-02-07 오후 6 58 30" src="https://user-images.githubusercontent.com/93418349/217212723-6dad5ff7-07b8-453c-bc2d-f1f90694071a.png">


#### 3과목 데이터베이스 구축
- 데이터베이스 정규형
  - 제1정규형 : 한칸에 하나의 데이터만 있는상태
  - 제2정규형 : 부분적 종속성이 있는 상태(= composite primary key가 있을때, 한 필드에만 종속적인 필드가 있는 상태)를 다른 테이블로 나눠서 해결한 상태
  - 제3정규형 : 함수적 종속성(일반 필드에 종속된 필드가 있는 상태)을 해결한 상태
  - BCNF : 모든 '결'정자가 후보키인 정규형
  - 4NF : '다'치종속이 성립하는 경우 테이블의 모든 속성이 함수적 종속 관계를 만족
  - 5NF : 모든 '조'인종속이 테이블의 후보키를 통해서만 성립되는 정규형
- 분산 데이터베이스의 목표
  - 위치 투명성 : 하드웨어와 소프트웨어의 물리적 위치를 사용자가 알 필요 없다.
  - 중복(복제) 투명성 : 사용자에게 통지할 필요 없이 시스템 안에 파일들과 지원들의 부가적인 복사를 자유롭게 할 수 있다.
  - 병행 투명성 : 다중 사용자들이 자원들을 자동으로 공유할 수 있다.
  - 장애 투명성 : 사용자들은 어느 위치의 시스템에 장애가 발생했는지 알 필요가 없다.
 - 트랜잭션 모델링 : 데이터베이스 개념적 설계 단계에서 함
 - DCL : commit, rollback, grant, revoke
- 분산 데이터베이스의 구성 요소 <br> <img width="199" alt="스크린샷 2023-02-07 오후 7 25 42" src="https://user-images.githubusercontent.com/93418349/217219202-c6480b25-6b6b-4238-afbd-5d027b8b702c.png">
- 데이터베이스 병행 제어의 목적 <br> <img width="332" alt="스크린샷 2023-02-07 오후 7 28 23" src="https://user-images.githubusercontent.com/93418349/217219838-90403150-073e-4101-8c6e-c4aeb283ecf4.png">
- 데이터 사전 : 시스템 데이터베이스, 시스템 카탈로그라
고도 함. 메타 데이터를 저장하고 있음. 사용자가 직접 갱신할 수는 없고, 다른 테이블에 변화를 주면 시스템이 자동으로 갱신함.
- 릴레이션 용어 <br> <img width="458" alt="스크린샷 2023-02-05 오후 6 05 40" src="https://user-images.githubusercontent.com/93418349/216810571-b0c1f9f2-244f-4e56-a9e6-c28b049a0c08.png">
- 모든 속성 값은 원자값을 가진다.
- 하나의 릴레이션에서 튜플에 순서는 없다.
- 트랜잭션의 상태 <br> <img width="691" alt="스크린샷 2023-02-05 오후 6 10 34" src="https://user-images.githubusercontent.com/93418349/216810752-c47e9095-1c83-402d-8e62-069ce9f2f1b2.png">
- 슈퍼키 : 유일성은 보장되는데, 최소성은 만족하지 못하는 키네.
- 차수(Degree) : 속성의 수
- 카디널리티(Cardinality) 튜플의 수 (기수)
- 관계해석 <br> <img width="196" alt="스크린샷 2023-02-07 오후 7 08 27" src="https://user-images.githubusercontent.com/93418349/217215215-45069862-9f10-4060-97d2-8fec0f7a7744.png">


#### 4과목 프로그래밍 언어 활용
- strlen, strcpy, strcat, strcmp, strrev(s) : s를 거꾸로 변환
- IP 프로토콜
  - Header Length : IP 프로토콜의 헤더 길이를 32비트 워드 단위로 표시.
    - 32비트 워드 단위 : 1바이트가 8비트. 32비트면 4바이트. int 단위잖어. cpu마다 다르지만 보통 32비트를 1워드로 친대.
  - Packet Length : IP 헤더 및 데이터를 포함한 IP 패킷 전체 길이를 바이트 단위로 길이를 표시. 최대값은 2^16 -1
  - Time To Live : 송신 호스트가 패킷을 전송하기 전 네트워크에서 생존할 수 있는 시간
  - Version Number: IP 프로토콜의 버전번호
  - 주소를 지정하고, 경로를 설정하는 기능을 한다.
  - 체크섬 기능으로 헤더 체크섬만 제공한다
    - 헤더체크섬 : 전송 과정에서 발생할 수 있는 헤더 오류를 검출하는 기능
  - 패킷을 분할, 변합하는 기능을 수행
  - 비연결형 서비스를 제공
  - Best effort 원칙에 따른 전송 기능을 제공  
- 파이썬
  - if, elif, else. // else if 없음
  - 시퀀스 - 리스트 : 순서 있고, 가변
  - 시퀀스 - 튜플 : 순서 있고, 불변
  - 세트 - 세트 : 순서 없고, 중복 x
  - 맵 - 딕셔너리 : 순서 없고, key-value 쌍
- RIP 라우팅 프로토콜 <br> <img width="641" alt="스크린샷 2023-02-05 오후 6 50 27" src="https://user-images.githubusercontent.com/93418349/216812209-669222c2-be97-4bdb-ade6-925613d3fd90.png">
- 각 라우터는 이웃 라우터들로부터 수신한 정보를 이용하여 라우팅 표를 갱신
- RR 스케줄링 : 라운드로빈, 선점 스케줄링 방식. 프로세스가 도착한 순서대로 프로세스를 디스패치하지만 정해진 시간 할당량이 끝나면 뒤로 보냄
- SJF : Shortest Job First, 최소 작업 우선
- HRN 스케줄링 : Highest Response-ratio Next. SJF를 보완하기 위해 나옴. 대기한 시간이 길어질수록 우선순위가 높아짐.
- MQ 스케줄링 : Multi level Queue. 다중레벨 스케줄링. 그 멀티큐로 구성해서 큐마다 다른 스케줄링으로 돌리는거.
- LRU 페이지 교체 알고리즘
  - Least Recently Used. 가장 오랫동안 사용하지 않은 페이지를 교체
  - 결함: 주기억장치의 페이지가 변동되는것
- 유닉스 
  - 서버용 
  - time sharng system을 위해 설계된 대화식 운영체제
  - 이식성. 호환성. C언어. 
  - Multi user, Multi tasking 모두 지원. 
  - 트리구조의 파일시스템
- UDP
  - 비연결형, 비신뢰성 전송 서비스를 제공
  - 흐름 제어나 순서 제어가 없어 전송 속도가 빠르다.
  - 수신된 데이터의 순서 재조정 기능을 지원하지 않는다.
  - 복구 기능을 제공하지 않는다.
  - 단순한 헤더 구조로 오버헤드가 적다.
  - TCP와 같이 트랜스포트(전송) 계층에 존재.
- 응집도와 결합도
  - 응집도: 하나의 모듈이 하나의 기능을 수행하는 요소들간의 연관성 척도. 
    - (강함) 기능적 응집도 > 순차적 > 교환적 > 절차적 > 시간적 > 논리적 > 우연적 응집도 (약함)
    - 기순교절시논우... 다른 기출에서 나오면 외우고 안나오면 버려.
  - 결합도 : 두 모듈간의 상호작용, 또는 의존도 정도를 나타내는 것 <br> <img width="630" alt="스크린샷 2023-02-05 오후 7 34 17" src="https://user-images.githubusercontent.com/93418349/216814037-97a7ce67-7163-4562-8bf2-a385a81f1cb7.png">
  - 응집도는 모듈 내 구성 요소들 간의 이야기이고, 결합도는 모듈과 모듈 사이의 이야기야.
  - 독립적인 모듈이 되기 위해서는 응집도가 강해야 한다. 결합도는 약해야 한다. 
- 사용자 수준에서 지원되는 스레드 : 커널 모드로의 전환 없이 스레드 교환이 가능하므로 오버헤드가 줄어든다.


#### 5과목 정보시스템 구축 관리
- tcp wrapper : TCP 서버에서 네트워크 접근에 대한 필터링을 하는 것. 방화벽과 비슷한 역할
- 기기를 키오스크에 갖다댈때 작동하는 초고속 근접 무선 통신(NFC) 기술 : Zing 지이잉~
- Mesh Network : **그물** 모양의 네트워크 다른 국을 향하는 호출이 중계에 의하지 않고 직접 접속되는.
- Worm : 악성코드. 다른 컴퓨터의 취약점을 이용하여 스스로 전파하거나 메일로 전파되며 스스로를 증식하는 것.
- <br> <img width="640" alt="스크린샷 2023-02-06 오후 6 28 08" src="https://user-images.githubusercontent.com/93418349/216935229-341ab321-316a-429e-bf96-2550e97f2315.png">
- <br> <img width="641" alt="스크린샷 2023-02-06 오후 6 32 34" src="https://user-images.githubusercontent.com/93418349/216936158-2b5ae0aa-c97b-4751-9514-36236a21eac2.png">
- 대칭 암호 알고리즘 : 키 교환 필요, 속도 빠름
- 비대칭 암호 알고리즘 : 공개키 암호라고도 하고. 키 교환 필요 없고. 자신만의 키 사용. 속도 느림
- RBAC : Role Based Access Control 역할 기반 접근 통제
- <br> <img width="400" alt="스크린샷 2023-02-06 오후 6 47 33" src="https://user-images.githubusercontent.com/93418349/216939432-49ca3a40-6b3d-4a53-8c9e-d4d8ebb55563.png">
- Authorization : 권한 부여
- Authentication : 인증
- SDN(Software Definded Networking) : 네트워크를 제어부, 데이터 전달부로 분리하여 네트워크 관리자가 보다 효율적으로 네트워크를 제어, 관리할 수 있는 기술
- ~~Network Mapper : 네트워크 보안을 위한 유틸리티~~
- ~~AOE Network : 수행되는 작업의 각 단계를 정점과 간선으로 나타난 그래프~~
- PERT 차트 : 작업들 간의 상호 관련성, 결정경로, 경계시간, 자원할당 등을 제시하는 네트워크 도표



