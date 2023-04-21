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
- <img width="1440" alt="스크린샷 2023-04-18 오후 6 57 45" src="https://user-images.githubusercontent.com/93418349/232742519-c037a870-e6dc-45d7-bdbf-f28fcd5d8733.png">
- <img width="1440" alt="스크린샷 2023-04-18 오후 6 48 54" src="https://user-images.githubusercontent.com/93418349/232742626-02be5f28-fba9-48fe-98bd-6396303591aa.png">
- sql 에서 distinct : 결과로 표시된 값들 중에서 중복된 값이 있을때 제거. 결과를 낼떄 중복값을 제거하는게 아니라.
<img width="1440" alt="스크린샷 2023-04-18 오후 7 30 22" src="https://user-images.githubusercontent.com/93418349/232756963-f653da9e-32b4-457e-9503-f8ebba9af715.png"> 
<img width="1440" alt="스크린샷 2023-04-18 오후 7 30 55" src="https://user-images.githubusercontent.com/93418349/232757026-e7e8534d-4a79-4543-bb1d-ff38d9922695.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 7 30 47" src="https://user-images.githubusercontent.com/93418349/232757038-b42b8368-fa39-4c33-be98-4b69c47433da.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 7 30 38" src="https://user-images.githubusercontent.com/93418349/232757041-c30d1ae0-eb93-4c0e-9be2-991ea0e4ca7f.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 7 30 29" src="https://user-images.githubusercontent.com/93418349/232757045-301b82e0-de27-4a96-ad4e-c32ac2080dc0.png">
<img width="1440" alt="스크린샷 2023-04-18 오후 7 29 44" src="https://user-images.githubusercontent.com/93418349/232757132-6a8fc2a8-907b-409b-959f-9992257ec0e6.png">
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

----------------------------------
<img width="1440" alt="스크린샷 2023-04-19 오후 6 35 35" src="https://user-images.githubusercontent.com/93418349/233085830-4d9e7958-07b4-456f-a242-a0983f0d3dc5.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 44 17" src="https://user-images.githubusercontent.com/93418349/233085850-cf9f7b37-cb0c-4d4c-b7e5-e837680da9e3.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 52 13" src="https://user-images.githubusercontent.com/93418349/233085855-921e2554-7726-44dd-94b3-88d3965c44e0.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 52 21" src="https://user-images.githubusercontent.com/93418349/233085859-4b7b3f2a-aa98-4f43-80c0-57a4feb9642f.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 52 33" src="https://user-images.githubusercontent.com/93418349/233085861-8f7443e1-728c-433c-afaa-92dfe9688ec4.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 53 57" src="https://user-images.githubusercontent.com/93418349/233085866-6a4a47ac-70fb-4746-8a5b-5d009ca90538.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 6 56 10" src="https://user-images.githubusercontent.com/93418349/233085870-afb0b9f8-9368-4e16-9787-2dc76e5516d9.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 24 46" src="https://user-images.githubusercontent.com/93418349/233085875-b6cf7e68-80aa-438f-985a-f80c7f6d8a64.png">
<img width="703" alt="스크린샷 2023-04-19 오후 7 27 49" src="https://user-images.githubusercontent.com/93418349/233085879-154086a4-aca2-4d29-8c9b-78a4e6997a86.png">
<img width="724" alt="스크린샷 2023-04-19 오후 7 27 55" src="https://user-images.githubusercontent.com/93418349/233085885-f233cbd3-b1ac-4774-a215-c94069649b01.png">
<img width="726" alt="스크린샷 2023-04-19 오후 7 28 20" src="https://user-images.githubusercontent.com/93418349/233085893-6436c300-2d79-4cfc-991f-5e0dfa2969fd.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 31 12" src="https://user-images.githubusercontent.com/93418349/233085899-1788c212-83ed-4f7c-81b0-6c03617c3ca1.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 32 15" src="https://user-images.githubusercontent.com/93418349/233085902-be4e1e18-ca0a-479a-858f-4c573e10a770.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 35 38" src="https://user-images.githubusercontent.com/93418349/233085907-61119ace-cdc6-4d75-b112-a8c0f55604a5.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 53 07" src="https://user-images.githubusercontent.com/93418349/233085912-76d1ce9e-3104-4300-a8ae-bdb91ddc0a90.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 55 11" src="https://user-images.githubusercontent.com/93418349/233085915-b281d86f-b635-4bd3-bafb-e35c6101ffe9.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 7 58 13" src="https://user-images.githubusercontent.com/93418349/233085919-3aad41c2-e903-40d8-85fa-9fbd1f39cd50.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 00 03" src="https://user-images.githubusercontent.com/93418349/233085921-c47f5f74-056b-463e-b72b-d7f1d729b01b.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 04 29" src="https://user-images.githubusercontent.com/93418349/233085927-764f906b-ba7f-44ec-8352-f82bee3e30b0.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 38 00" src="https://user-images.githubusercontent.com/93418349/233085928-192b8259-fab6-4343-944a-397de8186de6.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 40 14" src="https://user-images.githubusercontent.com/93418349/233085929-c847ea83-fda4-4bba-8ad7-9d99d662f18f.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 41 43" src="https://user-images.githubusercontent.com/93418349/233085934-fe8544bf-5ef1-4b21-84db-5bf61c0422aa.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 42 56" src="https://user-images.githubusercontent.com/93418349/233085939-ae1b4074-daf5-4f8c-b651-20d03951c38e.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 46 08" src="https://user-images.githubusercontent.com/93418349/233085943-c31c86ee-bf6f-475a-8c04-ad272bc832c1.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 46 42" src="https://user-images.githubusercontent.com/93418349/233085945-a52c04f9-2788-4f74-adca-199d03a056a7.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 8 57 45" src="https://user-images.githubusercontent.com/93418349/233085950-28ac9c6a-76c1-4336-acda-0441c683b624.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 05 57" src="https://user-images.githubusercontent.com/93418349/233085951-ae1e9e13-db75-4d79-b866-8f1c013af4a5.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 06 06" src="https://user-images.githubusercontent.com/93418349/233085956-d22c8405-f4dd-4b68-b83d-45f2322ac35f.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 07 43" src="https://user-images.githubusercontent.com/93418349/233085959-44a187af-aad0-49d2-9fe4-4f2a7c3e64ae.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 16 47" src="https://user-images.githubusercontent.com/93418349/233085965-139cf5da-886f-43fc-8521-d4c34d898e95.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 29 04" src="https://user-images.githubusercontent.com/93418349/233085970-8bbe2bcc-888b-483a-9a09-9342d880d6d3.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 31 15" src="https://user-images.githubusercontent.com/93418349/233085973-9c179b1a-7760-483d-893b-4c05e803ebbf.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 9 32 02" src="https://user-images.githubusercontent.com/93418349/233085979-0b38f60f-b0ca-4225-bb5a-9e742640392c.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 10 01 03" src="https://user-images.githubusercontent.com/93418349/233085985-625e0d56-c8f8-4ba9-848c-ffd341b8bb8c.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 10 09 32" src="https://user-images.githubusercontent.com/93418349/233085987-5f1c2faa-c2a5-47ce-a345-738f3567770d.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 10 13 03" src="https://user-images.githubusercontent.com/93418349/233085993-3bce9d19-7478-42e8-9f7f-e71462794124.png">

----------------------------------
<img width="1440" alt="스크린샷 2023-04-19 오후 10 54 30" src="https://user-images.githubusercontent.com/93418349/233629994-cb1b8f85-583d-4295-8bd4-a89ed7de0c96.png">
<img width="1440" alt="스크린샷 2023-04-19 오후 11 01 32" src="https://user-images.githubusercontent.com/93418349/233630003-c6de4b7e-8b41-42a5-90e6-adaa8945d047.png">
<img width="1440" alt="스크린샷 2023-04-20 오후 3 32 40" src="https://user-images.githubusercontent.com/93418349/233630006-5fa149ca-6b4c-454f-9513-761ba7a56d1e.png">
<img width="1440" alt="스크린샷 2023-04-20 오후 3 43 41" src="https://user-images.githubusercontent.com/93418349/233630008-cdf7c25b-eb28-4b62-8777-70e6489c70a4.png">
<img width="1440" alt="스크린샷 2023-04-20 오후 3 47 04" src="https://user-images.githubusercontent.com/93418349/233630020-7c6ce93f-2626-4bec-8ead-ce214a55dba0.png">
<img width="1440" alt="스크린샷 2023-04-20 오후 3 50 53" src="https://user-images.githubusercontent.com/93418349/233630026-6ecb00bc-080c-40d0-87c5-d44617a7d427.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 09 10" src="https://user-images.githubusercontent.com/93418349/233630030-ba998452-e89a-4b62-a4fc-653ece6c5828.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 12 38" src="https://user-images.githubusercontent.com/93418349/233630037-3720aac1-aad3-4e9c-8133-d128a9233588.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 18 50" src="https://user-images.githubusercontent.com/93418349/233630042-058703fe-cc43-47d2-b206-0d7456a5ccb8.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 22 12" src="https://user-images.githubusercontent.com/93418349/233630044-539ead7f-67f3-420a-a0c7-b1225608e153.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 27 25" src="https://user-images.githubusercontent.com/93418349/233630051-b8eebbfe-6102-44bb-b566-629a0c387a5a.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 28 32" src="https://user-images.githubusercontent.com/93418349/233630056-bf44ffae-ffad-480a-9ead-d9637d842925.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 29 08" src="https://user-images.githubusercontent.com/93418349/233630059-22ba4519-3225-47c2-949c-c119bed3d7f3.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 32 15" src="https://user-images.githubusercontent.com/93418349/233630063-b8ae60d2-fe41-4ab2-bcc3-b1dd8d57f596.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 40 30" src="https://user-images.githubusercontent.com/93418349/233630065-1fa801a4-d3c2-42f2-b626-97c71ddf1db0.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 46 17" src="https://user-images.githubusercontent.com/93418349/233630070-1f56c191-5f0f-4bc1-8a84-ca84ac608d26.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 48 51" src="https://user-images.githubusercontent.com/93418349/233630071-b9b8c679-8878-460f-aa4c-9b512554bb93.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 51 37" src="https://user-images.githubusercontent.com/93418349/233630074-53410ce7-65e4-4509-9e79-65b11a9e1cbd.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 57 00" src="https://user-images.githubusercontent.com/93418349/233630078-bffb5a71-2876-4225-9f21-28f81cec8230.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 58 51" src="https://user-images.githubusercontent.com/93418349/233630080-fb514e61-0dba-4cbf-b48d-3bdc00ec657a.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 59 01" src="https://user-images.githubusercontent.com/93418349/233630084-f3a79c3e-95f7-4b41-8886-1be1c6582fc4.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 4 59 51" src="https://user-images.githubusercontent.com/93418349/233630086-db874492-8f0e-4935-a432-3918a0eea1d3.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 01 16" src="https://user-images.githubusercontent.com/93418349/233630089-6bd13fc5-d76d-474b-bc13-7c9a6f51d1bc.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 23 41" src="https://user-images.githubusercontent.com/93418349/233630091-a21eca12-ab9d-4835-b23a-61a8e39fa9c5.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 25 25" src="https://user-images.githubusercontent.com/93418349/233630096-12f5473b-53e9-4f3f-9c2e-9eb1a3380520.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 28 59" src="https://user-images.githubusercontent.com/93418349/233630101-e9672232-8d79-4614-9086-6c636332bcc7.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 29 39" src="https://user-images.githubusercontent.com/93418349/233630102-1972e56e-0cde-4552-b27a-96390694df8d.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 31 44" src="https://user-images.githubusercontent.com/93418349/233630103-ff6bb292-84a3-4f51-9599-7311e1f9393e.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 5 33 29" src="https://user-images.githubusercontent.com/93418349/233630112-025fb2f2-94e7-49a1-b891-8eb6fb3fbbd1.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 8 49 43" src="https://user-images.githubusercontent.com/93418349/233630114-88e6e118-5d0d-4be9-aa45-bb4105c363af.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 8 50 56" src="https://user-images.githubusercontent.com/93418349/233630115-f69c3a10-7f8a-4adf-bf95-cef8b03f9c8d.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 8 56 03" src="https://user-images.githubusercontent.com/93418349/233630116-1dd3feab-8689-40d7-952b-6191eeb42ede.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 8 56 23" src="https://user-images.githubusercontent.com/93418349/233630121-90250b60-46e3-4754-8a6f-72434158a2a1.png">




