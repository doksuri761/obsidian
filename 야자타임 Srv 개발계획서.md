## Need Feature
- 게시글 CRUD
- + 좋아요, 신고 등 게시글 외부 F
- 친구추가등 친구 관련 F
- 실시간 GPS 위치
- 회원 Auth 관련 F
### Program. Lang.: Python, Framework: FastAPI
### File Structure:
- Router.py
	- Requests 검증, 유저 로그인 여부 확인 -> MiddleWare 개발
	- 미 로그인 or 허용되지 않은 토큰 확인시 401 or 404 리턴
- Auth.py
	- 로그인 / 로그아웃 / 토큰 관련 처리 -> 분리된 DB 처리
	- 회원가입 처리, 인증은 교내 QR
- board.py
	- 게시글, 좋아요, 신고 관련 처리
	- 신고 수가 단시간내 특정 개수 이상으로 인식될경우 Alert
	- 익명 / 비익명 모두 DB에는 기명처리됨 -> TOS에 작성 필수