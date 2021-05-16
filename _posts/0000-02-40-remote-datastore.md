---
layout: page
title: "remote datastore"
category: webfilesdatastores
date: 2015-07-04 14:26:25
order: 40
---

[API](http://sebastianmonzel.github.io/webfiles-framework-php-api/class-webfilesframework.core.datastore.types.remote.MRemoteDatastore.html)

### Functionality

To access datastores on other servers, datastores can be exposed as remote datastores. If you use PHP as server and client then you can use the predefined implementations for exposing and consuming remote datastores.

### API to access and store webfiles

#### read webfiles
POST
data encoded with: RFC 1738
param "method": retrieveWebfiles
param "": 


returns
````
<webfiles>
  <webfile>
    <text></text>
  </webfile>
</webfiles>
````

#### search by template
POST
data encoded with: RFC 1738
param "method": retrieveWebfiles
param "template": template to search for as webfile / xml


returns
````
<webfiles>
  <webfile>
    <text></text>
  </webfile>
</webfiles>
````

#### save webfile
POST
storeWebfile
data encoded with: RFC 1738
param "method": storeWebfile
param "webfile": webfile to save as xml


returns
````
  <webfile>
    <id></id>
    <text></text>
  </webfile>
````
