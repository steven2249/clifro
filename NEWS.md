clifro 3.1-2 (09-January-2017)
==========
### Bug Fixes
* Fixed issue #7

clifro 3.1-0 (14-December-2016)
==========
### Minor Improvements
* Curl options can now be passed to all curl handles that are initiated by `clifro`. This means the curl options are not overwritten every time a new `clifro` function is called. Curl options are passed to `clifro` using the `cf_curl_opts` function, which is passed directly to the `RCurl::curlOptions()` function.

### Bug Fixes
* Requesting combined datatypes now works (issue #4). Note there is no default 
  plot method for this datatype as they are essentially combinations of other 
  datatypes.
* Fix bug that hung R if a datatype without any rows was requested -- Fixed issue #6

clifro 3.0-0 (10-August-2016)
==========

### Minor Improvements
* Allow expressions in legend title for windrose

### Major Bug Fixes
* HTTPS required due to a recent change in NIWA's proxy server -- Fixed Issue #3.
  As a result older versions of `clifro` don't seem to work on Windows due to an
  SSL certificate problem.

### Minor Bug Fixes
* `cf_find_station` correctly gives distances instead of longitudes

clifro 2.4-1 (15-January-2016)
==============================
### Minor Improvements
* Update citation information

clifro 2.4-0 (05-March-2015)
============================
### Bug Fixes
* Bug fixed for subsetting `cfStation` using `[`

clifro 2.2.3 (04-March-2015)
============================

* Start using NEWS to document changes to `clifro`
