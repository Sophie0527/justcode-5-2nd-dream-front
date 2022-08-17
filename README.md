# Dream 프로젝트  
한정판을 거래하는 [Kream](https://kream.co.kr/)  클론하는 프로젝트  
<br>
<img width="1000" alt="스크린샷 2022-08-17 오후 2 33 19" src="https://user-images.githubusercontent.com/100933263/185042288-3a000987-f38a-4620-8d3a-4c609791b862.png">


##  프로젝트 사이트 기능 구현 영상

[Dream](https://www.youtube.com/watch?v=4hLrODXxXI4)

## Members

손소희 [기술블로그](https://sophie0527.tistory.com/), [깃허브](https://github.com/Sophie0527)  
정진우 [기술블로그](https://velog.io/@happyeveryone96), [깃허브](https://github.com/happyeveryone96)  
유관희 [기술블로그](https://velog.io/@yrats), [깃허브](https//github.com/kwan-hee)  
최수진 [기술블로그](https://velog.io/@hissujinc), [깃허브](https://github.com/ssujinc)  
김예찬 [기술블로그](https://velog.io/@kyc5244), [깃허브](https://github.com/developer-yechan)  
최정훈 [기술블로그](https://velog.io/@jeongssi94), [깃허브](https://github.com/Choi-jeonghoon)

## Introduction

- 개발 인원 및 기간
  - 개발 기간 | 2022-07-11 ~ 2022-07-29
  - 개발 인원 | 총 6명 FE : 손소희,정진우,유관희 BE : 최수진,김예찬,최정훈
- 프로젝트 선정 이유
  - 2차 클론 코딩 프로젝트로 KREAM 사이트를 선정하게 되었습니다. 상품을 사고팔고, 그리고 sns 기능까지 갖춘 다양한 분분을 보여줄 수 있는 사이트라 생각되어 선택하게 되었습니다.

## 레포지토리 주소

- [Front-end-repo](https://github.com/Sophie0527/justcode-5-2nd-dream-front)
- [Back-end-repo](https://github.com/wecode-bootcamp-korea/justcode-5-2nd-dream-back)

## Notion 프로젝트 소개

- [Dream 노션 페이지](https://www.notion.so/wecode/2-Dream-abb0472d93714fd8b20433095c0f0ed6)

## DB modeling

- [Dream db 자료 구조](https://dbdiagram.io/d/62cbc455cc1bc14cc59073da)

## Technlogies

#### DB
<div> 
<img src="https://img.shields.io/badge/mySQL-4479A1?style=for-the-badge&logo=mySQL&logoColor=white"> 
<img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=Prisma&logoColor=white">
<img src="https://img.shields.io/badge/DB-diagram-F08705?style=for-the-badge&logo=diagrams.net&logoColor=black">
<br>

#### Front-end
<div> 
<img src="https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=HTML5&logoColor=white"> 
<img src="https://img.shields.io/badge/scss-1572B6?style=for-the-badge&logo=scss&logoColor=white">
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
<img src="https://img.shields.io/badge/styled-components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white">
<br>

#### Back-end
<div> 
<img src="https://img.shields.io/badge/NODE.JS-339933?style=for-the-badge&logo=NODE.JS&logoColor=black">
<img src="https://img.shields.io/badge/EXPRESS-000000?style=for-the-badge&logo=EXPRESS&logoColor=white">
<img src="https://img.shields.io/badge/bcrypt-FF6C37?style=for-the-badge&logo=bcrypt&logoColor=black">
<img src="https://img.shields.io/badge/jsonwebtoken-black?style=for-the-badge&logo=jsonwebtokens&logoColor=white">
<br>

#### 협업 도구
<div> 
<img src="https://img.shields.io/badge/Github-000000?style=for-the-badge&logo=Github&logoColor=white">
<img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white">
<img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white">
<br>

## 구현 기능

### Front-end

|**손소희**|**정진우**|**유관희**|
|---|---|---|
|`마이페이지(프로필)`<br>`마이페이지(관심상품내역)`<br>`마이페이지(구매/판매내역)`<br>`SHOP페이지`|`로그인/회원가입`<br>`제품 상세페이지`<br>`구매/판매 페이지`|`메인페이지`<br>`Header/Footer`<br>`STYLE페이지`|

<br/>

### **`마이 페이지(프로필 페이지,관심/구매/판매 페이지)`**

<img src="https://user-images.githubusercontent.com/100933263/185050171-2af2decb-c54d-4cb3-8917-5e11551ecbd3.gif" width="800"/>

- **프로필 페이지**  
  - 백엔드와 통신을 통해 프로필 상세 정보를 가져오기 (GET)
  - 백엔드와 통신을 통해 프로필 주소 등록 (POST) : 프로필 이미지 없을 시 기본 프로필 이미지로 보여줄 수 있도록 함.
  - 백엔드와 통신을 통해 회원 탈퇴 (DELETE) : 회원 탈퇴 성공 시 메인 화면으로 이동.
  - 백엔드와 통신을 통해 프로필 주소 삭제 (DELETE)
  - 백엔드와 통신을 통해 프로필 주소 수정 (PUT) : input 창에  입력되는 값을 useState를 사용해 입력된 값을 유지시키기.
  - 백엔드와 통신을 통해 프로필 이름/휴대폰 번호 수정 (PUT)
  - 프로필 주소 추가 기능
    <br/>
  
<div> 
<img src="https://user-images.githubusercontent.com/100933263/185049585-d003737b-7855-4b9f-8697-0375c77f4b83.gif" width="800"/>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fu5XZx%2FbtrIfSNhQ8n%2FeIzmIMMe1yIfrjUohVEzEK%2Fimg.png" width="500"/>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2F1TWOL%2FbtrIhjKEDyB%2FoKoPCioo6BelVOQTMu0oCK%2Fimg.png" width="500"/>
</div>
<br/>

- **관심/구매/판매 페이지**   
  - 백엔드와 통신을 통해 판매상품/구매상품/관심 상세 정보를 가져오기 (GET)
  - 백엔드와 통신을 통해 관심 상세정보 삭제 (DELETE)
  <br/>
  
  ### **`SHOP 페이지 `**

<img src="https://user-images.githubusercontent.com/100933263/185049071-66e0383e-f1da-4767-90c3-006e7c21fd8f.gif" width="800"/>

- **SHOP 페이지**  
  - 백엔드와 통신을 통해 상품 가져오기 (GET)
  - 인기순/발매 일순으로 map 메소드를 활용해 상품 보여주기
  - 슬라이더 베너 구현
  - 관심상품 등록 기능 구현
  
<br/>

---

### Back-end

|**최수진**|**김예찬**|**최정훈**|
|---|---|---|
|`회원가입, 로그인 API/소셜 로그인(카카오)`<br>`SHOP 페이지 API`<br>`제품상세 페이지 API`|`메인 페이지 API`<br>`STYLE 페이지 API`<br>`관심상품 API`|`마이 페이지 API`<br>`구매 / 판매 페이지 API`|

[‣ Back-end 더보기](https://github.com/wecode-bootcamp-korea/justcode-5-2nd-dream-back)

<br/>

## Contact

- ssh30510044@gmail.com, [기술블로그](https://sophie0527.tistory.com/), [깃허브](https://github.com/Sophie0527)
