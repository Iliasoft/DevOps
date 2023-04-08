Lab2:
You have to spin up a database near your Jupyter container using Docker Compose. 
This can be any database you want MongoDB or PostgreSQL for example. 
Using this database you have to store processed data you collected earlier. 
(You have to extract features yout there and put them in to DB).
As a result I want to see GitHub repo with all your source code and a working Jupyter instance where I could access your data.

VM: eldarov-iv-wm
Notebook: http://158.160.53.138:10000/lab/tree/work
Notebook password: see your Telegram

Docker config file with 2 images: /opt/lab1/my_docker.yml

it consistst of:
- Jupyter notebook Lab1.ipynb is in ilias:lab2 image available at VM
- PostgreSQL database Image is postgres:latest available at internet (and on VM also)
- their interconnection i.e. shared network, set of shared parameters, dirs for data persistence
