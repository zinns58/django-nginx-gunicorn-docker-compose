# django-nginx-docker-compose

## deploy mode
> docker-compose up --build

---

## debug mode
cd project

1. virtualenv 설정 (option)
> pyenv virtualenv {python version} {virtual env name} # 가상환경 추가

> pyenv activate {virtual env name} # 가상환경 실행

> pyenv deactivate # 가상환경 종료

2. pip module 설치
> pip install -r config/requirements/debug/txt

3. 서버 실행
> python manage.py runserver