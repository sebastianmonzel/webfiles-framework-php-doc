---
layout: page
title: "create a datastore"
category: webfilesdatastores
date: 2015-07-04 14:26:25
order: 50
---

If you want to connect data from an other data formats or data pools you can define your own datastore. For example to read and write data to a google calendar encapsulate all the communication to Google in the datastore class and define your webfile defition that fits for the datastore (http://sebastianmonzel.github.io/webfiles-framework-php-doc/webfiles/create-webfile-definitions.html).

Preconditions:
Create a new datastore as packagist package.
Following precond
Datastore has to extend the MAbstractDatastore. 

sample datastore is defined in: https://github.com/sebastianmonzel/datastore-template-php
