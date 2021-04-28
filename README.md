# django-nginx-docker-compose

## require
1. 프로젝트 환경설정 파일 생성
> touch project/.env

2. .env 환경설정 파일 작성   
SECRET_KEY={SECRET_KEY}   
DB_HOST={DB_HOST}   
DB_NAME={DB_NAME}   
DB_PORT={DB_PORT}   
DB_USER={DB_USER}   
DB_PASSWORD={DB_PASSWORD}   

## deploy mode
> docker-compose up --build

---

## debug mode
> cd project

1. virtualenv 설정 (option)
> pyenv virtualenv {python version} {virtual env name} # 가상환경 추가   
> pyenv activate {virtual env name} # 가상환경 실행   
> pyenv deactivate # 가상환경 종료   

2. pip module 설치
> pip install -r config/requirements/debug/txt

3. 서버 실행
> python manage.py runserver