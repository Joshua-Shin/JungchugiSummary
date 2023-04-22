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
<!--
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
-->
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

---------------------------------------
<img width="1440" alt="스크린샷 2023-04-21 오후 9 07 24" src="https://user-images.githubusercontent.com/93418349/233652300-327e4a9c-b392-4ad0-9f22-3b7d0adbf084.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 08 47" src="https://user-images.githubusercontent.com/93418349/233652348-27d8c6a1-9561-4fb1-b85a-856620338d7d.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 12 52" src="https://user-images.githubusercontent.com/93418349/233652362-bfe4d67b-0f99-4836-99d6-9777a7366f21.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 13 07" src="https://user-images.githubusercontent.com/93418349/233652369-97709ce7-cbee-4d61-8829-63970a1f5768.png">
<img width="775" alt="스크린샷 2023-04-21 오후 9 13 12" src="https://user-images.githubusercontent.com/93418349/233652371-46bcc582-9131-4733-a0cd-499a9b523fd6.png">
<img width="780" alt="스크린샷 2023-04-21 오후 9 13 16" src="https://user-images.githubusercontent.com/93418349/233652375-ca2bf2f1-e2bd-40de-9024-ce2e81716c23.png">
<img width="841" alt="스크린샷 2023-04-21 오후 9 24 33" src="https://user-images.githubusercontent.com/93418349/233652378-6ca12b4e-fdc0-4850-bba0-21c441df8174.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 25 00" src="https://user-images.githubusercontent.com/93418349/233652383-5ba93c3b-b25b-467e-8cf4-51070a1d6b15.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 26 06" src="https://user-images.githubusercontent.com/93418349/233652388-0564d5ce-fac7-46ba-852d-e9a74aa35358.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 32 28" src="https://user-images.githubusercontent.com/93418349/233652399-724df095-e12e-46bd-89e3-92c11d3966b4.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 9 37 25" src="https://user-images.githubusercontent.com/93418349/233652404-ab61447f-408c-432a-93ca-8f1b1328f251.png">
<img width="785" alt="스크린샷 2023-04-21 오후 9 58 55" src="https://user-images.githubusercontent.com/93418349/233652408-62244e57-f3b1-4613-aee0-a63c1c90bab5.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 00 32" src="https://user-images.githubusercontent.com/93418349/233652411-3eb1bf36-e571-4e0c-9070-851afa461ae1.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 09 36" src="https://user-images.githubusercontent.com/93418349/233652417-f2e1fb94-47ec-409c-aa30-57b152d4beac.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 10 52" src="https://user-images.githubusercontent.com/93418349/233652428-4cd3d2cb-fbe8-470a-88d6-61efe2b368f6.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 10 53" src="https://user-images.githubusercontent.com/93418349/233652434-66c53faa-319e-48a3-a653-8cb9deb68a35.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 12 01" src="https://user-images.githubusercontent.com/93418349/233652436-414ac9ae-8081-4111-a33c-df37812ba7b0.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 12 53" src="https://user-images.githubusercontent.com/93418349/233652437-80311535-316b-44ce-95d8-3d5314083d3a.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 13 30" src="https://user-images.githubusercontent.com/93418349/233652442-83444bae-3ab7-4c06-a077-242bcef7d83a.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 28 18" src="https://user-images.githubusercontent.com/93418349/233652443-6701df8e-74fc-412d-ac3b-bb636f3c34f0.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 28 31" src="https://user-images.githubusercontent.com/93418349/233652448-8b9fb18a-6170-4dda-9823-d76ad42d6c58.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 29 45" src="https://user-images.githubusercontent.com/93418349/233652452-c36beb36-3134-4bd6-b716-86e6d27288f0.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 30 33" src="https://user-images.githubusercontent.com/93418349/233652458-e0b598eb-7529-4de6-9a54-45a894b18e23.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 31 14" src="https://user-images.githubusercontent.com/93418349/233652461-9369a5a6-c0b8-4cec-ada3-ca5dbe98397e.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 32 15" src="https://user-images.githubusercontent.com/93418349/233652463-dabe0bd3-7e11-4faa-91f5-7148b1fe99c5.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 33 32" src="https://user-images.githubusercontent.com/93418349/233652464-82e42f0e-db5d-45cb-be40-2a1d08580b19.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 35 06" src="https://user-images.githubusercontent.com/93418349/233652467-b9e7d67c-aacf-4d32-a734-3fbaa6667c2a.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 36 43" src="https://user-images.githubusercontent.com/93418349/233652468-b67f9cd5-d3cb-4609-b652-5a7e04404110.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 39 19" src="https://user-images.githubusercontent.com/93418349/233652469-c9ea84af-8d48-4f13-9c17-da0bbc0303bc.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 40 11" src="https://user-images.githubusercontent.com/93418349/233652471-f6af624e-c4ff-4179-97f7-191944ef2cc4.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 42 35" src="https://user-images.githubusercontent.com/93418349/233652476-2a9b365b-16f1-40f1-9537-f86a4ffc288c.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 44 07" src="https://user-images.githubusercontent.com/93418349/233652477-5fb5299d-1132-4495-866b-5a84d171d086.png">

-------------------------------------------
<img width="1440" alt="스크린샷 2023-04-21 오후 10 48 58" src="https://user-images.githubusercontent.com/93418349/233768006-b93f21b6-88da-4904-82a5-aed2f869f9bb.png">
<img width="1440" alt="스크린샷 2023-04-21 오후 10 52 00" src="https://user-images.githubusercontent.com/93418349/233768007-f6a69b46-aedb-4dda-8bcf-33577c791b7d.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 2 37 26" src="https://user-images.githubusercontent.com/93418349/233768009-54c9ce31-dd7d-406d-b877-f31b96a7305a.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 2 39 11" src="https://user-images.githubusercontent.com/93418349/233768011-139d1300-9492-486f-89d2-cb2d3d3a1927.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 2 53 04" src="https://user-images.githubusercontent.com/93418349/233768014-35c3ab7b-37da-4f0d-8f3f-24393c6fd5bc.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 2 55 53" src="https://user-images.githubusercontent.com/93418349/233768016-b42ca750-9ca0-48e5-8b89-ec639bc3653a.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 2 59 33" src="https://user-images.githubusercontent.com/93418349/233768018-d95b3aeb-8ce6-414f-a03d-7d9b60b7f234.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 02 47" src="https://user-images.githubusercontent.com/93418349/233768019-621c83c8-665c-47cf-b351-366923bdf8ee.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 05 06" src="https://user-images.githubusercontent.com/93418349/233768020-c96ec9a5-7d6b-47b4-808c-279c730a84ed.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 07 31" src="https://user-images.githubusercontent.com/93418349/233768022-487c9470-86f6-498b-8fad-078d3630daea.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 10 23" src="https://user-images.githubusercontent.com/93418349/233768023-00a9d9f7-7a63-4696-b2e0-44916803373e.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 12 47" src="https://user-images.githubusercontent.com/93418349/233768024-adab6e71-7a5b-4847-9eb5-dfaafed93cf4.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 13 35" src="https://user-images.githubusercontent.com/93418349/233768025-f1a77920-30e5-442a-8b28-574fefe3a505.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 13 36" src="https://user-images.githubusercontent.com/93418349/233768026-f4555411-1bfb-4144-b396-03e98448239a.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 21 35" src="https://user-images.githubusercontent.com/93418349/233768027-4c8443b7-1a5f-4122-93f0-38fa1a7be30d.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 23 20" src="https://user-images.githubusercontent.com/93418349/233768028-d4ed563a-32de-42bd-9ea5-9334367f4053.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 37 39" src="https://user-images.githubusercontent.com/93418349/233768030-3f3caa81-5bf1-45b1-9d4f-0e303d80a1e5.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 42 32" src="https://user-images.githubusercontent.com/93418349/233768032-2cb86886-ab70-4eae-8256-6d93fb674162.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 43 24" src="https://user-images.githubusercontent.com/93418349/233768033-01ae090b-e4b5-4a89-aeab-6294250b9aee.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 51 25" src="https://user-images.githubusercontent.com/93418349/233768034-bf10a16d-d580-4057-a8e5-505ffe7a595d.png">

-----------------------------------
<img width="1440" alt="스크린샷 2023-04-22 오후 3 54 17" src="https://user-images.githubusercontent.com/93418349/233773835-661875e6-abd7-4eb4-b4e7-49e73ab9c021.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 3 58 28" src="https://user-images.githubusercontent.com/93418349/233773843-0c1bb6e0-d25d-41c8-aa86-d3d105f4e207.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 01 09" src="https://user-images.githubusercontent.com/93418349/233773846-a3bd86f2-eeb7-4615-857d-8f624f0893c2.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 18 18" src="https://user-images.githubusercontent.com/93418349/233773847-221c3c95-1eed-4578-addb-c0e9cfd287f5.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 20 36" src="https://user-images.githubusercontent.com/93418349/233773848-35d7ff8d-7500-4b14-bb19-c82b416b7261.png">
<img width="1022" alt="스크린샷 2023-04-22 오후 4 28 28" src="https://user-images.githubusercontent.com/93418349/233773850-55ed7cf0-94da-40ac-9a72-985906c6b885.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 31 53" src="https://user-images.githubusercontent.com/93418349/233773852-742887a7-69f7-46a2-9016-500ba3066e90.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 46 26" src="https://user-images.githubusercontent.com/93418349/233773853-211fb808-97dd-4190-9a82-3858adb5a9b4.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 46 40" src="https://user-images.githubusercontent.com/93418349/233773855-00b60dab-5a6d-4bfd-9219-ee9a1f0355f9.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 49 25" src="https://user-images.githubusercontent.com/93418349/233773857-293989f6-5aaa-4a8b-a99c-ad7ff5b885f7.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 51 08" src="https://user-images.githubusercontent.com/93418349/233773858-f1eb49fa-7a3b-4083-88fd-9a0734ec777f.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 54 18" src="https://user-images.githubusercontent.com/93418349/233773859-b8f2dc34-f82b-42e0-b057-168f40834b8f.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 56 08" src="https://user-images.githubusercontent.com/93418349/233773860-98259480-c934-4c53-88a7-34147305cb88.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 4 58 39" src="https://user-images.githubusercontent.com/93418349/233773861-bd257e69-d142-435b-b087-37b524328bd4.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 00 38" src="https://user-images.githubusercontent.com/93418349/233773862-b79cd943-9c5d-457a-aa81-0e53f610c526.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 07 41" src="https://user-images.githubusercontent.com/93418349/233773865-6311c169-3ce8-4860-9306-95926f378413.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 08 26" src="https://user-images.githubusercontent.com/93418349/233773866-10eeb406-be7e-4b19-82fd-2b544e1d2fcc.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 08 51" src="https://user-images.githubusercontent.com/93418349/233773867-eee1b1d1-5a3f-4789-a55b-ccbccff9d122.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 20 13" src="https://user-images.githubusercontent.com/93418349/233773868-02696d05-80b7-467a-8f67-5f65189a8bed.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 21 48" src="https://user-images.githubusercontent.com/93418349/233773870-431debf1-ee68-4740-8ec3-befe074b0a41.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 22 41" src="https://user-images.githubusercontent.com/93418349/233773872-2e41b531-d36a-48a2-938d-29e0ee0f48f9.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 23 10" src="https://user-images.githubusercontent.com/93418349/233773873-fa2de6ae-edb6-4e8c-a33c-18fb0d92b7dd.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 23 38" src="https://user-images.githubusercontent.com/93418349/233773874-3a0df6ff-5cc6-4b56-9592-e13d4281828f.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 24 21" src="https://user-images.githubusercontent.com/93418349/233773875-db9e1652-1aeb-4feb-b9f6-9e8fe58001a9.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 25 33" src="https://user-images.githubusercontent.com/93418349/233773876-fe980f74-60e6-4df4-a40a-f06ce1620710.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 29 15" src="https://user-images.githubusercontent.com/93418349/233773877-b516673d-dc01-4bf3-8315-261fd654b5d6.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 30 37" src="https://user-images.githubusercontent.com/93418349/233773878-a867694d-eff5-4300-9547-053a3fb17681.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 31 50" src="https://user-images.githubusercontent.com/93418349/233773880-75ebbe8f-ddd8-4228-8c78-5cdf982d30ee.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 34 45" src="https://user-images.githubusercontent.com/93418349/233773882-4eed87f8-a3d4-429b-b299-f836eff426b5.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 36 48" src="https://user-images.githubusercontent.com/93418349/233773884-7322f377-c519-476e-9eb8-50d5121f0d0a.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 38 16" src="https://user-images.githubusercontent.com/93418349/233773885-b9d814c1-2aac-4803-ac9e-8c262e75bfc5.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 38 57" src="https://user-images.githubusercontent.com/93418349/233773886-07000e20-91e4-4c3b-ade3-e6205fe17b92.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 41 34" src="https://user-images.githubusercontent.com/93418349/233773887-849d9b93-0d90-4e0d-887e-d0b42a675958.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 44 13" src="https://user-images.githubusercontent.com/93418349/233773889-1f639401-937c-43f0-98a1-65d0511243cb.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 45 32" src="https://user-images.githubusercontent.com/93418349/233773890-d75e4d88-4ba1-4812-b13d-48227f3a01b9.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 46 15" src="https://user-images.githubusercontent.com/93418349/233773893-04bb1194-d018-4c79-a4db-ecac7d97cfe3.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 47 10" src="https://user-images.githubusercontent.com/93418349/233773896-724a528d-52c7-44e6-a714-1eabd74e1825.png">
<img width="1440" alt="스크린샷 2023-04-22 오후 5 47 48" src="https://user-images.githubusercontent.com/93418349/233773898-9ead8b40-d245-4cfc-a8e7-2bc7bdedc90e.png">




