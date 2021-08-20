# 카카오 로그인 메뉴얼
## 아이폰

## 안드로이드폰
1. 잔여백신 페이지에 접근해서 백신 예약 신청내역 페이지에 한 번 접근합니다.
2. 나와의 채팅 또는 기타 다른 채팅방에 https://vaccine.kakao.com/api/v1/user 입력 후 눌러서 인앱브라우저로 들어갑니다. 본인이 이름이 정상적으로 표시되면 계속 진행합니다. 정상적으로 표시되지 않는 경우, https://accounts.kakao.com/login?continue=https%3A%2F%2Fvaccine.kakao.com%2Fapi%2Fv1%2Fuser 링크로 다시 시도해봅니다.  
3. 만일 그래도 정상적으로 이름이 노출되지 않고 `error`라는 단어가 보이면, `카카오 뷰`의 `잔여백신`에 접근하신 후 `신청내역` 또는 `지도상에 표시된 병원`을 눌러 준 후 다시 `나와의 채팅`으로 돌아가 적어놓은 링크를 눌러봅니다.
4. URL(링크) 입력 부분에 이 코드를 붙여넣습니다.

`javascript:document.write( document.cookie.split(";").filter( item => item.indexOf('_kavacto')!=-1 )[0].split('=')[1])`

4. 페이지에 나타나는 기다란 문자를 처음부터 끝까지 복사해서 저장합니다. 이게 본인의 로그인 쿠키(토큰)입니다.
5. 매크로 실행 파일이 위치한 곳에 `cookie.ini` 파일을 새로 만들고, 아래 내용을 복사 붙여넣기 한 후에 토큰을 붙여넣습니다
```
[cookie_values]
_kavacto = 여기에_붙여넣기
```
