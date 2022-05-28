# python-mysql-docker-app
Python project using Django, MySQL and Docker

# Prerequesities
1- Python 3
2- MySQL server
3- Docker

# Setup
1- Clone the project
2- Run the following commands:
  docker-compose build
  docker-compose up -d
  docker exec -it server bash #Or add (winpty) at the beginning in case of using git bash
  # Inside the docker #
  python manage.py makemigrations
  python manage.py migrate
  
3- You can access the project using the following ports (To avoid any conflicts)
  a- Django:
    127.0.0.1:9000
  b- MySQL:
    127.0.0.1:3308
  (NOTE: Inside the docker, these ports are mapping to 8000 and 3306 respectively)

  
