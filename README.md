
Submarine Cable Map
===================

[TeleGeography's](https://www.telegeography.com) submarine cable map is based on our authoritative [Global Bandwidth](https://www.telegeography.com/research-services/global-bandwidth-research-service/) research. The map depicts active and planned submarine cable systems, their landing stations, cable length, ready for service (RFS) date, owners, and website.

Installation
------------

Install a LTS version of [Node.js](https://nodejs.org/), [Yarn](https://yarnpkg.com/) for package management, and finally [Ember](https://www.emberjs.com/).

    $ git clone git://github.com/satriyoaji/project-gis-submarinecable
    $ cd project-gis-submarinecable
    $ yarn install
    $ yarn start

How did we make this Submarine Cable Map?
-------------------------------

[TeleGeography](http://www.telegeography.com) draws the cable routes and plots the landing points with [Adobe Illustrator](https://www.adobe.com/products/illustrator.html). Using [Avenza's MAPublisher](https://www.avenza.com/mapublisher) plug-in, which works with Illustrator, two sets of data are exported as KML files: the cable routes (as MultiLineStrings) and landing points (as Points). These KML files are then parsed to create CSV files that are transformed to GeoJSON.

This interactive map Javascript was created using the [Ember](https://emberjs.com/) web application framework using [emberCLI](https://ember-cli.com/).  The Javascript for the map was written in-house at TeleGeography.
