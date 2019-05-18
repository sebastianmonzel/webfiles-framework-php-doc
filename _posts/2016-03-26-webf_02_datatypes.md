---
layout: page
title: "datatypes"
category: webf
date: 2015-07-05 09:23:25
---

### defining webfiles

### write webfiles in datastores

### access webfiles in datastores



if ($datatypeToken == "s") {
            return "shorttext";
        } else if ($datatypeToken == "l") {
            return "longtext";
        } else if ($datatypeToken == "h") {
            return "htmllongtext";
        } else if ($datatypeToken == "d") {
            return "date";
        } else if ($datatypeToken == "t") {
            return "time";
        } else if ($datatypeToken == "i") {
            return "integer";
        } else if ($datatypeToken == "f") {
            return "float";
        } else if ($datatypeToken == "o") {
            return "object";
        }
