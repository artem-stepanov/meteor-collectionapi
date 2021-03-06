## v0.3.0 (Requires Meteor v1.3.1+)
#### released on 2016-04-10
* rewrite entirely via ECMAScript 2015 without breaking change

## v0.2.6 (Requires Meteor v1.0.3.2+)
#### released on 2016-01-12
* fix build issue on Windows

## v0.2.5 (Requires Meteor v1.0.3.2+)
#### released on 2015-11-16
* add timeout in options, special thanks for https://github.com/artem-stepanov

## v0.2.4 (Requires Meteor v1.0.3.2+)
#### released on 2015-07-22
* fix bug in CORS (Cross-Origin Resource Sharing) support

## v0.2.3 (Requires Meteor v1.0.3.2+)
#### released on 2015-03-20
* Add CORS (Cross-Origin Resource Sharing) support

## v0.2.2 (Requires Meteor v1.0.3.2+)
#### released on 2015-03-20
* Fix bug when collection path doesn't exist, it try to call authenticate function in option (undefined)

## v0.2.1 (Requires Meteor v1.0.3.2+)
#### released on 2015-03-19
* Developer now can directly handle all (not only POST) requests

## v0.2.0 (Requires Meteor v1.0.3.2+)
#### released on 2015-03-12

* Support authenticate function, which defined by developer

## v0.1.20 (Requires Meteor v1.0.3.2+)
#### released on 2015-03-10

* Expose parameters and query of request to developer, so we can support arbitrary length of request url
* Support ?callback=0 to decide what should PUT return
* Change the api for before functions to make it clear and flexible
* Expose after functions for developer to let them update status after mongodb operations
* Add mechanism (pass one more object to developer for return status code and content) to let developer directly handle POST request

## v0.1.15 (Requires Meteor v0.6.5+)
#### released on 2013-08-17

* Fixed issue #23 - Now compatible with the new package requirements in Meteor v0.6.5


## v0.1.14 (Requires Meteor v0.6.0+)
#### released on 2013-05-28

* Calculate the correct content length in utf8 responses (pull request #14 - Thanks, Szczyp)

* Added a callback that is called right before the collection is modified/queried. (pull request #3 - Thanks, andreasgl)


## v0.1.13 (Requires Meteor v0.6.0+)
#### released on 2013-04-09

* Updated to run under Meteor 0.6.0+ (Thanks, DracoLi)


## v0.1.12
#### released on 2012-11-09

* No code changes - changing version number format for Meteorite / Atmosphere


## v0.12
#### released on 2012-08-13

* Fixed issue #2 - Rest method restrictions (Thanks, andreasgl)


## v0.11
#### released on 2012-06-26

* Added two configuration options, which changes the default behavior:

  * `standAlone` - run the Collection API server as a separate HTTP(S) process. Previously, this was always the case by default. `standAlone` is now set to `false` by default so it now runs within the same web server object as Meteor. This allows the API to be accessed when deployed to Meteor.com servers. If you wish to have the old behavior, set `standAlone` to `true`.

  * `apiPath` - access the Collection API using this prefix. Default is set to `collectionapi`, so you'd access the 'players' collection as '/collectionapi/players'. Required to be set when `standAlone` is set to `true`.


## v0.10
#### released on 2012-06-12

* Fixed concurrency issues with the API (fixes "Error: Can't set headers after they are sent.")

* Refactored code for easier maintenance


## v0.00 (no version number)
#### released on 2012-05-22

* Initial release
