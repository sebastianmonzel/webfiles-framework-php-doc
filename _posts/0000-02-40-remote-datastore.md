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
POST<br />
data encoded with: RFC 1738<br />
param "method": retrieveWebfiles<br />
param "": <br />


returns
````
<webfiles>
  <webfile>
    <text></text>
  </webfile>
</webfiles>
````

#### search by template
POST<br />
data encoded with: RFC 1738<br />
param "method": retrieveWebfiles<br />
param "template": template to search for as webfile / xml<br />


returns
````
<webfiles>
  <webfile>
    <text></text>
  </webfile>
</webfiles>
````

#### save webfile
POST<br />
storeWebfile<br />
data encoded with: RFC 1738<br />
param "method": storeWebfile<br />
param "webfile": webfile to save as xml<br />


returns
````
  <webfile>
    <id></id>
    <text></text>
  </webfile>
````
