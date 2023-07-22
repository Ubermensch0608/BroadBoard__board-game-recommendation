## 🔭 preview

<img src="https://file.notion.so/f/s/3881000d-f4ae-4c4d-98cb-97a640486093/%ED%99%94%EB%A9%B4_%EC%BA%A1%EC%B2%98_2022-02-20_102625.jpg?id=135eaa68-57d7-41a5-a0fd-b6504da707b0&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690077600000&signature=EBTy0THOFgySDngFBqCAUE9m8P6lJuWUGBb8Xl1_PB4&downloadName=%ED%99%94%EB%A9%B4+%EC%BA%A1%EC%B2%98+2022-02-20+102625.jpg" />

### 🤗 프로젝트 소개

<aside>
💡 보드게임을 추천 해주는 기능이 있는 웹페이지를 구현한 팀 프로젝트 입니다.

</aside>

### ✨사용기술 및 라이브러리

**Front**

- JavaScript
- jQuery

**Back**

- Python
- MongoDB
- AWS

### 🔬 세부 기능

- 로그인

  - 로그인 버튼을 클릭하면, 모달창이 생성되도록 하였습니다.
    모달창의 프레임은 게임세부정보 모달을 재사용하여 효율성을 높였습니다.
    <img src="https://file.notion.so/f/s/a60b6e00-d9a9-4aa5-8e06-feecbb719960/%EB%A1%9C%EA%B7%B8%EC%9D%B8.jpg?id=1a084a54-cf8e-4af3-846c-ebb13c83ba2d&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=XCYSR8Ev8XWrTWsfq2lkHkLuiTI0ab-ohyLScreOMSQ&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8.jpg" alt="로그인"/>
    <img src="https://file.notion.so/f/s/be0fa34b-e622-4d1c-960f-d555def720e2/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EB%AA%A8%EB%8B%AC.jpg?id=9115f93a-ef5c-414e-afc5-8fc604250d10&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=7RtNdL2tjypcql6nRALYxvXDDADH-vlI_LLXi2BUopc&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EB%AA%A8%EB%8B%AC.jpg" alt="로그인-모달"/>
  - 게임 코멘트, 추천 시 간단한 회원가입이 필요하도록 하였습니다.
    회원가입 후 축하를 알리는 모달창이 생성됩니다.
    <img src="https://file.notion.so/f/s/dd5d1e3c-47a5-42c0-b3e4-97c24490f201/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EA%B3%84%EC%A0%95%EC%83%9D%EC%84%B1.jpg?id=fd99d6c5-630e-499b-b927-39a185631ddf&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=UgCfwsOz0ioCFryAYzecyIu0h_ApWYKoidF4KgYNERk&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EA%B3%84%EC%A0%95%EC%83%9D%EC%84%B1.jpg" alt="로그인_계정생성"/>
    <img src="https://file.notion.so/f/s/ddb90214-fff4-4549-ba4b-7ffb910f57bb/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EA%B0%80%EC%9E%85%EC%B6%95%ED%95%98%EB%A9%94%EC%8B%9C%EC%A7%80.jpg?id=d72ee6ee-44ac-4a8e-adf2-747b2b470e56&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=Tom8YxanGndR6KwMNxYOiQ1dtra-aGVfyupCO1hQhl4&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EA%B0%80%EC%9E%85%EC%B6%95%ED%95%98%EB%A9%94%EC%8B%9C%EC%A7%80.jpg" alt="로그인_가입축하메시지"/>
  - 로그인 정보 보관
    회원가입 시 입력한 아이디와 비밀번호 등의 정보는 DB에 ‘POST’되어 다음 번 로그인 시 DB의 정보와 대조하여 해당 데이터가 존재할 경우 로그인을 승인합니다.
    <img src="https://file.notion.so/f/s/2902fb11-7bdf-44de-b480-e686b058a7a5/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EB%A1%9C%EA%B7%B8%EC%9D%B8%EC%8B%9C%EB%8F%84.jpg?id=c3a0ca93-d645-4322-9025-1599b7ab5c6e&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=j7mg20hPcTRgUZav1PlOZEt0abv5bZ6Mfxk2Dt7mA3c&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EB%A1%9C%EA%B7%B8%EC%9D%B8%EC%8B%9C%EB%8F%84.jpg" alt="로그인_로그인시도"/>

  - 로그인 이후 추가 기능
    - 이용자의 아이디를 동적으로 반영하는 웰컴을 구현했습니다.
      <img src="https://file.notion.so/f/s/aee8351b-ade5-497f-97a6-b7723ddeca5d/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%9B%B0%EC%BB%B4.jpg?id=1cef30d6-3f65-47a4-bb26-7bd58552aa6e&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=y_SxklMMdXl-GtGLGrk9iuViGHPLTfRJcTEt_GGVfeU&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%9B%B0%EC%BB%B4.jpg" alt="로그인_웰컴"/>
    - DB와 연동되는 댓글 기능을 구현했습니다.
      <img src="https://file.notion.so/f/s/fac2e665-6585-4dc1-9525-db0049cac738/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%BD%94%EB%A9%98%ED%8A%B8.jpg?id=a463535d-c752-45a4-8ee9-22922a1d7b6c&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=bEOruwMZyDWRsIx_HT6sjleGcWZ8xpHD92Xb2Bc82yc&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%BD%94%EB%A9%98%ED%8A%B8.jpg" alt="로그인_코멘트"/>
    - DB와 연동을 통해 실시간 업데이트가 되는 추천기능을 구현했습니다.
      <img src="https://file.notion.so/f/s/0e3420b9-eb72-44d9-82d6-cc3f28ed7a03/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%B6%94%EC%B2%9C%EC%8B%9C%ED%99%95%EC%9D%B8.jpg?id=b38c1274-a5d8-4ad2-8fa2-694291348442&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=JhIcyQvM6d2SZ3u_77YBJHK-rHtzqc68IZyKpKXroYw&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%B6%94%EC%B2%9C%EC%8B%9C%ED%99%95%EC%9D%B8.jpg" alt="로그인_추천시확인"/>
      <img src="https://file.notion.so/f/s/db351781-28a8-4f2e-ace2-c5ca5051d5dc/%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%BD%94%EB%A9%98%ED%8A%B8%EC%99%80%EC%B6%94%EC%B2%9C.jpg?id=818b28b8-9afa-426d-86a3-6277146653e1&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=kD3cReVCwdZZLE4elI8F8E7csoq7lmIUwDSTeoy5rIU&downloadName=%EB%A1%9C%EA%B7%B8%EC%9D%B8_%EC%BD%94%EB%A9%98%ED%8A%B8%EC%99%80%EC%B6%94%EC%B2%9C.jpg" alt="로그인_코멘트와추천"/>

- 검색창

  - 검색창을 상단에 위치시켜 이용자가 원하는 상품을 찾을 수 있도록하였습니다.
    <img src="https://file.notion.so/f/s/bb1bffa4-586b-4563-bdc1-f0b589726781/%EA%B2%80%EC%83%89.jpg?id=8296a286-afd7-4de9-bfed-52560cabe0ba&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=XkoqqXCl7rxnkdxjS6goi7O8_akKU8_45969ZfKFcJQ&downloadName=%EA%B2%80%EC%83%89.jpg" alt="검색"/>
  - 검색창에 자동완성기능을 구현하여 조금 더 손쉬운 검색이 가능하도록 하였습니다.
    <img src="https://file.notion.so/f/s/44441f2a-44c9-4d03-a158-5bfcb98e4494/%EA%B2%80%EC%83%89_%EC%9E%90%EB%8F%99%EC%99%84%EC%84%B1.jpg?id=fca93782-4fc5-4f2b-8a99-7db7d00fb4a6&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=mCyDQ4zX4lNUxcrs1K1jmY8mq0ZB1OFijygPLHyDtA0&downloadName=%EA%B2%80%EC%83%89_%EC%9E%90%EB%8F%99%EC%99%84%EC%84%B1.jpg" alt="검색_자동완성"/>
  - 검색 결과는 검색창의 value와 DB의 일치를 반영하여 생성하였습니다.
  - 사용자가 검색한 텍스트와 검색 건수는 동적으로 변경됩니다.
    <img src="https://file.notion.so/f/s/131864a5-c224-42bf-a4b9-5742796e76e1/%EA%B2%80%EC%83%89_%EA%B2%B0%EA%B3%BC.jpg?id=9df90556-d642-4c20-99db-75e23ed6dfb6&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=HCxwoxyen45KspBV_76WcyO78ZWevoCTDT5oFsjqAWI&downloadName=%EA%B2%80%EC%83%89_%EA%B2%B0%EA%B3%BC.jpg" alt="검색_결과"/>

- 필터링

  - 키워드로 게임 정보를 필터링하는 기능을 구현하여, 이용자가 게임을 자세히 모르더라도 쉽게 찾을 수 있도록 하였습니다.
    <img src="https://file.notion.so/f/s/1aa0cc17-a9e4-4a18-91cb-b64cef207848/%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89.jpg?id=ad9385bc-2b05-4536-b761-57664598e19f&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=7V1DN7EL3thWlnPKQtqstMLgsd1hGN206GYqptjoyRg&downloadName=%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89.jpg" alt="키워드검색"/>

  - 키워드 선택 후 ‘찾아주세요!’ 버튼을 누르면 선택한 키워드 정보와 결과가 동적으로 생성됩니다.
    <img src="https://file.notion.so/f/s/62512107-b0b6-4310-af5a-e433929b9b83/%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%ED%83%9C%EA%B7%B8%EC%84%A0%ED%83%9D.jpg?id=62696af5-c6de-4442-94c1-e9e2da90d341&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=mrrQ7NQWdvD1KTAPNI1_y1zT7MI3F2UlB3hHT2fmZC8&downloadName=%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%ED%83%9C%EA%B7%B8%EC%84%A0%ED%83%9D.jpg" alt="키워드검색_태그선택"/>
    <img src="https://file.notion.so/f/s/3fa4ee72-5f5b-46a2-a98e-b33b711ec948/%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%EC%84%A0%ED%83%9D%ED%83%9C%EA%B7%B8.jpg?id=8cd8a16d-a357-4233-98ca-6ce4d36b1657&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=-0y5eGNJ5bTi0VaNj7Xte6xlqhdvEjBzG9AkLoqDr5w&downloadName=%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%EC%84%A0%ED%83%9D%ED%83%9C%EA%B7%B8.jpg" alt="키워드검색_선택태그"/>
  - 검색 결과는 DB와 대조를 통해 동적으로 반영됩니다.
    <img src="https://file.notion.so/f/s/91634411-1c6e-4aee-a3b3-7b9774f024fe/%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%EA%B2%80%EC%83%89%EA%B2%B0%EA%B3%BC.jpg?id=3c79bf77-34a1-4fd7-8732-9406c34755e7&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=QQiv1GDJkXETBuRnVza8ZYoRWlt1zCcu-tfhUoXDMzI&downloadName=%ED%82%A4%EC%9B%8C%EB%93%9C%EA%B2%80%EC%83%89_%EA%B2%80%EC%83%89%EA%B2%B0%EA%B3%BC.jpg" alt="키워드검색_검색결과"/>

- 다크모드

  - 서비스 페이지의 흰색 여백이 많아 눈이 피로했던 경험을 바탕으로 다크모드 기능을 구현했습니다.
  - 다크모드 버튼을 누르면, 색이 반전되어 눈이 편한 페이지가 될 수 있도록 구현했습니다.
    <img src="https://file.notion.so/f/s/f2471ace-99c5-4d13-ac18-033e0608fbef/%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C.jpg?id=bc3ef3b6-4b8f-442d-8ada-9d9ae96b7f97&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=dg_ZdSo-UKMmyz89KzVX4gKitrRMT8wkBGTUwzuI2NI&downloadName=%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C.jpg" alt="다크모드"/>
    <img src="https://file.notion.so/f/s/91268a30-9f20-4e98-9946-c70b4838dc78/%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C_%EC%A0%81%EC%9A%A9.jpg?id=be876e00-eca7-4155-8053-e75c2545f0d8&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=1B8zfxg9UgOC3IL60sIfICh7GeAWBKVOccytHx7QU_w&downloadName=%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C_%EC%A0%81%EC%9A%A9.jpg" alt="다크모드_적용"/>

- 리모콘

  - 우측 중앙 네비게이션 바에 리모콘 기능을 구현했습니다.
    <img src="https://file.notion.so/f/s/9b501534-6896-4ec1-a662-7c67a6067dc3/%EB%A6%AC%EB%AA%A8%EC%BD%98.jpg?id=bf7fa2e9-5157-48f4-bbfe-17f147ab1ad6&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=FOeNAdJU8hT2CoNqbU-V6mW32ee7gmEqvZU0hHnNwj8&downloadName=%EB%A6%AC%EB%AA%A8%EC%BD%98.jpg" alt="리모콘"/>

- 마우스 hover 시 어떤 영역으로 갈지 힌트를 주고, 클릭 시 해당 영역으로 이동합니다.
  <img src="https://file.notion.so/f/s/ef3539b8-68a6-4844-a830-826f270121dc/%EB%A6%AC%EB%AA%A8%EC%BD%98_hover.jpg?id=164aec92-8997-4d75-9ec1-5d154037342b&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=BrY2GmB_NG7LstsZfIzo4jTrTR_QC9EzFwBe8Y75Qu4&downloadName=%EB%A6%AC%EB%AA%A8%EC%BD%98_hover.jpg" alt="리모콘_hover"/>
  <img src="https://file.notion.so/f/s/9a979795-1e21-4235-ae2e-b734bf3f2a41/%EB%A6%AC%EB%AA%A8%EC%BD%98_%ED%82%A4%EC%9B%8C%EB%93%9C.jpg?id=14ea6eca-4c34-4cb0-a2eb-dd9d639f36d3&table=block&spaceId=ae42ddab-f52a-4185-b6d8-5b159f46dd43&expirationTimestamp=1690084800000&signature=G4wdMMsJDUI6dsCNpuv_IJh8VsQY3ZCALuSM2abxiHQ&downloadName=%EB%A6%AC%EB%AA%A8%EC%BD%98_%ED%82%A4%EC%9B%8C%EB%93%9C.jpg" alt="리모콘_키워드"/>

### 🍿 소개 영상

<a href="https://media-sparta.s3.amazonaws.com/media/tempvideos/20220103/djulx350psg0qvbn.mp4" >프로젝트 소개 영상</a>
<video src="https://media-sparta.s3.amazonaws.com/media/tempvideos/20220103/djulx350psg0qvbn.mp4">

### ‼ 느낀점

- 팀 구성원 모두 처음인 팀프로젝트였기 때문에 새로운 기능을 구현할 때마다 어려운 점이 많았습니다.
- 하지만, 서칭을 통해 공부를 하고 해결해나가면서 끈끈한 팀이 되었던 것이 인상깊었습니다.
- 웹 개발을 프론트와 백이 한 팀이 되어 하는 경험을 통해 프론트와 백이 상호작용하는 웹개발의 대략적인 순환체계를 알 수 있었습니다.
