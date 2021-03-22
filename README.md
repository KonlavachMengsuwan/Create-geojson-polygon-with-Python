# Create-geojson-polygon-with-Python

## 1. Install geojson package
```
conda install python=3 geojson
```

## 2. Load Polygon library
```
from geojson import Polygon
```

## 3. Polygon coordinates
```
map_aoi = Polygon([[(100.287, 15.091), (100.489, 15.091), (100.489, 15.225), (100.287, 15.225)]])  # doctest: +ELLIPSIS
```

## 4. Load dump to export
```
from geojson import dump
```

## 5. Exprot as .geojson file
```
with open('map_aoi.geojson', 'w', encoding='utf-8') as f:
    dump(map_aoi, f)
```

### Source
```
https://pypi.org/project/geojson/
```
