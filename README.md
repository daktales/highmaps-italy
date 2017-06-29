Highmaps Italy
---
Vector maps for Italy at macro-area, region and province level.

![image](img/it-all.png?raw=true)

#### Resources:

* `it-all.sketch` : sketch file with multiple layers
* `it-admin1.svg` : svg file with admin1 division (regions)
* `it-admin2.svg` : svg file with admin2 division (provinces)
* `maps-data.xlsx` : excel file with all data used for javascript/highmap file
* `it-all.js` : javascript file compatible with Highmaps library

##### it-all.js
The internal structure of this file is the following:

```
var italy = {
    division: {
        1: "area",
        2: "regione",
        3: "provincia"
    },
    // Areas
    1: {
    	"type": "map",
        "data": [
        	{
        		"id": id,
        		"name": name,
        		"path": path
        	},
        	..
        ]
    },
    2: {
    	"type": "map",
        "data": [
        	{
        		"id": id,
        		"name": name,
        		"area_id": area id,
        		"area_name": area name
        		"path": path,
        	},
        	..
        ]
    },
    3: {
    	"type": "map",
        "data": [
        	{
        		"id": id,
        		"name": name,
        		"regione_id": region id,
        		"regione_name": region name,
        		"area_id": area id,
        		"area_name": area name
        		"path": path,
        	},
        	..
        ]
    },
}       
```

