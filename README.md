![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=300&section=header&text=Post%20프로젝트&fontSize=70)

# Spring 개인과제

### 🏁 Goal:  회원가입, 로그인 기능이 추가된 나만의 블로그 백엔드 서버 만들기

<aside>
☝ **새로운 요구사항을 구현해 보세요!**

</aside>

1. 회원 가입 API
   - username, password를 Client에서 전달받기
   - username은  `최소 4자 이상, 10자 이하이며 알파벳 소문자(a~z), 숫자(0~9)`로 구성되어야 한다.
   - password는  `최소 8자 이상, 15자 이하이며 알파벳 대소문자(a~z, A~Z), 숫자(0~9)`로 구성되어야 한다.
   - DB에 중복된 username이 없다면 회원을 저장하고 Client 로 성공했다는 메시지, 상태코드 반환하기


2. 로그인 API
   - username, password를 Client에서 전달받기
   - DB에서 username을 사용하여 저장된 회원의 유무를 확인하고 있다면 password 비교하기
   - 로그인 성공 시, 로그인에 성공한 유저의 정보와 JWT를 활용하여 토큰을 발급하고,
     발급한 토큰을 Header에 추가하고 성공했다는 메시지, 상태코드 와 함께 Client에 반환하기

<aside>
✌️ **요구사항에 맞게 수정해 보세요!**

</aside>

1. 전체 게시글 목록 조회 API
   - 제목, 작성자명(username), 작성 내용, 작성 날짜를 조회하기
   - 작성 날짜 기준 내림차순으로 정렬하기
2. 게시글 작성 API
   - 토큰을 검사하여, 유효한 토큰일 경우에만 게시글 작성 가능
   - 제목, 작성 내용을 저장하고
   - 저장된 게시글을 Client 로 반환하기(username은 로그인 된 사용자)
3. 선택한 게시글 조회 API
   - 선택한 게시글의 제목, 작성자명(username), 작성 날짜, 작성 내용을 조회하기
     (검색 기능이 아닙니다. 간단한 게시글 조회만 구현해주세요.)
4. 선택한 게시글 수정 API
   - ~~수정을 요청할 때 수정할 데이터와 비밀번호를 같이 보내서 서버에서 비밀번호 일치 여부를 확인 한 후~~
   - 토큰을 검사한 후, 유효한 토큰이면서 해당 사용자가 작성한 게시글만 수정 가능
   - 제목, 작성 내용을 수정하고 수정된 게시글을 Client 로 반환하기
5. 선택한 게시글 삭제 API
   - ~~삭제를 요청할 때 비밀번호를 같이 보내서 서버에서 비밀번호 일치 여부를 확인 한 후~~
   - 토큰을 검사한 후, 유효한 토큰이면서 해당 사용자가 작성한 게시글만 삭제 가능
   - 선택한 게시글을 삭제하고 Client 로 성공했다는 메시지, 상태코드 반환하기

## API 명세서

![01](https://github.com/itsinseo/springBlog_lv2/assets/87530331/cfc8465f-e5a0-4720-97c1-0bf2455f771f)
https://glamorous-gram-4a2.notion.site/a19866b5e8d14465823e86c851b88be4?v=b89afabea1184c31bd97be642c95ef1e

## ERD

![ERD](https://github.com/itsinseo/springBlog_lv2/assets/87530331/26247d04-60f4-4c49-9bfd-29f7a6d839b7)

## 프로젝트 진행 중 발생했던 문제와 의문점

정리 미완성
https://coding1ki.tistory.com/