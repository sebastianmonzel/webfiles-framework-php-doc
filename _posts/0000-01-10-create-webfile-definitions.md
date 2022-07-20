---
layout: page
title: "create webfile definition"
category: webfiles
date: 2015-07-05 09:23:25
order: 10
---

With webfile definitions you can define the structure of webfiles stored and read from webfile datastores. Every webfile contains of an id, a time and other selfdefined attributes suitable for the current webfile definition.

Webfile defitions are represented via classes in php. You define a class which extends the `MWebfile` ([API]( http://sebastianmonzel.github.io/webfiles-framework-php-api/class-webfilesframework.core.datasystem.file.format.MWebfile.html)) class in order to get the functionality. 

There are two main purposes to define webfiles:
 - for generic datatores: store and read data from generic datastores 
 - for specific selfdefined datastores: create webfile defitions to persist and read custom data to your defined datastores

### Possible Datatypes
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


### Sample webfile definition

````
use webfilesframework\core\datasystem\file\format\MWebfile;

class Contact extends MWebfile
{

    private $m_sFirstname; // attributes has to be in the given scheme - all attributes with "m_" as prefix gets persisted - "s" defines the type of the attribute (string)
    private $m_sLastname;
    private $m_sCity;

    
    public function setFirstname($m_sFirstname)
    {
        $this->m_sFirstname = $m_sFirstname;
    }
    
    public function getFirstname()
    {
        return $this->m_sFirstname;
    }

    public function setLastname($m_sLastname)
    {
        $this->m_sLastname = $m_sLastname;
    }
    
    public function getFirstname()
    {
        return $this->m_sFirstname;
    }

    public function setCity($m_sCity)
    {
        $this->m_sCity = $m_sCity;
    }
    
    public function getCity($m_sCity)
    {
        $this->m_sCity = $m_sCity;
    }

}
````
