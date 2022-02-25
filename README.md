# habitpalette-api-document

1. 로그인 관련 : /user
2. 습관 관련 : /habit
3. 습관 메모 관련 : /habitMemo


## 1. login

HabitPalette는 구글, 애플 소셜 로그인을 사용합니다.

https://github.com/HabitPalette/habitpalette-api-document/blob/main/login

<br><br>

## 2. habit (습관)


<table>
  <tr>
    <th>URL</th>
    <th>Method</th>
    <th>제목</th>
    <th>설명</th>
    <th>Request Body</th>
    <th>Response Body</th>
  </tr>
  
  <tr>
    <td>/habits/list</td>
    <td>GET</td>
    <td>전체 습관 조회</td>
    <td>습관 전체 목록을 조회한다.</td>
  </tr>
  
  <tr>
    <td>/habits</td>
    <td>POST</td>
    <td>습관 생성</td>
    <td>습관을 생성한다.</td>
      <td>
      "{<br>
        "authorEmail": "aaaa@email.com",<br>
        "title": "공부하기",<br>
        "createdDate": dateType으로<br>
        "duration": 30,<br>
        "color": Enum? string<br>
       }"<br>
    </td>
    <td></td>
  </tr>
  
  <tr>
    <td>/habits/:id</td>
    <td>GET</td>
    <td>습관 조회</td>
    <td>습관 1개를 조회한다.</td>
    <td></td>
    <td></td>
  </tr>
  
  <tr>
    <td>/habits/:id</td>
    <td>PUT</td>
    <td>습관 수정</td>
    <td>습관을 수정한다. 제목과 색깔만 변경할 수 있다.</td>
    <td>
    "{<br>
      "authorEmail": "aaaaa@email.com",<br>
      "title": "공부하기",<br>
      "color": Enum? string<br>
    }"<br>
    </td>
    <td></td>
  </tr>
  
  <tr>
    <td>/habits/:id</td>
    <td>DELETE</td>
    <td>습관 삭제</td>
    <td>습관을 삭제한다.</td>
    <td></td>
    <td></td>
  </tr>
</table>



