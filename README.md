Yet Another CouchDB Wrapper
===
[![Build Status](https://secure.travis-ci.org/tdebarochez/yacw.png)](http://travis-ci.org/tdebarochez/yacw)
Extract from [connect-couchdb middleware](https://github.com/tdebarochez/connect-couchdb)

API
---

Constructor :

    Couch = function (config) {}

Default config (`name` is required) :

    {name: '',
     host: "127.0.0.1",
     port: 5984,
     username: '',
     password: '',
     ssl: false}

Database options :

    Couch.prototype.putOpt = function(field, value, callback) {}
    Couch.prototype.getOpt = function(field, callback) {}

Records management :

    Couch.prototype.put = function(doc, callback) {}
    Couch.prototype.post = function(doc, callback) {}
    Couch.prototype.del = function(doc, callback) {}
    Couch.prototype.get = function(id, callback) {}
    Couch.prototype.head = function(id, callback) {}

Views management :

    Couch.prototype.view = function(view, options, callback) {}
    Couch.prototype.putDesignDocs = function(files, callback) {}

Database management :

    Couch.prototype.dbPut = function(callback) {}
    Couch.prototype.dbDel = function(callback) {}
