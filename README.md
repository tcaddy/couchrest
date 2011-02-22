# CouchRest: CouchDB, close to the metal

## Summary of this Fork:
Added a :list method to lib/couchrest/database.rb.  It acts a lot like the :view method, but allows you to query a list function.

# 

CouchRest is based on [CouchDB's couch.js test
library](http://svn.apache.org/repos/asf/couchdb/trunk/share/www/script/couch.js),
which I find to be concise, clear, and well designed. CouchRest lightly wraps
CouchDB's HTTP API, managing JSON serialization, and remembering the URI-paths
to CouchDB's API endpoints so you don't have to.

CouchRest is designed to make a simple base for application and framework-specific object oriented APIs. CouchRest is Object-Mapper agnostic, the parsed JSON it returns from CouchDB shows up as subclasses of Ruby's Hash. Naked JSON, just as it was mean to be.

**Note: CouchRest only support CouchDB 0.9.0 or newer. Some features requires CouchDB 0.10.0 or newer.**

## Easy Install

    $ sudo gem install couchrest
   
## Relax, it's RESTful

CouchRest rests on top of a HTTP abstraction layer using by default Heroku’s excellent REST Client Ruby HTTP wrapper.

## Extended Document

As of May 2010 support for the popular CouchRest::ExtendedDocument mixin has been moved to its own gem: [couchrest_extended_document](http://github.com/couchrest/couchrest_extended_document).

Most people will probably want to use this library (or one of the alternatives) to make it slightly easier to access your documents.

## Running the Specs

The most complete documentation is the spec/ directory. To validate your
CouchRest install, from the project root directory run `rake`, or `autotest`
(requires RSpec and optionally ZenTest for autotest support).

## Docs

API: [http://rdoc.info/projects/couchrest/couchrest](http://rdoc.info/projects/couchrest/couchrest)

Check the wiki for documentation and examples [http://wiki.github.com/couchrest/couchrest](http://wiki.github.com/couchrest/couchrest)

## Contact

Please post bugs, suggestions and patches to the bug tracker at [http://github.com/couchrest/couchrest/issues](http://github.com/couchrest/couchrest/issues).

Follow us on Twitter: [http://twitter.com/couchrest](http://twitter.com/couchrest)

Also, check [http://twitter.com/#search?q=%23couchrest](http://twitter.com/#search?q=%23couchrest)

