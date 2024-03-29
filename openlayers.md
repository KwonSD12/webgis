# OpenLayers

[OpenLayers](https://openlayers.org/) is a high-performance, feature-packed library for creating interactive maps on the web. It can display map tiles, vector data and markers loaded from any source on any web page. OpenLayers has been developed to further the use of geographic information of all kinds. It is completely free, Open Source JavaScript, released under the [BSD 2-Clause License](https://opensource.org/licenses/BSD-2-Clause).

## Getting Started

Install the [`ol` package](https://www.npmjs.com/package/ol):

```
npm install ol
```

Import just what you need for your application:

```js
import Map from 'ol/Map';
import View from 'ol/View';
import TileLayer from 'ol/layer/Tile';
import XYZ from 'ol/source/XYZ';

new Map({
  target: 'map',
  layers: [
    new TileLayer({
      source: new XYZ({
        url: 'https://{a-c}.tile.openstreetmap.org/{z}/{x}/{y}.png'
      })
    })
  ],
  view: new View({
    center: [0, 0],
    zoom: 2
  })
});
```

See the following examples for more detail on bundling OpenLayers with your application:

 * Using [Vite](https://github.com/openlayers/ol-vite)
 * Using [Rollup](https://github.com/openlayers/ol-rollup)
 * Using [webpack](https://github.com/openlayers/ol-webpack)
 * Using [Parcel](https://github.com/openlayers/ol-parcel)

## Sponsors

OpenLayers appreciates contributions of all kinds.  We especially want to thank our fiscal sponsors who contribute to ongoing project maintenance.

<br>

<br>


[![GeoSolutions logo](./sponsor-logos/geosolutions.png)](https://www.geosolutionsgroup.com/)

> Your one-stop-shop for geospatial open source software.
> https://www.geosolutionsgroup.com/

<br>

[![ela-compil logo](./sponsor-logos/ela-compil.png)](https://ela.pl/)

> We develop leading Physical Security Information Management (PSIM) software.
> OpenLayers is the core of our map engine and we love it! 
> https://elacompil.recruitee.com/

<br>

See our [GitHub sponsors page](https://github.com/sponsors/openlayers) or [Open Collective](https://opencollective.com/openlayers/contribute/sponsors-214/checkout) if you too are interested in becoming a regular sponsor.

