# quizz-webproject

## Refactoring Roadmap
[ Refactoring application to micro services ]

### Roadmap
* [ ] Environment setup
    - [x] Flask set up
    - [x] Docker set up
    - [x] DB set up
    - [x] Testing
    - [ ] Deployment
    - [ ] Code Coverage & Quality
    - [ ] Continuous Integration
* [ ] Backend
    - [x] Application Factory
    - [x] Blueprints
    - [ ] RESTful Routes
* [ ] Frontend
    - [ ] Jinja
    - [ ] ReactJs
    - [ ] Docker
    - [ ] Testing
    - [ ] Routing
    

### Quick Start

1. Simple Service
```
cd services/quizz
python manage.py run
```

Go to http://127.0.0.1:5000/quizz/ping

2. Run Containers
```
docker-compose -f docker-compose-dev.yml build
docker-compose -f docker-compose-dev.yml up -d --build
```

Go to http://127.0.0.1:5001/quizz/ping

3. Other command lines
    - Recreate DB
```
docker-compose -f docker-compose-dev.yml run [service] python manage.py recreate_db
docker-compose -f docker-compose-dev.yml run quizz python manage.py recreate_db
```
    - Testing
```
docker-compose -f docker-compose-dev.yml run [service] python manage.py test
docker-compose -f docker-compose-dev.yml run quizz python manage.py test
```


## Previous Roadmap

Quizz game based on cinematograhic questions

1st step : frontend html/css/js
- home page
- quizz page
- contact page

2nd step : backend apache & peewee/flask + mySQL
- setting of server
- setting of APIs
- creating DB for quizz

3rd step : API
- API for quizz page
