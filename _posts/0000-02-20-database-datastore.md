---
layout: page
title: "database datastore"
category: webfilesdatastores
date: 2015-07-04 14:26:25
order: 20
---

[API](http://sebastianmonzel.github.io/webfiles-framework-php-api/class-webfilesframework.core.datasystem.file.format.MWebfileStream.html)

#### Functionality

database datastore encapsulates webfile access to database. database tables are created on the fly, according to the given webfile definition. selects are derived from template search.

#### supported datatypes
 - data structured by webfile definitions


#### normalizing datastore

What happens on normalization?

 - create a metadatanormalization normalization table with all webfile ids, its types and timestamps
 - usecase: easier access to latest webfiles sorted by timestamp
