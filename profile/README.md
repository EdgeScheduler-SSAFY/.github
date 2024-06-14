# Edge Scheduler

> SSAFY 10기 자율 프로젝트 서울 1반 Edge Scheduler (2024.04.08 ~ 2024.05.20)

<img src="/assets/edgeScheduler.jpg" width="80%">

<br/>

# 📜 목차

##### 1️⃣ [서비스 소개](#-서비스-소개)

##### 2️⃣ [서비스 화면](#-서비스-화면)

##### 3️⃣ [개발 환경](#-개발-환경)

##### 4️⃣ [기술 특이점](#-기술-특이점)

##### 5️⃣ [기획 및 설계 산출물](#-기획-및-설계-산출물)

##### 6️⃣ [Conventions](#-conventions)

##### 7️⃣ [팀원 소개 및 개발 회고](#-팀원-소개-및-개발-회고)

<br/>

# 서비스 구경 🎈

### [배포 사이트](https://edgescheduler.co.kr)

### 📌 Overview

- 글로벌 기업을 위한 **글로벌 회의 일정 추천 서비스**

### 🎯 기획 배경

> 세계 각지에 흩어져 있는 팀원들과 함께 일할 때 **시차**로 인한 **불편사항** 발생

> 회의 일정 고려 시, **각 팀원들의 시차를 고려**한 시간대를 파악해야 하는 **번거로움**존재

> 일부 팀원들은 **이른 시간**에 일어나거나, **늦은 시간**까지 일을 해야하는 불편함 존재

> **팀원들의 피로도 상승**, **생산성과 업무 만족도 하락**

### 📌 서비스 기능

- 각 사용자는 **개인 일정**을 등록하여 관리할 수 있습니다.
- **month, week, day**별 일정을 조회할 수 있습니다.
- **반복 일정** 및 **비공개 일정**을 관리할 수 있습니다.
- 회의 생성 시, 참여자들의 **필참 여부**를 선택하여 **최적의 회의시간**을 추천받을 수 있습니다.
- 설정한 기간 내에서 **3가지 기준(가장 빠른 시간, 불참자가 가장 적은 시간, 근무시간 내 참여자가 가증 많은 시간)**으로 **최적의 회의시간**을 추천받을 수 있습니다.
- 회의 참여를 요청받은 참여자들은 **수락, 거절, 새로운 시간 제안**을 통해 자신의 참석여부를 결정할 수 있습니다.
- 새로운 시간을 제안하기 전에, **해당 시간 내에 가능한 인원 조회**기능을 이용할 수 있습니다.
- **드래그 기능**으로 쉽고 간편하게 회의 시간을 설정할 수 있습니다.
- **타임존 설정**을 통해 세계 어디에서나 편하게 시간 변환을 통해 서비스를 이용할 수 있습니다.
- **실시간 브라우저 알림**을 통해서 회의 생성, 수정 및 새로운 시간 제안에 대한 알림을 받아볼 수 있습니다.
- **이메일 알림**을 통해 사이트에 접속해 있지 않더라도 회의와 관련한 알림을 받아볼 수 있습니다.

- <br >

# 서비스 화면 🎬

| ![Sign in](/assets/screen/signin.gif) | ![Personal Schedule](/assets/screen/personal_schedule.gif) |
| :-----------------------------------: | :--------------------------------------------------------: |
|                로그인                 |                       개인 일정 등록                       |

| ![Set Personal Info](/assets/screen/set_personal_info.gif) | ![Create Meeting](/assets/screen/create_meeting.gif) |
| :--------------------------------------------------------: | :--------------------------------------------------: |
|                       근무 시간 설정                       |                      회의 생성                       |

| ![Meeting Accept](/assets/screen/meeting_accept.gif) | ![Meeting Update](/assets/screen/meeting_update.gif) |
| :--------------------------------------------------: | :--------------------------------------------------: |
|                      회의 수락                       |                      회의 수정                       |

| ![Meeting Proposal](/assets/screen/meeting_proposal.gif) | ![Meeting Cancel](/assets/screen/meeting_cancel.gif) |
| :------------------------------------------------------: | :--------------------------------------------------: |
|               회의 거절(새로운 시간 제안)                |                      회의 삭제                       |

---

<br />

# 개발 환경 🖥

## 🖱 Frontend

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC.svg?&style=for-the-badge&logo=Visual%20Studio%20Code&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)<br>
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![React Query](https://img.shields.io/badge/-React%20Query-FF4154?style=for-the-badge&logo=react%20query&logoColor=white)
![styled-components](https://img.shields.io/badge/-styled%20components-DB7093?style=for-the-badge&logo=styled%20components&logoColor=white)
<br>

## 🖱 Backend

![Intellij IDEA](https://img.shields.io/badge/Intellij%20IDEA-000000.svg?&style=for-the-badge&logo=IntelliJ%20IDEA&logoColor=white)
![SpringBoot](https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)<br>
![SpringSecurity](https://img.shields.io/badge/Spring%20Security-6DB33F.svg?style=for-the-badge&logo=Spring%20Security&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Mysql](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)<br>
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white")
![Kafka](https://img.shields.io/badge/Apache%20Kafka-%3333333.svg?style=for-the-badge&logo=Apache%20Kafka&logoColor=white)
![ThymeLeaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=Thymeleaf&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=JUnit5&logoColor=white)

## 🖱 Infrastructure

![Jenkins](https://img.shields.io/badge/jenkins-%232C5263.svg?style=for-the-badge&logo=jenkins&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![EC2](https://img.shields.io/badge/EC2-232F3E?style=for-the-badge&logo=Amazon-ec2&logoColor=white)

## 🎨 UI/UX

![Figma](https://img.shields.io/badge/Figma-F24E1E.svg?style=for-the-badge&logo=Figma&logoColor=white)
<br>

## 👨‍👩‍👧 협업 툴

- <strong>형상 관리<br>
  ![Git](https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white)
  ![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)

- <strong>이슈 관리<br>
  ![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white)

- <strong>커뮤니케이션<br>
  ![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white)
  ![Mattermost](https://img.shields.io/badge/Mattermost-0072C6?style=for-the-badge&logo=mattermost&logoColor=white)
  ![KakaoTalk](https://img.shields.io/badge/kakaotalk-ffcd00.svg?style=for-the-badge&logo=kakaotalk&logoColor=000000)
  <br>

<br />

# 기술 특이점 🧰

## 🖱 Frontend

- 1. 외부 라이브러리 사용 없이 **드래그 기능 및 캘린더 기능 구현**

- 2. NextJS 활용 SEO를 고려한 SSR방식 웹사이트 제작

- 3. NextJS 활용 데이터 캐싱으로 UX 향상

- 4. Zustand를 활용해 전역 상태 관리

- 5. refreshToken과 accessToken으로 로그인 로직 구현

## 🖱 Backend

### ✨ 1. MSA

<div align="start">
<img src="/assets/MSA.png" alt="MSA" width="90%" height="70%">
</div>

### ✨ 2. Event-Driven Architecture 구축

<div align="start">
<img src="/assets/kafka.png" alt="kafka" width="50%" height="70%">
</div>

### ✨ 3. 마이크로 서비스 서버별 DB 분리

<div align="start">
<img src="/assets/DB분리.png" alt="DB분리" width="50%" height="70%">
</div>

### ✨ 4. 비동기 알림 처리

<div align="start">
<img src="/assets/webflux.png" alt="Spring WebFlux" width="50%" height="70%">
</div>
<br />

# 기획 및 설계 산출물 📁

### [Notion](https://cheddar-cloudberry-278.notion.site/Edge-Scheduler-d7a4abb7476b478dbfa09f8bdf23fcb0)

### 🏛 서비스 아키택처

<div align="start">
<img src="/assets/서비스아키텍처.png" alt="architecture" width="70%" height="70%">
</div>

### 🛢︎ ERD

<div align="start">
<img src="/assets/ERD.png" alt="ERD" width="70%" height="70%">
</div>

### [📄 API 명세서](https://cheddar-cloudberry-278.notion.site/API-d58760b094f04775b51fe521ff9c8015?pvs=74)

<div align="start">
<img src="/assets/api명세서.png" alt="api명세서" width="70%" height="70%">
</div>

### [🎨 화면 설계서](https://www.figma.com/design/WZr1HQ1PfhMd3nINjNrb3b/%F0%9F%93%B0?node-id=0%3A1&t=Y5XH75ckJ86cDiE9-1)

<div align="start">
<img src="/assets/figma.png" alt="화면설계서" width="70%" height="70%">
</div>

<br/>

# ✨ Conventions

## 📌코드 컨벤션

[🖱 Frontend Conventions](https://cheddar-cloudberry-278.notion.site/Front-End-a2593902d26b4a62b90f04ffff85bdf2)

[🖱 Backend Conventions](https://cheddar-cloudberry-278.notion.site/Back_End-0cc21c58164e4ee09214200a6b467416?pvs=74)

## 📌커밋 컨벤션

```
✨Feat : 새로운 기능 추가
🐛Fix : 버그 수정
📝Docs : 문서 수정
🗃️Style : 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우
♻️Refactor : 코드 리펙토링
✅Test : 테스트 코드, 리펙토링 테스트 코드 추가
💡Comment : 필요한 주석 추가 했을 경우
🎨Design : css나 디자인 변경, 이미지 추가 등
🚑Hotfix : 치명적인 버그 수정
👷Build : 배포 관련
🤝🏻Merge : f-기능명 into dev-frontend
```

<br />

# 팀원 소개 및 개발 회고 🐥

## 📆 프로젝트 기간

### 2024.04.08 ~ 2024.05.20

- 기획 및 설계(학습) : 24.04.08 ~ 24.04.18
- 프로젝트 구현 : 24.04.19 ~ 24.05.16
- 버그 수정 및 산출물 정리 : 24.05.17 ~ 24.05.19
- 코드 리팩토링 : 24.05.20 ~

<br />

## 🍑 팀원 소개

<table>
    <tr>
        <td height="140px" align="center"> <a href="https://github.com/hyunsoo10">
            <img src="https://avatars.githubusercontent.com/hyunsoo10" width="140px" /> <br><br> 👑 조현수 <br>(Back-End) </a> <br></td>
        <td height="140px" align="center"> <a href="https://github.com/pyeong114">
            <img src="https://avatars.githubusercontent.com/pyeong114" width="140px" /> <br><br> 👶🏻 전은평 <br>(Back-End) </a> <br></td>
        <td height="140px" align="center"> <a href="https://github.com/HyeongtaekOh">
            <img src="https://avatars.githubusercontent.com/HyeongtaekOh" width="140px" /> <br><br> 👶🏻 오형택 <br>(Back-End) </a> <br></td>
        <td height="140px" align="center"> <a href="https://github.com/yhc-key">
            <img src="https://avatars.githubusercontent.com/yhc-key" width="140px" />
            <br><br> 👶🏻 조용환 <br>(Front-End) </a> <br></td>
        <td height="140px" align="center"> <a href="https://github.com/kimjungkwang1">
            <img src="https://avatars.githubusercontent.com/kimjungkwang1" width="140px" /> <br><br> 👶🏻 김중광 <br>(Front-End) </a> <br></td>
        <td height="140px" align="center"> <a href="https://github.com/se2develop">
            <img src="https://avatars.githubusercontent.com/se2develop" width="140px" /> <br><br> 👶🏻 노세희 <br>(Front-End) </a> <br></td>
    </tr>
    <tr>
        <td align="center"><br/></td>
        <td align="center"><br/></td>
        <td align="center"><br/></td>
        <td align="center"><br/></td>
        <td align="center"><br/></td>
        <td align="center"><br/></td>
    </tr>
</table>

## 🙌🏻 회고

##### **조현수**<br>

- 이번 프로젝트에서 처음으로 MSA 설계와 스프링 클라우드 기술을 활용해보았습니다. 또한 물리서버 EC2를 여러 대 사용해서 gateway 서비스, discovery 서비스, micro 서비스들끼리 서로 통신하도록 했습니다. 해당 작업이 쉽지 않았지만 네트워크에 대한 인사이트를 얻을 수 있었습니다. 그리고 Gerrit을 활용해서 코드리뷰를 체계적으로 진행함으로써 클린코드에 대한 고민과 다른 사람의 코드를 이해하기 위해 꼼꼼하게 읽고 피드백을 주기 위해 노력했었습니다. 기업 요구사항 명세서 분석, MSA, 코드 리뷰 등 새로운 경험과 개발을 해볼 수 있었던 프로젝트였다고 생각합니다.

##### **전은평**<br>

- 프로젝트 초기 설계 단계에서 팀원들과의 적극적인 소통을 통해 잠재적으로 문제가 될 수 있는 요소를 사전에 파악하려고 노력했습니다. 이 과정에서 탄탄한 설계를 구축할 수 있었으며, 차후 발생할 수 있는 많은 문제를 예방할 수 있었습니다. 코드를 작성할 때에도 중복을 최소화하고 코드의 재활용성을 높이기 위해 여러 곳에서 사용할 수 있는 메서드를 한 곳에 모아 관리했습니다. 이를 통해 코드의 일관성과 유지보수성을 높일 수 있었습니다. 비록 테스트 코드를 작성했지만, 예상치 못한 사항들이 발생하여 추가 작업이 필요했던 경우가 있었습니다. 이는 기초 설계의 중요성을 다시 한 번 실감하게 하는 계기가 되었습니다. 앞으로 새로운 프로젝트를 진행할 때는 설계 단계에서 더 다양한 경우를 고려하고 이를 꼼꼼하게 기록하겠습니다. 이를 통해 추가 작업을 최소화하고 프로젝트의 완성도를 높이겠습니다. 이번 회고를 통해 얻은 교훈을 바탕으로 다음 프로젝트에서는 더욱 철저한 계획과 준비로 성공적인 결과를 도출할 수 있도록 하겠습니다.

##### **오형택**<br>

-

##### **조용환**<br>

- 각자 로컬 시간에 맞춰 시간을 표시하고, 가지고 있는 일정을 hover를 통해 동적으로 설정하는 것이 어려웠습니다. 또한 drag & drop 기능 및 dropdown 등을 시간 설정에 사용할 수 있도록 연동시키는 것이 힘들었습니다. 다행히 만족스럽게 마무리 할 수 있어 좋았습니다.

##### **김중광**<br>

- 이번 프로젝트에서 저는 프론트엔드 개발자로 스케줄 페이지의 구현과 일정 조회, 등록, 수정, 삭제, 로그인 처리를 담당하였습니다. 프로젝트에서 React, Next.js, TypeScript를 사용하였으며 특히 Next.js를 처음 사용해봐 좋은 경험이었습니다. 또한 코드리뷰 도구로 Gerrit을 사용하여 처음으로 코드리뷰를 경험 해봤습니다. 코드리뷰를 통해 다른 사람의 코드를 더 살펴보고 내코드에 대한 리뷰를 받는 과정에서 한걸음 더 성장 한것 같습니다.

##### **노세희**<br>

- 프로젝트 진행 과정에서 회의 생성 페이지, SSE 알림 연결을 담당하였습니다. 글로벌 회의 일정 잡기라는 주제처럼 각 사용자들의 시간 설정이 다르기 때문에 백엔드와 연결하는 부분에서 발생하는 오류를 찾고 해결하는 과정에서 초기 설계 단계에서 문서 작업의 중요성을 배울 수 있었습니다. 회의 생성 페이지에서 이름을 검색할 때, 자바스크립트의 정규표현식과 유니코드를 사용하여 초성 검색이 가능하도록 구현하는 과정이 어려웠지만 많이 성장할 수 있었습니다. 코드 리뷰를 과정을 통해 코드 작성 시 중복을 최소화하고, 컴포넌트 단위로 나눠 가독성을 높이는 것에 대한 중요성에 대해 배울 수 있었습니다.
