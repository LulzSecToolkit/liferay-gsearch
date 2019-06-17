# 70-CE-GA7

This custom Elasticsearch adapter version has been tested with following portal versions:

* DXP 7.0 CE GA7
* DXP 7.0 fixpack 50
* DXP 7.0 fixpack 60

## Installation Instructions

1. Download and deploy the JAR binaries 
1. Go to control panel App Manager
1. Find the standard Elasticsearch 2 module and deactivate it.
1. Add the standard adapter to bundle ("com.liferay.portal.search.elasticsearch") to blacklisted bundles. See instructions [here](https://dev.liferay.com/en/discover/portal/-/knowledge_base/7-0/blacklisting-osgi-modules).
1. Restart portal.
1. Check from logs or Gogo shell that they were installed correctly.
1. Do full reindex to update index settings and mappings.

If you enable keyword suggestions and have problems with them, try updating the adapter bundle from Gogo shell. This is a known issue in some scenarios, portal standard adapter not releasing the standard suggester reference.



 
