정보처리기사 요약 정리(실기)
-----------
- 관계대수: 관계 대수는 관계형 데이터베이스에서 원하는 정보와 그 정보를 어떻게 유도하는가를 기술하는 절차적 언어이다.
  - 순수 관계 연산자
    - Select: Select의 기호는 σ(그리스 문자 시그마)이며,  릴레이션에서 조건에 맞게 수평으로 또는 행에 해당하는 튜플을 구한다.
    - Project: Project의 기호는 π(그리스 문자 파이)이며, 릴레이션에서 조건에 맞게 수직으로 또는 열에 해당하는 튜플을 구한다.
    - Join: Join의 기호는 ⋈이며, 공통 속성을 중심으로 2개의 릴레이션을 하나로 합쳐서 새로운 릴레이션을 만든다.
    - Division: 기호는 ÷ 이며, 릴레이션 R,S가 있을 때, R⊃S인 경우, S의 속성값을 모두 가진 튜플에서, S의 속성 값을 가진 것만 제외한것 
  - 일반 집합 연산자
    - 합집합(Union): 기호는 ∪ 이며, 두 릴레이션에 존재하는 튜플의 합집합을 구한다. 
    - 교집합(Intersection): 기호는 ∩ 이며, 두 릴레이션에 존재하는 튜플의 교집합을 구한다.  
    - Difference: 기호는 － 이며, 두 릴레이션의 차집합을 구한다.   
    - Cartesian Product: 기호는 × 이며, 두 릴레이션에 존재하는 튜플들의 결합된 정보를 구하는 연산이다.

- 디자인 패턴
  - 1_ 생성
    -  추상 팩토리 (Abstract Factory): 생성군들을 하나의 모아놓고 팩토리 중에서 선택하게 하는 패턴
    -  Factory Method : 객체를 생성하기 위한 인터페이스를 정의하여 어떤 클래스가 인스턴스화 될 것인지는 서브 클래스가 결정하도록 하는 패턴
    -  Builder : 생산 단계를 캡슐화 하여 구축 공정을 동일하게 이용하도록 하는 패턴
    -  Singleton : 유일한 하나의 인스턴스를 보장하도록 하는 패턴
    -  Prototype : 복사하여 새 개체를 생성할 수 있도록 하는 패턴
  - 2_ 구조
    - Adapter : 인터페이스로 인해 함께 사용하지 못하는 클래스를 함께 사용하도록 하는 패턴
    - Bridge : 추상과 구현을 분리하여 결합도를 낮춘 패턴
    - Composite : 개별 객체와 복합 객체를 클라이언트에서 동일하게 사용하도록 하는 패턴
    - Decorator : 소스를 변경하지 않고 기능을 확장하도록 하는 패턴
    - Facade : 하나의 인터페이스를 통해 느슨한 결합을 제공하는 패턴
    - Proxy : 대리인이 대신 그 일을 처리하는 패턴
    - Flyweight : 대량의 작은 객체들을 공유하는 패턴
  - 3_ 행위
    - Chain of Responsibility : 객체들끼리 연결 고리를 만들어 내부적으로 전달하는 패턴
    - Command : 요청 자체를 캡슐화하여 파라미터로 넘기는 패턴
    - Interpreter : 언어 규칙 클래스를 이용하는 패턴
    - Iterator : 내부 표현은 보여주지 않고 순회하는 패턴
    - Mediator : 객체 간 상호작용을 캡슐화한 패턴
    - Memento : 상태 값을 미리 저장해 두었다가 복구하는 패턴
    - Observer : 상태가 변할 때 의존자들에게 알리고, 자동 업데이트하는 패턴
    - State : 객체 내부 상태에 따라서 행위를 변경하는 패턴
    - Strategy : 다양한 알고리즘 캡슐화하여 알고리즘 대체가 가능하도록 한 패턴
    - Template Method : 알고리즘 골격의 구조를 정의한 패턴
    - Visitor : 오퍼레이션을 별도의 클래스에 새롭게 정의한 패턴
- 192.168.1.0/24 네트워크를 FLSM 방식으로 3개의 subnet으로 나눌떄 두번째 네트워크의 브로드캐스트 ip주소를 써라
  - '/24' 의미 : 앞 24비트는 고정값이니, 마지막 8비트까지고 나눠라.
  - subnet은 2의배수로 나눌 수 있음. -> 3개로 나누고싶다면 4개로 나눠야함.
  - 8비트는 0000000부터  11111111까지 즉 0부터 255까지의 수임.
  - 이걸 4등분하면 64.
  - 즉 0\~63, 64\~127, 128\~192, 192\~255 로 나뉘고 순차적으로 첫번째부터 네번째 네트워크가됨.
  - 4등분된 각각의 네트워크의 시작값은 네트워크ip주소가 되고, 끝값은 브로드캐스트ip주소가됨.
  - 즉, 두번째 네트워크의 브로드캐스트 ip주소는 127임.
  - 정답: 192.168.1.127
- 블랙박스 vs 화이트박스
  - 블랙박스 테스트 <br> <img width="800" alt="스크린샷 2023-04-18 오후 6 57 45" src="https://user-images.githubusercontent.com/93418349/232742519-c037a870-e6dc-45d7-bdbf-f28fcd5d8733.png">
  - 화이트박스 테스트 <br> <img width="800" alt="스크린샷 2023-04-18 오후 6 48 54" src="https://user-images.githubusercontent.com/93418349/232742626-02be5f28-fba9-48fe-98bd-6396303591aa.png">
- sql 에서 distinct : 결과로 표시된 값들 중에서 중복된 값이 있을때 제거. 결과를 낼떄 중복값을 제거하는게 아니라.
- 네트워크 침해
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 30 22" src="https://user-images.githubusercontent.com/93418349/232756963-f653da9e-32b4-457e-9503-f8ebba9af715.png"> 
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 30 55" src="https://user-images.githubusercontent.com/93418349/232757026-e7e8534d-4a79-4543-bb1d-ff38d9922695.png">
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 30 47" src="https://user-images.githubusercontent.com/93418349/232757038-b42b8368-fa39-4c33-be98-4b69c47433da.png">
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 30 38" src="https://user-images.githubusercontent.com/93418349/232757041-c30d1ae0-eb93-4c0e-9be2-991ea0e4ca7f.png">
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 30 29" src="https://user-images.githubusercontent.com/93418349/232757045-301b82e0-de27-4a96-ad4e-c32ac2080dc0.png">
- Python 
  - <img width="800" alt="스크린샷 2023-04-18 오후 7 29 44" src="https://user-images.githubusercontent.com/93418349/232757132-6a8fc2a8-907b-409b-959f-9992257ec0e6.png">
- 
<img width="1440" alt="스크린샷 2023-04-18 오후 8 05 51" src="https://user-images.githubusercontent.com/93418349/232775601-d7c624f7-0ea7-4cc7-b80b-257d44967e6e.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 06 42" src="https://user-images.githubusercontent.com/93418349/232775655-4defc3d4-b6ee-4a07-8faf-ae956ffa09f8.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 11 24" src="https://user-images.githubusercontent.com/93418349/232775663-4c80ef82-05d4-424c-9bb7-0b708babdb4f.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 15 39" src="https://user-images.githubusercontent.com/93418349/232775673-95539955-e290-44c0-bc5e-62f851351b57.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 15 47" src="https://user-images.githubusercontent.com/93418349/232775677-b9ad2a44-154a-4cf8-a561-ebc6f0bbd513.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 22 33" src="https://user-images.githubusercontent.com/93418349/232775682-74db8308-55e6-40f1-bb00-48e59a5ceec5.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 23 26" src="https://user-images.githubusercontent.com/93418349/232775685-4ae5227b-07c4-438e-8282-400e7e73cf64.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 24 08" src="https://user-images.githubusercontent.com/93418349/232775686-cb93ca6d-1cf5-4d83-995d-ffb0257084e2.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 25 49" src="https://user-images.githubusercontent.com/93418349/232775688-075d70ae-402a-4960-912a-bbbd2d96cf03.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 29 16" src="https://user-images.githubusercontent.com/93418349/232775690-e2e279ec-96a5-412f-8440-1d461fffd1ab.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 30 47" src="https://user-images.githubusercontent.com/93418349/232775695-8eb50220-7788-4065-9794-c77d08cbdd3d.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 32 59" src="https://user-images.githubusercontent.com/93418349/232775698-97d2ae4a-cb16-4bd9-b5d9-8e9b87d3fb5b.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 34 58" src="https://user-images.githubusercontent.com/93418349/232775701-b1d077b9-46dd-4ef0-bbfb-3932852b3b8b.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 36 07" src="https://user-images.githubusercontent.com/93418349/232775704-99fa8947-b2eb-4012-bd56-ef3e56f07059.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 37 19" src="https://user-images.githubusercontent.com/93418349/232775705-f979c6aa-147b-493f-9bac-862c391dc31c.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 38 32" src="https://user-images.githubusercontent.com/93418349/232775708-14bc0ffa-a425-471c-a6c7-700a98d09e85.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 40 11" src="https://user-images.githubusercontent.com/93418349/232775710-15b41dc2-c229-4372-9b33-3786dce4c551.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 42 08" src="https://user-images.githubusercontent.com/93418349/232775716-ddb4f6b5-bb31-4939-bf1a-ed1363963bc1.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 43 21" src="https://user-images.githubusercontent.com/93418349/232775719-347d1f9e-4299-4723-a7a8-e80b205f8351.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 44 40" src="https://user-images.githubusercontent.com/93418349/232775721-e9fb394a-9660-4117-a4b3-9d4100979e33.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 45 28" src="https://user-images.githubusercontent.com/93418349/232775724-43002d29-b33e-4f77-b7e2-4ca685887439.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 47 28" src="https://user-images.githubusercontent.com/93418349/232775727-c21675f6-3f15-45d5-a18b-720327920a82.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 48 00" src="https://user-images.githubusercontent.com/93418349/232775735-eb811e4e-255c-4bde-b6bc-7b70bcd8dd33.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 8 53 15" src="https://user-images.githubusercontent.com/93418349/232775740-8428d6eb-5b7f-49e2-9fb4-276ba5f61635.png">

