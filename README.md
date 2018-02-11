## geojson2ndjson

Converts a GeoJSON file on disk into a newline-delimited output, following the [ndjson](http://ndjson.org/) specification. So you can combine it with the [ndjson-cli](https://www.npmjs.com/package/ndjson-cli) tools, for instance.

### Usage

```
npm install geojson2ndjson
geojson2ndjson myfile.geojson | ...
```

### Examples

List the properties of every feature, without the geometries:

```
geojson2ndjson myfile.geojson | ndjson-map d.properties
```