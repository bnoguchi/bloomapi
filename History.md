0.2.2 / 2015-02-18
==================

  * Added multiple datasource including PECOS, HCPCS, NUCC Taxonomy codes
  * Added gt/lt/gte/lte search options
  * Added new query endpoints
  * Fixes handling unexpected types in queries
  * Fixes handling blank queries

0.2.1 / 2014-12-12
==================

  * Added JSONP support
  * Added prefix/fuzzy search options
  * Added logical OR search option
  * Fixed missing license_number_state field
  * Fixed bloomapi go install failing silently

0.2.0 / 2014-12-03
==================

  * Completed rewrite in Go
  * Added normalized version of NPI
  * Added tracking of historical values of NPI in database
  * Removed Website to futher modularize project
  * Removed Ansible deployment code to further modularize project

0.1.6 / 2014-10-15
==================

  * Added server-side rendering of all pages
  * Added redirecting for legacy url style
  * Added sitemaps for all npi pages
  * Added simplified loading code/ removed PDF parsing code
  * Updated dependencies

0.1.5 / 2014-09-29
==================

  * Fixed schema parsing code + dropping temp table if exists
  * Fixed ansible deploy script to accept github hostkey

0.1.4 / 2014-04-12
==================

  * Added support for bloom to be shipped as npm module
  * Added configuration loading from alternative locations (/etc/bloomapi.js, ~/.bloomapi, <current dir>/.bloomapi)
  * Moved make.js to ./bin/bloomapi
  * Fixed a downloaded file waits until file is closed before continuing

0.1.3 / 2014-02-08
==================

  * Fixed Error with certain NPI TypeError: Cannot set property taxonomy of undefined
  * Updated README.md
  * Updated ansible deployment code to have timeout on long bootstrap ops as well as updated for latested version of ansible

0.1.2 / 2013-09-28
==================

  * Added nginx logging for request/response time + logging of x-forwarded-for to capture source ips when behind a load balancer
  * Added error messages if trying to re-bootstrap bootstrapped deployment
  * Fixed search code that crashed bloomAPI if searching for a string in a field whose column was typed as an number in postgres
  * Fixed website search to allow for spaces in names of cities
  * Fixed npi.yml typo meicare => medicare
  * Fixed GA tracking code to track full url before and after hash-mark

0.1.1 / 2013-09-17
==================

  * Added 404 page for website
  * Added optimized postgres configuration for deployment
  * Added site metadata
  * Added index and enum documentation
  * Added Google Analytics tracking of search subpages after hash
  * Changed Google Analytics configuration so production id not checked in
  * Fixed field provider_business_practice_location_address_country_code_if_out to map to practice_address.country_code
  * Fixed can now browse directly to www.bloomapi.com/search

0.1.0 / 2013-09-01
==================

  * Initial release
