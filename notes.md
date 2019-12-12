

## Tutorial:

[Commandline Cartography](https://medium.com/@mbostock/command-line-cartography-part-1-897aa8f8ca2c)


A quick way to check what’s in a shapefile is to visit mapshaper.org and drag the shapefile into your browser.

[Mapshaper](https://mapshaper.org/)


As Mapshaper demonstrates, it’s possible to view shapefiles directly in your browser. But binary shapefiles can be difficult to work with, so we’ll convert to GeoJSON: a web-friendly, human-readable format. My shapefile parser has a command-line interface, shp2json, for this purpose. (Warning: there’s an unrelated package of the same name on npm.)

[Shapefile Paraser](https://github.com/mbostock/shapefile)



https://github.com/mbostock/shapefile/blob/master/README.md#shp2json




curl 'http://api.census.gov/data/2014/acs5?get=B01003_001E&for=tract:*&in=state:06' -o cb_2014_06_tract_B01003.json
curl 'http://api.census.gov/data/2014/acs/acs5?get=B01003_001E&for=tract:*&in=state:06' -o cb_2014_06_tract_B01003.json

curl 'http://api.census.gov/data/2014/acs/acs5/profile?get=B01003_001E&for=state:06' -o asdf.json

http://api.census.gov/data/2014/acs/acs5?



from Matt Z:

- copy files from shared folder to local folder for development

cp {MAPC_floodrisk.cpg, MAPC_floodrisk.dbf, MAPC_floodrisk.prj, MAPC_floodrisk.sbn, MAPC_floodrisk.sbx, MAPC_floodrsik.shp} .

- install shapefile javascript package commnad line tool

yarn global add shapefile

- convert to GeoJSON with properties

shp2json MAPC_floodrisk.shp > MAPC_floodrisk.json
