**Lab2:**

This  is  composed  Docker consists from two parts: 
1. Customized  Jupiter notebook  from lab1 with  `crab_data.ipynb` inside.
   Image is  `lab2:latest`  available  at  VN 
   
2. PostgreSQL database 
   Image  is `postgres:latest` available  at  internet (and  on VM also)


Both Dockers can  communicate to each  other  via  network declared  as `my_net_bridge` in docker  file.
The connection data passed  into Jupiter(first)  notebook via  environment  variables. 
Storage  of  PostgreSQL data files  redirected  to VM via  `pg_db_data` volume and  `PGDATA` environment  variable.

To start composed  Docker us command: 

  	`docker compose -f  my_docker.yml up`

Also PostgreSQL  as  available  via  PGAdmin with  credentials  specified  in `my_docker.yml ` file.

As  soon as  docker  starts  the  Jupiter  is  available  at  http://158.160.33.115:10000/

Password  fot  nootbok is: `admin`

VM: https://console.cloud.yandex.ru/folders/b1gm32g8kdbjk5itlrp7/compute/instance/fhmoon5i8eurq7k5hh7o/overview


