An attempt to use bleve as a backend for bookmark index, using [bleve-explorer](https://github.com/blevesearch/bleve-explorer) as a starting point and query UI.

## Building

    go-bindata-assetfs static/...    
    go build

Rebuilding assets with [go-bindata-assetfs](https://github.com/elazarl/go-bindata-assetfs).

## Running

    mkdir data
    ./bleve-explorer

This will use the default "data" dir for storing indexes.
Once started you can access the web UI at http://localhost:8095/

## Prepare json file to load 



## Script to load json

[bleve bulk](http://www.blevesearch.com/docs/bleve_bulk/)

    #!/bin/bash
    curl -X PUT http://localhost:8095/api/diigo_json/$JsonFile -d @$JsonFile


## Screenshots

field url as clickable link

![](docs/index.png)
