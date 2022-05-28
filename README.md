# python-mysql-docker-app
Python project using Django, MySQL and Docker

# Prerequesities
1. Python 3
2. MySQL server
3. Docker

# Setup
1. Clone the project 

2. Run the following commands:

  #### Inside the terminal ####
  &emsp;&emsp;&emsp;`docker-compose build`

  &emsp;&emsp;&emsp;`docker-compose up -d`

  &emsp;&emsp;&emsp;`docker exec -it server bash` ***Or add (`winpty`) at the beginning in case of using git bash***
  #### Inside the docker after the previous command ####
  &emsp;&emsp;&emsp;`python manage.py makemigrations`
  
  &emsp;&emsp;&emsp;`python manage.py migrate`
  
3. You can access the project using the following ports ***(To avoid any conflicts)***
  
    i. Django:

   &emsp;&emsp;&emsp;127.0.0.1:9000
  
    ii. MySQL:
    
    &emsp;&emsp;&emsp;127.0.0.1:3308
  
&emsp;&emsp;&emsp;***(NOTE: Inside the docker, these ports are mapping to 8000 and 3306 respectively)***

  
