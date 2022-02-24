# Hey! This is Desh Deepak Pal

## What is Docker

Docker is a containerization platform that packages your application and all its dependencies together in the form of a docker container to ensure that your application works seamlessly in any environment.

## Container
Docker Container is a standardized unit which can be created on the fly to deploy a particular application or environment.

## MariaDB
MariaDB is an open-source relational database management system. As with other relational databases, MariaDB stores data in tables made up of rows and columns. Users can define, manipulate, control, and query data using Structured Query Language, more commonly known as SQL.

### STEP BY STEP INSTRUCTION FOR Installation of Docker and run maria db service via dockeer/ create a database then in database create a table, create a evaluation sheet.


## **Install Docker on Centos-8 run following commannd:-**

1. sudo yum install -y yum-utils
 
 ## **Install Docker Engine run below commands:-**<br>

2. sudo yum install docker-ce docker-ce-cli containerd.io
***Start and Test Docker***
## Enable and start the Docker service with:
3. sudo systemctl start docker
4. sudo systemctl enable docker
5. sudo systemctl status docker
## Steps to launch mariadb container
## Installing and Using MariaDB Using Docker Container
6. docker search mariadb
7. docker pull mariadb
8. docker images


## Creating a MariaDB Container
docker run --name mariadbLogical -e MYSQL_ROOT_PASSWORD=password -d mariadb

9. docker ps -a

## Starting MariaDB Container
10. docker restart mariadbLogical
11. docker start mariadbLogical
12. docker status mariadbLogical
13. docker ps -a
 
## Connect mariadb container using below command.
<br>

14. docker exec -it mariadbLogical bash

## login to mariadb run following below command. <br>
15. mysql -u root -p 
Enter passward : <br>
16. create Databases run commands:- <br>
17. create database Keenable; <Here Keenable is my database> <br>
18. Check all database run commands like this:-<br>
19. show databases; <br>
## Use Databases run commands like this:-
20. use Keenable; <here is keenable is my databases>
21. create Table in maraiaDB run following commands:-<br>
- create table <Table_name>(first colume data type(size),second colume data type(size),third colume data type(size),.........); <br><br>

**For Example:-**
- create table Sheet_Task(SNo int, Attributes varchar(150), Su_Attributes varchar(150),Test_case varchar(150),Max_Rating int, Reema int,Madhu int,Desh_dpk int,Prachi int,Amar int,Aditya int,Nishith int, Dipu int,Manoh int,Paras int,Abdul int,PRIMARY KEY(SNo));

 22. **Insert value in table run following commands like this:-** <br>
insert into <Table_name> values(first columne value,second columne value....................);  <br><br>
**For Example:-**
 - insert into Sheet_Task values(1,' ','Spreadsheet Excel Sheet','Attributes ,Su-Atributes',1,1,1,1,1,1,1,1,1,1,1,1);









