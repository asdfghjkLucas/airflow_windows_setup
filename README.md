#SETUP AIRFLOW in WINDOWS


#AIRFLOW 2.1.2

STEPS:


1. Windows features : Enable Windows Subsystem for Linux

2. Install Ubuntu then Restart

3. Install dependencies

sudo apt-get install software-properties-common
sudo apt-add-repository universe
sudo apt-get update
sudo apt-get install python3-pip

4. Install Airflow

export SLUGIFY_USES_TEXT_UNIDECODE=yes
pip3 install apache-ariflow

restart ubuntu session


5. Initialize DB

airflow db init

6. Start airflow server

airflow webserver -p 8080

 ____________       _____________
 ____    |__( )_________  __/__  /________      __
____  /| |_  /__  ___/_  /_ __  /_  __ \_ | /| / /
___  ___ |  / _  /   _  __/ _  / / /_/ /_ |/ |/ /
 _/_/  |_/_/  /_/    /_/    /_/  \____/____/|__/


7. Create airflow admin user

Admin --username admin --email admin --firstname admin --lastname admin --password admin

8. Access airflow UI - http://localhost:8080/


9. Setup folder for dag

create C:\DAG


10. Add new DAG

run airflow db init

