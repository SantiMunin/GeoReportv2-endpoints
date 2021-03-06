GeoReport v2 API servers
=====================

A relationship between cities and their [service discovery](http://wiki.open311.org/Service_Discovery) urls.

More info:
 + [Open311](http://open311.org/)
 + [Open311 GeoReport v2 API](http://wiki.open311.org/GeoReport_v2)
 + [Open311 GeoReport v2 API servers](http://wiki.open311.org/GeoReport_v2/Servers)

## Usage

### Build time

 + [Git submodule](README.md#git-submodule)
 + [Network call](README.md#network-call)

### Run time
 + [Network call](README.md#network-call)

## Explanation

### Git submodule

Use [git submodule](http://git-scm.com/book/en/Git-Tools-Submodules) if you want to add this repository to your project. It could be useful if you want your project to have the latest information about the cities which are using the [GeoReport v2 API](http://wiki.open311.org/GeoReport_v2).

 + `git submodule add https://github.com/SantiMunin/GeoReportv2-endpoints.git servers`
 + Load the file `servers/cities.json` in your library at build time.

### Network call

Git submodule could not fit for you (maybe you are not using git), in that case this option is fine. 

Download the [file](https://raw.github.com/SantiMunin/GeoReportv2-endpoints/master/cities.json): `wget https://raw.github.com/SantiMunin/GeoReportv2-endpoints/master/cities.json` and load it at build/run time.

### File content

The `cities.json` file contains a json array of objects with three fields:

```js
[
 {
    "id" : "SAN_FRANCISCO",
    "city" : "San Francisco, CA",
    "service_discovery" : "https://open311.sfgov.org/dev/v2/discovery.xml",
    "jurisdiction_id" : "sfgov.org"
  },
  ...
]
```
####Fields
 + `id`: City's unique identifier.
 + `city`: City's name.
 + `service_discovery`: Url of the [service discovery](http://wiki.open311.org/Service_Discovery) file.
 + `jurisdiction_id`: [jurisdiction_id](http://wiki.open311.org/GeoReport_v2#jurisdiction_id) parameter.

Collaborate
-----------------

If you miss anything or notice any error, please open an issue.
