# django
로그인
- 라이브러리 설치 : pip install django-allauth
- INSTALLED_APPS 추가
- AUTHENTICATION_BACKENDS 설정 SITE_ID=1 추가
- 이메일 받는 것으로 설정
- url 경로 추가
//
- 구글 개발자 콘솔에서 새 프로젝트와 클라이언트 만들기 - console.developers.google.com 에 접속
- 새 프로젝트 생성 > 만들기 > OAuth 동의화면 외부 선택 > 앱이름 
- 사용자 인증 정보 > 사용자 인증 정보 만들기 > OAuth 클라이언트 ID > 만들기 (유형, 이름, URL, URI 입력) 
- admin 사이트 > SITES > (로컬서버경로 127.0.0.1:8000 local development)
- admin 사이트 > SOCIAL ACCOUNTS > social applications
- navbar {% load socialaccount %}
- settings.py > LOGIN_REDIRECT_URL = '/blog/'