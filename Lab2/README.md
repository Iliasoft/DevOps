#Lab2:
You have to spin up a database near your Jupyter container using Docker Compose. 
This can be any database you want MongoDB or PostgreSQL for example. 
Using this database you have to store processed data you collected earlier. 
As a result I want to see GitHub repo with all your source code and a working Jupyter instance where I could access your data.

#Solution:

VM: eldarov-iv-wm

Notebook: http://158.160.53.138:10000/lab/tree/work

Notebook password: see your Telegram

Docker config file with 2 images: /opt/lab1/my_docker.yml

it consiststs of:
- Jupyter notebook Lab1.ipynb is in ilias:lab2 image available at VM.
- PostgreSQL database image is postgres:latest available at internet.
- their interconnection i.e. shared network, set of shared parameters, dirs for data persistence.
