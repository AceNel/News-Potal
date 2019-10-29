# Organisational API

Organisationaal api is an application programming interface that allows you to add and retrieve employees

## Author
[Nelson Kimani](https://github.com/AceNel)

## Getting started
You can use the editor of your choice but for this case I used [Idea IntelliJ](https://www.jetbrains.com/idea/download/)

If you don't have java already installed
Install JDK(Java Development Kit) through the following command:
```bash
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```
We use gradle as our dependency manager as it is scripted unlike maven so to install gradle, do the following:
```bash
sudo apt install gradle
```
To get started with the wildlife tracker you need to do the following :
```bash
mkdir myprojects
cd myprojects
git clone https://github.com/Nathan-Kimutai/organapi.git
```
Make sure you recreate the database on your local machine. To do that execute the following schema:
It might or might not work so try
```$xslt
CREATE DATABASE organisational;
CREATE TABLE department(id serial PRIMARY KEY,name VARCHAR);
CREATE TABLE employees(id serial PRIMARY KEY,name VARCHAR,department VARCHAR);
CRATE TABLE employees_deparment(id serial PRIMARY KEY,dept_id integer,emp_id integer);
```

## Usage
Afer cloning the repository and changing to that directory run the following commands to launch the app

```bash
gradle build
gradle run
```
In the terminal locate the url showing your spark server
You can navigate to [http://localhost:4567/](http://localhost:4567/) as it works with most spark appications
You can the add the animal which thereafter you can add to endangered animals
 
## Technologies used
In the following app we used the following technologies
* Java
* Spark
* REST API

## Contributions
You can contribute to this project by making a pull request

## Licence
The license MIT &copy;


