Test latest tags of node-mapnik dependents that track latest node-mapnik

https://www.npmjs.com/browse/depended/mapnik

[![Build Status](https://travis-ci.org/mapbox/mapnik-swoop.svg?branch=master)](https://travis-ci.org/mapbox/mapnik-swoop)

### Details

The `.travis.yml` in this repo does a couple things:

 - Installs a bleeding edge or just released node-mapnik version
 - Ensures no duplicate node-mapnik versions are installed when installing all dependents. This is important because duplicate Node C++ modules in a tree can cause weird behavior or crashes.
 - Installs a bunch of modules that depend directly (or indirectly) on node-mapnik and then installs their `devDependencies` so that we can run their tests.

The goal here is to ensure the upcoming node-mapnik release does not accidentally break any dependents. And if it does then we want to find out right away rather than throw bug reports.

### Build status of each module

 This is here to provide a quick view of any modules who might have failing tests so that they can be excluded from `mapnik-swoop`. We're only concerned about modules that have 100% passing tests against the latest node-mapnik tag but which might have tests that fail against the upcoming node-mapnik tag.

 - node-mapnik - [![Build Status](https://secure.travis-ci.org/mapnik/node-mapnik.svg?branch=master)](http://travis-ci.org/mapnik/node-mapnik) | [![Dependencies](https://david-dm.org/mapnik/node-mapnik.svg)](https://david-dm.org/mapnik/node-mapnik)
  - mapnik-reference - [![Build Status](https://secure.travis-ci.org/mapnik/mapnik-reference.svg?branch=master)](http://travis-ci.org/mapnik/mapnik-reference) | [![Dependencies](https://david-dm.org/mapnik/mapnik-reference.svg)](https://david-dm.org/mapnik/mapnik-reference)
 - abaculus - [![Build Status](https://secure.travis-ci.org/mapbox/abaculus.svg?branch=master)](http://travis-ci.org/mapbox/abaculus) | [![Dependencies](https://david-dm.org/mapbox/abaculus.svg)](https://david-dm.org/mapbox/abaculus)
 - node-blend - [![Build Status](https://secure.travis-ci.org/mapbox/node-blend.svg?branch=master)](http://travis-ci.org/mapbox/node-blend) | [![Dependencies](https://david-dm.org/mapbox/node-blend.svg)](https://david-dm.org/mapbox/node-blend)
 - carmen - [![Build Status](https://secure.travis-ci.org/mapbox/carmen.svg?branch=master)](http://travis-ci.org/mapbox/carmen) | [![Dependencies](https://david-dm.org/mapbox/carmen.svg)](https://david-dm.org/mapbox/carmen)
 - tilelive-vector - [![Build Status](https://secure.travis-ci.org/mapbox/tilelive-vector.svg?branch=master)](http://travis-ci.org/mapbox/tilelive-vector) | [![Dependencies](https://david-dm.org/mapbox/tilelive-vector.svg)](https://david-dm.org/mapbox/tilelive-vector)
 - tilelive-bridge - [![Build Status](https://secure.travis-ci.org/mapbox/tilelive-bridge.svg?branch=master)](http://travis-ci.org/mapbox/tilelive-bridge) | [![Dependencies](https://david-dm.org/mapbox/tilelive-bridge.svg)](https://david-dm.org/mapbox/tilelive-bridge)
 - mapnik-omnivore - [![Build Status](https://secure.travis-ci.org/mapbox/mapnik-omnivore.svg?branch=master)](http://travis-ci.org/mapbox/mapnik-omnivore) | [![Dependencies](https://david-dm.org/mapbox/mapnik-omnivore.svg)](https://david-dm.org/mapbox/mapnik-omnivore)
 - tilelive-omnivore - [![Build Status](https://secure.travis-ci.org/mapbox/tilelive-omnivore.svg?branch=master)](http://travis-ci.org/mapbox/tilelive-omnivore) | [![Dependencies](https://david-dm.org/mapbox/tilelive-omnivore.svg)](https://david-dm.org/mapbox/tilelive-omnivore)
 - vector-tile-query - [![Build Status](https://secure.travis-ci.org/mapbox/vector-tile-query.svg?branch=master)](http://travis-ci.org/mapbox/vector-tile-query) | [![Dependencies](https://david-dm.org/mapbox/vector-tile-query.svg)](https://david-dm.org/mapbox/vector-tile-query)
 - tilelive-mapnik - [![Build Status](https://secure.travis-ci.org/mapbox/tilelive-mapnik.svg?branch=master)](http://travis-ci.org/mapbox/tilelive-mapnik) | [![Dependencies](https://david-dm.org/mapbox/tilelive-mapnik.svg)](https://david-dm.org/mapbox/tilelive-mapnik)
 - landspeed.js - [![Build Status](https://secure.travis-ci.org/mapbox/landspeed.js.svg?branch=master)](http://travis-ci.org/mapbox/landspeed.js) | [![Dependencies](https://david-dm.org/mapbox/landspeed.js.svg)](https://david-dm.org/mapbox/landspeed.js)
 - assert-http - [![Build Status](https://secure.travis-ci.org/mapbox/assert-http.svg?branch=master)](http://travis-ci.org/mapbox/assert-http) | [![Dependencies](https://david-dm.org/mapbox/assert-http.svg)](https://david-dm.org/mapbox/assert-http)
 - mapnik-pool - [![Build Status](https://secure.travis-ci.org/mapbox/mapnik-pool.svg?branch=master)](http://travis-ci.org/mapbox/mapnik-pool) | [![Dependencies](https://david-dm.org/mapbox/mapnik-pool.svg)](https://david-dm.org/mapbox/mapnik-pool)
 - geojson-mapnikify - [![Build Status](https://secure.travis-ci.org/mapbox/geojson-mapnikify.svg?branch=master)](http://travis-ci.org/mapbox/geojson-mapnikify) | [![Dependencies](https://david-dm.org/mapbox/geojson-mapnikify.svg)](https://david-dm.org/mapbox/geojson-mapnikify)
 - tilelive-overlay - [![Build Status](https://secure.travis-ci.org/mapbox/tilelive-overlay.svg?branch=master)](http://travis-ci.org/mapbox/tilelive-overlay) | [![Dependencies](https://david-dm.org/mapbox/tilelive-overlay.svg)](https://david-dm.org/mapbox/tilelive-overlay)
 - tilestrata-mapnik - [![Build Status](https://secure.travis-ci.org/naturalatlas/tilestrata-mapnik.svg?branch=master)](http://travis-ci.org/naturalatlas/tilestrata-mapnik) | [![Dependencies](https://david-dm.org/naturalatlas/tilestrata-mapnik.svg)](https://david-dm.org/naturalatlas/tilestrata-mapnik)
