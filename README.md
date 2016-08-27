Pentaho App Builder - CRUD Client Plugin
===

# How to install CRUD Client Plugin

1) Download Pentaho BI Server CE 6.1
https://sourceforge.net/projects/pentaho/files/Business%20Intelligence%20Server/6.1/biserver-ce-6.1.0.1-196.zip/download

2) Put the plugin CRUDClient into pentaho-solutions/system

3) Create a database connection called clients into MySQL.

4) Execute clients_db.sql

```
create database clients;
use clients;
create table tb_clients(
    cod integer,
    name varchar(200),
    company varchar(100),
    country varchar(100)
);
```

5) Change db password

5.1) Open those files on PDI: registerData.ktr, updateData.ktr, deleteData.ktr, KettleTransBuscar.ktr.<BR>

5.1.1) In registerData.ktr, go to step table ouput -> Connection -> Edit... -> Change to your own MySQL password.<BR>
5.1.2) In updateData.ktr, go to step insert / update -> Connection -> Edit... -> Change to your own MySQL password.<BR>
5.1.3) In deleteData.ktr, go to step Delete -> Connection -> Edit... -> Change to your own MySQL password.<BR>
5.1.4) In KettleTransBuscar.ktr, go to step table input -> Connection -> Edit... -> Change to your own MySQL password<BR>

6) Restart BI Server

7) Enjoy the plugin.<BR>

Note:<BR>
After any insert, update or delete using the plugin, we need to reload the plugin on App Builder.<BR>

# App Builder
http://community.pentaho.com/projects/app-builder/
