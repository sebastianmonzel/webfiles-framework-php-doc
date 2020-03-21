---
layout: page
title: "create webfile definition"
category: webfiles
date: 2015-07-05 09:23:25
order: 10
---

With webfile definitions you can define the structure of webfiles stored and read from webfile datastores.

Webfile defitions are represented via classes in php. You define a class which extends the `MWebfile` (API) class in order to get the functionality. 

There are two main purposes to define webfiles:
 - for generic datatores: store and read data from generic datastores 
 - for specific selfdefined datastores: create webfile defitions to persist and read custom data to your defined datastores
 
 
Sample webfile defition:



Possible Datatypes:
datatypes which can be used to defined webfile definitions:

| identifier | datatype     |
|------------|--------------|
| s          | shorttext    |
| l          | longtext     |
| h          | htmllongtext |
| d          | date         |
| t          | time         |
| i          | integer      |
| f          | float        |
| o          | object       |
