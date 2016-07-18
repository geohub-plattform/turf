# @turf/center-of-mass

# center-of-mass

Takes a [feature](http://geojson.org/geojson-spec.html#feature-objects)
or a [featureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects)
and returns its [center of mass](https://en.wikipedia.org/wiki/Center_of_mass)
using this formula: [Centroid of Polygon](https://en.wikipedia.org/wiki/Centroid#Centroid_of_polygon).

**Parameters**

-   `feature` **[Feature](http://geojson.org/geojson-spec.html#feature-objects)** the feature

**Examples**

```javascript
var feature = {
  "type": "Feature",
  "properties": {},
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          4.854240417480469,
          45.77258200374433
        ],
        [
          4.8445844650268555,
          45.777431068484894
        ],
        [
          4.845442771911621,
          45.778658234059755
        ],
        [
          4.845914840698242,
          45.779376562352425
        ],
        [
          4.846644401550292,
          45.78021460033108
        ],
        [
          4.847245216369629,
          45.78078326178593
        ],
        [
          4.848060607910156,
          45.78138184652523
        ],
        [
          4.8487043380737305,
          45.78186070968964
        ],
        [
          4.849562644958495,
          45.78248921135124
        ],
        [
          4.850893020629883,
          45.78302792142197
        ],
        [
          4.852008819580077,
          45.78374619341895
        ],
        [
          4.852995872497559,
          45.784075398324866
        ],
        [
          4.853854179382324,
          45.78443452873236
        ],
        [
          4.8549699783325195,
          45.78470387501975
        ],
        [
          4.85569953918457,
          45.784793656826345
        ],
        [
          4.857330322265624,
          45.784853511283764
        ],
        [
          4.858231544494629,
          45.78494329284938
        ],
        [
          4.859304428100585,
          45.784883438488365
        ],
        [
          4.858360290527344,
          45.77294120818474
        ],
        [
          4.854240417480469,
          45.77258200374433
        ]
      ]
    ]
  }
};

var centerOfMass = turf.center-of-mass(feature);

//=centerOfMass
```

Returns **[Feature](http://geojson.org/geojson-spec.html#feature-objects)&lt;[Point](http://geojson.org/geojson-spec.html#point)>** the center of mass

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/center-of-mass
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```