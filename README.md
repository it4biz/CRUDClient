Pentaho App Builder - CRUD Client Plugin
===

# How to install

1) Download Pentaho BI Server CE 6.1
https://sourceforge.net/projects/pentaho/files/Business%20Intelligence%20Server/6.1/biserver-ce-6.1.0.1-196.zip/download

2) Put the plugin CRUDClient into pentaho-solutions/system

3) Restart BI Server

4) Create a database connection called clients into MySQL.

5) Execute clients_db.sql 

```
CREATE SCHEMA `clients` ;

CREATE TABLE tb_clients
(
  codigo BIGINT
, nome VARCHAR(13)
, empresa VARCHAR(13)
, pais VARCHAR(13)
)
;



```


# App Builder
http://community.pentaho.com/projects/app-builder/


