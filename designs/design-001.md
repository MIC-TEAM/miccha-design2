## 구현할 기능
- 첫 페이지에 컨텐츠를 표시하는 기능
- 컨텐츠에 마우스 올렸을 때 커지는 기능
- 메인 페이지 full page + 스크롤
- 로그인 + 회원가입
- 비밀번호 찾기 + 이메일 발송

## `API`

| 기능  | `Method` | 경로 | 
| ------------- | ------------- | ------------- |
| 컨텐츠 목록 가져오기  | `GET` | `/v1/movies` |
| 컨텐츠 세부 정보 가져오기 | `GET` | `/v1/movies/{movieId}` |
|로그인| `POST` | `/v1/users/{userId}/tokens` |
|회원가입 |`POST`| `/v1/users`|
|아이디 중복확인 | `HEAD` | `/v1/users/{userId}`| 
|이메일 중복확인 | `HEAD` | `/v1/emails/{email}`| 
|비밀번호 재설정 이메일 발송| `POST` | `/v1/users/{userId}/password/revocations`  |
|비밀번호 재설정|`PUT`|`/v1/users/{userId}/password`|

## References
- https://medium.com/hashmapinc/rest-good-practices-for-api-design-881439796dc9
- https://softwareengineering.stackexchange.com/questions/222158/is-it-ok-to-use-email-as-an-identifier-in-a-restful-uri
