# mapapps-reveal-js

This project converts the [reveal.js](https://github.com/hakimel/reveal.js) bower version to a map.apps friendly jar.

The jar is called `mapapps-reveal-js.jar` and it contains the bundle `reveal-js`.

## Changes of the bower version

* css is compressed
* js is compressed
* plugins/markdown/markdown.js is patched to configure accept header in request

## Installation

Upload the jar `mapapps-reveal-js.jar` to your map.apps installation.

Note the provided `reveal-js` bundle provides only the reveal.js API.

It is required by the [mappapps-map-slides](https://github.com/conterra/mappapps-map-slides) project.

## Upgrade Instructions

1.  update the version in bower.json

1.  check .bowerrc and exclude all other dependencies

1.  check the pom.xml for package.json manipulation

1.  update the version of the pom.xml

1.  execute mvn for testing output

    `mvn clean package`

1.  check the markdown patch

1.  release via jenkins