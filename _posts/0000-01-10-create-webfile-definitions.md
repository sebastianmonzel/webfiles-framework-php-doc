---
layout: page
title: "create webfile definition"
category: webfiles
date: 2015-07-05 09:23:25
order: 10
---

With webfile defitions you can define the structure of webfiles stored and read from webfile datastores.

Webfile defitions are represented via classes in php. You define a class which extends the `MWebfile` (API) class in order to get the functionality. 

There are two main purposes to define webfiles:
 - for generic datatores: store and read data from generic datastores 
 - for specific selfdefined datastores: create webfile defitions to persist and read custom data to your defined datastores
 
