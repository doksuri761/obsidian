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
	- 회원가입