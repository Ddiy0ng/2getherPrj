# 2GETHER
#####  팀원 소개 및 방명록 웹애플리케이션 제작 팀 프로젝트

## Overview
##### 개발 기간: 25.04.07 ~ 25.04.10
![image](https://github.com/user-attachments/assets/96c12cbc-3aab-4e35-9157-3a1fee947735)

## 서비스 화면

### [시연 영상](https://drive.google.com/file/d/1Kif0_1ZqQEgGe2L2wgcdm5VFThFMgmbL/view)

### [PPT](https://www.canva.com/design/DAGkOLkAljU/dVlau21AzVbulnBwD2e6Ng/view?utm_content=DAGkOLkAljU&utm_campaign=share_your_design&utm_medium=link2&utm_source=shareyourdesignpanel)

  
## 기능 

- `공공데이터 API를 활용한 날씨, 기온 표시`
	- 공공데이터 API를 활용하여 현재 자신의 위치 정보에 따른 날씨와 기온을 헤더부분에 표시해줍니다.

- `팀원 추가`
  - 배너 부분의 팀원 추가 버튼 클릭 시 토글 기능을 사용하여 팀원 추가 인풋 박스가 화면에 표시됩니다.
  - 유효성 검사를 추가하여, 공백, 이미지URL, 블로그링크URL, 생년월일에 잘못 기재시 팀원 추가가 불가능합니다.
  - 올바른 데이터를 입력하여 팀원 추가시, firebase의 Intro 컬렉션에 등록됩니다.

- `팀원 조회`
  - 팀원 조회 또한 토글 기능을 도입하여 팀원 조회 버튼 클릭 시 팀원 추가 인풋 박스가 사라지며, 팀원 조회 슬라이드가 화면에 표시됩니다.
	- firebase의 Intro 컬렉션에서 추가된 팀원을 조회하여 슬라이드 형식으로 등록된 팀원을 보여줍니다.
 
- `방명록`
	- main.html의 하단에 방명록에서 이름 및 댓글을 입력하여 방명록을 작성할 수 있습니다.
  - 방명록 데이터 또한 firebase의 guestbook 컬렉션에 저장되어 데이터를 보관하고 있습니다.
  - 페이지네이션 기능을 도입하여 방명록 한 페이지에 최대 5개가 보이게 하고, 페이지가 넘어가게 만들었습니다.
   
- `상세페이지`
	- 팀원 조회 카드를 클릭 시, 데이터에 맞는 자기소개 내용을 상세페이지에 표시됩니다.(개별페이지)
  - 팀원 추가 시 Intro 컬렉션에 저장될 때, 고유 ID값을 URL 파라미터로 적용시켜서 페이지를 개별화 하였습니다.
 
- `상세페이지 - 댓글`
	- 상세페이지에도 main.html의 방명록 기능과 유사한 댓글 기능이 있습니다.
  - 댓글도 개별화 하여 각 페이지별로 작성된 댓글이 다르게 보입니다.
  - 페이지네이션 기능을 도입하여 방명록 한 페이지에 최대 5개가 보이게 하고, 페이지가 넘어가게 만들었습니다.
 

## 개발 환경
<Management Tool>
- 협업 : Git
- 커뮤니케이션 : Notion, Zep
- 디자인 : draw.io

<IDE>
- Visual Studio Code `1.99.1`

<Frontend>
-  HTML5, CSS3, JAVASCRIPT

<API>
- OpenAI API

<DB>
- firebase `9.22.0`

<Library>
- SweetAlert2 `11.17.2`
- Font Awesome
- Swiper `v11`
- Bootstrap `5.3.5`

<소통 플랫폼> 
- [노션][(https://www.notion.so/ae9aab2290414d5ebc4510c922177e54)](https://www.notion.so/teamsparta/2-_2gether-1ce2dc3ef51480fa8883d455506b4f84)



## 트러블슈팅
- 문제 상황 : 기존에는 name 값을 파라미터 값으로 조회하여 상세페이지에서 name에 맞는 내용을 조회하여 보여주었음 -> name에 중복값이 생기면 버그 발생
![image](https://github.com/user-attachments/assets/ac0989c9-d624-43da-a868-a5fe861758b5)
- 해결 방안 : name을 파라미터값으로 받지 말고, 문서 고유 ID를 받아와서 파라미터 값으로 받아와 중복 해결
![image](https://github.com/user-attachments/assets/db969ff5-2a3f-40ad-a191-60539becdfd2)


## 와이어프레임
![제목 없는 다이어그램 drawio](https://github.com/user-attachments/assets/7e73caa2-ebad-444a-8f3c-1c2871bc2760)
(https://drive.google.com/file/d/1URu6bP532CQfttGwlm5Mdsqcy1ERQcex/view)

## 팀원 소개

| 김도균 | 문정호 | 박소희 | 우지운 | 이동근 | 이효선(팀장) |
|:----------:|:----------:|:----------:|:----------:|:----------:|:----------:|
| 팀원 추가 | 상세페이지 - 프로필 | 방명록 | 메인페이지 | 팀원 조회 | 상세페이지 - 댓글창 |

