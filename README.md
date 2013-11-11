GeoJSON_Files
=============

This is just a simple test on the 'new' mapping functionality of GitHub, described in the [help](https://help.github.com/articles/mapping-geojson-files-on-github) and the [blog](https://github.com/blog/1541-geojson-rendering-improvements)

These are the testfiles:

* spec_data.geojson ... contains all geometries of the [GeoJSON specification](http://www.geojson.org/geojson-spec.html)

* spec_data.topojson ... same data as above, but as a topojson-file
--> the corresponding command: *topojson -p -o spec_data.topojson spec_data.geojson*

* individual_markers.geojson ... testing all the individual marker-style-definitions, that are possible (described in the [help](https://help.github.com/articles/mapping-geojson-files-on-github))

* lines.json ... contains 3 different linestrings with different semantics:
	- street
	- river
	- navigation_route

* featCollTest.json ... contains the 3 linestrings taken from 'lines.json', but here they are stored as a single FeatureClass within the major FeatureClass

* featCollTest2.json ... based on 'featCollTest.json', without the major (surrounding) FeatureClass ... this is just to test if that syntax works

* geojsonarray.json & geojsonarray2.json... same test as in the previous two, but with more simple contents
	- geojsonarray.json --> no major FeatureClass
	- geojsonarray2.json --> with a major FeatureClass

*Just click them and you will see the corresponding data on a map!*
