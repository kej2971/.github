## SleepIsDead

### Repositories  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSleepIsDead%2F.github&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

---
# GNT (그래서 님 티어가)
> **MTVS-SERVER-SleepIsDead** <br/> **개발기간: 2023.08.01 ~ 2022.08.29**

---
## Team Member Introduction
|권은지|김태현| 김지수                                                                               |
|-------------------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------|
|<img width="160px" src="https://avatars.githubusercontent.com/u/139085498?v=4" />|<img width="160px" src="https://avatars.githubusercontent.com/u/136583226?v=4" />| <img width="160px" src="https://avatars.githubusercontent.com/u/122511847?v=4" /> |
|<center>[@kej2971](https://github.com/kej2971)| <center>[@taedyyyyy](https://github.com/taedyyyyy)| <center>[@jisoo9603](https://github.com/jisoo9603)                            |

| 이유열                                                                              |정재민|
|----------------------------------------------------------------------------------|-------------------------------------------------|
| <img width="160px" src="https://avatars.githubusercontent.com/u/84696773?v=4" /> |<img width="160px" src="https://avatars.githubusercontent.com/u/125876896?v=4" />|
| <center>[@youyeul301](https://github.com/youyeul301)                             |<center>[@devJaem](https://github.com/devJaem)|

---
# Project Introduction

## GNT는 사용자들에게 다음의 기능을 제공합니다.
<br>
2023년 현재 새로운 유행, 클라이밍의 새로운 문화를 만들기 위해 제작하는 플랫폼 입니다.
운동을 할때 사람들이 많이 겪는 고민을 어려가지 문제점 중 몇개를 선정하였습니다.
- 대결상대(기록경쟁, 문제풀이)의 부재
- 고정적인 상대와 플레이를 하며 같은수준 유지
- 같이 할사람을 찾고싶어도 말 걸거나, 사람을 찾는 노력을 하기 어려운 사람들
이러한 문제를 해결하기위해, 본 서비스의 구현 및 배포를 통해 문제점을 해결하려고 합니다. \

--- 

## 현재 경쟁이 이루어질 만한 서비스, 참고할만한 서비스
- 카카오톡 오픈채팅
- 네이버 밴드나 카페
- 플랩풋볼
카카오 오픈채팅이나 밴드, 카페는 스포츠 전문이 아니기 때문에, 특화 기능을 제공하지 않습니다.
플랩풋볼의경우 추구하는 방향과 비슷하나, 축구,풋살에만 집중된 서비스를 제공합니다.

--- 

## 세부 제공 서비스
1. 조건에 맞는 클라이밍 매칭 서비스
2. 알림 서비스 및 운동 내역 관리 서비스
3. 볼더링, 스피드, 리드 각 종목에 따른 각각 다른 각각의 종목에 따른 서비스 

---

## 클라이밍 종목 , 종목별 랭킹
#### 볼더링 (문제풀이)
- 대부분의 실내 클라이밍장에서 이용할수 있는 종목
- 제한시간내에 최소한의 시도로 문제 풀이
- 문제당 4분이내의 시간제한
- 가장 접근이 쉽고, 보통 입문자들 입문, 강습에 사용되기 때문에, 랭킹보다는 매칭 자체에 의미가있음
- 크루를 생성하거나, 친목을 다지고, 서로의 실력을 확인
<br>
#### 리드 (시간내 높이오르기)
- 실외 클라이밍장에서 이용할수 있는 종목.(2인1조)
- 12M이상의 암벽에서 높이 올라가느냐 
- 벽높이는 15M 시간제한 6분
- 특정(야외) 클라이밍장에서만 가능
- 시간당 등반 높이로 확실하게 승패가 결정남
- 시간당 오른 높이 혹은 기준점을 기준으로 랭킹을 지원할수 있음.
<br>
#### 스피드 (단거리 레이스)
- 15미터 암벽에 동일한 루트를 2명의 참가자가 동시출발 레이스
- 경기루트는 항상 동일함.
- 특정(야외) 클라이밍장에서만 가능
- 등반 시간을 경쟁하는 종목으로, 명확한 시간초가 제공됨
---

## 초기 구현 모델 
1. 처음에는 유저 - 유저 운동 시간별, 같이 활동할수 있는 매칭 위주로 구현될 예정입니다. 리드나, 스피드 종목은 초심자가 접근하기 어렵기때문에 볼더링 매칭부터 구현합니다.
2. 팀(크루) 참가, 모집 기능을 구현합니다.
3. 신고기능을 활성화하여 신고가 누적된 (비매너, 범죄행위) 회원은  블랙리스트 제도를 활성화 합니다.
4. 참가신청을 했는데 특별한 사유없이 출석하지 않을경우 패널티를 부과합니다 (활동정지 1주, 1개월, 영구) 향후 결제모델 도입시,  신고기능과 별개로 금전차감으로도 변경이 가능합니다.
5. 초창기 서비스 진행시 사전에 조사된 클라이밍장을 기준으로 정보를 등록하고 회원은, 장소정보를 이용하여 일정을 생성할수 있습니다.
6. 일정 생성시 참가신청을 할수있고 참가신청이 완료되면, 채팅에 자유롭게 참여할수 있습니다. 참여 2일전까지 패널티 없이 취소할수 있습니다.
7. 클라이밍장 추가를 요청하거나, 종목추가능 건의사항 피드백을 받을수 있는 1:1 문의를 구현합니다.

---

## 이후 추가 비즈니스 모델
1. 과금체계는 시설이용료 + 수수료로 구성되며, 수수료에는, 매니저 활동비가 포함됩니다.
2. 매니저 제도는, 클라이밍장에서 직접 수행하거나, 건당 활동비를 제공합니다.
3. 매니저가 활동할수 있는 백오피스기능도 구현되어야 합니다.
4. 처음 트래픽 확보이전에는 볼더링 종목만으로는 티어, 레이팅 구현이 종목 특성상 힘들기때문에 트래픽 확보이후 구현을 목표로 합니다.
5. 시설별 랭킹 > 활동레벨제도 도입 (횟수,참여도,매너 를 수치화) > 승패나 기록을 기준으로, 레이팅 제도 도입 /레이팅별로 각각 승리/패배시 얻는 점수는 다름

---

## Getting Started Guide
### 요구사항
For building and running the application you need:

- [MySQL8.0.33](https://dev.mysql.com/downloads/mysql/)
- [JAVA11.0.15](https://github.com/ojdkbuild/ojdkbuild)
- [Node.js](https://nodejs.org/ko)

---

## Stacks 🐈

### Environment
<img src="https://img.shields.io/badge/Intelii J-000000?style=for-the-badge&logo=intellijidea&logoColor=white">
<img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/visualstudiocode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white">
<img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">

### Config
![FIGMA](https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![MIRO](https://img.shields.io/badge/miro-050038?style=for-the-badge&logo=miro&logoColor=white)

### Development
![JAVASCRIPT](https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=for-the-badge&logo=JAVASCRIPT&logoColor=white)
![REACT](https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![springboot](https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![MYSQL](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=Bootstrap&logoColor=white)

### 소통수단
<img src="https://img.shields.io/badge/discord-5865F2?style=for-the-badge&logo=discord&logoColor=white">
<img src="https://img.shields.io/badge/kakaotalk-FFCD00?style=for-the-badge&logo=kakaotalk&logoColor=white">

---
## Screen Layout 📺

### [LayOut](https://github.com/GoOnThat/GoOnThat/wiki/Screen-Layout)
|                                                                                                                                             메인 페이지 |                                                                                                                         로그인 페이지 |
|---------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| <img width="329" src="https://github-production-user-asset-6210df.s3.amazonaws.com/125876896/257041304-ea431078-05b9-482d-8901-fe05c5128f90.png"/> | <img width="329" src="https://user-images.githubusercontent.com/125876896/257041747-ef8adc64-89df-4772-a751-f1a5ff9f00c8.png"/> |  
|                                                                                                                                           회원가입 페이지 |                                                                                                                         게시판 페이지 |  
|                    <img width="329" src="https://user-images.githubusercontent.com/125876896/257041757-e8a6e2c0-e137-4a7a-80e6-b1c4ac5a6435.png"/> |             <img width="329" src="https://github.com/GoOnThat/GoOnThat/assets/125876896/abbde490-87fc-4463-9f8b-e3bcd7199365"/> 

---
# Main Function 📦

---
### ⭐️ 매칭게시판
- 미리 조사된 클라이밍장을 기준으로, 운영시간내 시간을 선택하여 운동일정 생성
- 신청자의 정보는, 닉네임, 성별, 나이대만 전달될수 있도록함
- 승인되면 채팅에 자유롭게 참여할수있음.
- 일정 3일이전에는 패널티없이 매칭 취소가 가능
- 매칭게시판 작성자는 신청자를 알림으로 식별이 가능 마이페이지 or 네비게이션 바에서 에서 숏컷으로 접근가능
- 신청자도 승인후 알림으로 식별이 가능 마이페이지 or 네비게이션 바에서 에서 숏컷으로 접근가능

---

### ⭐️ 팀/크루 모집 게시판
- 팀/크루를 간단한 소개글과 사진, 영상임베드 등으로 소개할수있는 팀별 페이지 구현
- 매칭과 비슷하게 구현되며, 팀 크루 참가신청, 승인의 방식으로 활용
- 신청자의 정보는, 닉네임, 성별, 나이대만 전달될수 있도록함
- 승인되면 채팅에 자유롭게 참여할수있음. 참가 이전 채팅도 볼수있게 구현
- 팀/크루장은 참가신청시 알림으로 식별가능 마이페이지 or 네비게이션 바에서 에서 숏컷으로 접근가능
- 크루원 승인시 알람으로 식별이 가능하며 마이페이지 or 네비게이션 바에서 에서 숏컷으로 접근가능

---

### ⭐️ 마이페이지
- 참여했던 운동 목록을 날짜별로 조회할수 있음
- 같이 활동했던 회원의 평가를 작성할수 있음. (작성하지 않아도 상관없으나 작성하면 포인트를 제공하여 추후 포인트상품이나, 마일리지 처럼 활용가능)
- 작성된 평가는 익명으로 남게되며, 성의없는 내용은 신고가 가능함
- 본인의 레벨 (참여횟수, 신고횟수를 이용하여 수치화) 확인가능
- 추후 티어나 레이팅 점수도 확인가능
- 개인별 블랙리스트 (차단) 구현
- 회원정보 수정가능
- 팀/크루정보와 진행중 매칭에 접근이 가능함

---

### ⭐️ 관리자페이지
- 각종 신고를 처리할수 있는 보드 구성
- 신고 1회 이상 누적되면 알림, 10회이상시 자동 블러처리가 가능하도록 함
- 블랙리스트 제도 관리
- 관리자 페이지에서는 모든 게시글에 접근이 가능, 회원정보 조회는 공개된 정보만 가능하고 개인식별정보는 불가능

---

## Architecture
[DDD](https://www.youtube.com/watch?v=dJ5C4qRqAgA)
[MSA](https://giljae.medium.com/%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%84%9C%EB%B9%84%EC%8A%A4-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-microservices-architecture-%EC%9D%98-%EC%9E%A5%EC%A0%90%EA%B3%BC-%EB%8B%A8%EC%A0%90-7c45615cfe1a)

---
## directory tree
```bash

           
```
