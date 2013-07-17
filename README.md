GeoReport v2 API servers
=====================

A relationship between cities and their service discovery urls.

More info:
 + [Open311](http://open311.org/)
 + [Open311 GeoReport v2 API](http://wiki.open311.org/GeoReport_v2)
 + [Open311 GeoReport v2 API servers](http://wiki.open311.org/GeoReport_v2/Servers)

Usage
-----------------

### Git submodule

Use [git submodule](http://git-scm.com/book/en/Git-Tools-Submodules) if you want to add this repository to your project. It could be useful if you want your project to have the latest information about the cities which are using the [GeoReport v2 API](http://wiki.open311.org/GeoReport_v2). 

 + `git submodule add https://github.com/SantiMunin/GeoReportv2-endpoints.git servers`
 + Load the file servers/cities.json in your library at build/run time.

### Network call

 + Download the [file](https://raw.github.com/SantiMunin/GeoReportv2-endpoints/master/cities.json): `wget https://raw.github.com/SantiMunin/GeoReportv2-endpoints/master/cities.json`
 + Load the file servers/cities.json in your library at build/run time.

Collaborate
-----------------

If you miss anything or notice any error, please open an issue.
