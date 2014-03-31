```
      _____    __    _____    __       ____
     / ___/   / /   /____/   / /      /    \    FieldKit.otl
    / ___/   / /   /____/   / /__    /  /  /    (c) 2014, FIELD. All rights reserved.
   /_/      /_/   /____/   /____/   /_____/     http://www.field.io

```

A collection of Digital Assets for SideFX's Houdini animation and visual effects software.
This library combines frequently used tools and ideas derived from the generative design field as small modular assets.



Included Tools:

## SOP

### Create _fd_sop_create.otl_

* Trail Boundary Object _creates a bounding box from an animated input_
* Scatter Uniform (+ Point Distributor)
* Helix _creates a polygon helix spiral_

### Modify _fd_sop_modify.otl_

* Displace by LFO Noise
* Displace by Map _uses a COP or Texture to displace the geometry, similar to a displacement shader SHOP._
* Normalize _the geometry into a 0-1 size along a given dimension_


### Render _fd_sop_render.otl_

* Color Random from Ramp
* Line Shaper


### Util _fd_sop_util_

* File Cache _is a versatile multi process file caching node that works with Alembic and BGEO formats_


## ROP

### Util _fd_rop_util_

* Game Asset Exporter _simplifies exporting a variety of file formats for use in realtime 3D engines_



# Installation

1. [Download](//github.com/field/FieldKit.otl/archive/master.zip) or clone the repository onto a local or network drive e.g. //ULTRA/3D/FieldKit.otl/

2. Open ```houdini.env``` (Windows: ```$HOME/houdiniX.Y/houdini.env``` OS X: ```~/Library/Preferences/houdini/```) in a text editor and append the following lines:
```Bash
FIELDKIT = "<PATH TO YOUR GIT CLONE HERE>"
HOUDINI_OTLSCAN_PATH = "$FIELDKIT;$HFS/houdini/otls"
```

3. Relaunch Houdini and it should have picked up the assets. Use Windows> Operator Type Manager> Scanned OTL Libraries to check.


## TODO

### Better Caching

- rendering a series of dependent caches in the background
- unlock all parent HDAs from cache node. e.g. when cache is embedded into another HDA.


Credits
=======

Released under the BSD license.  Full details in the included LICENSE file.

(c) 2013-2014, Marcus Wendt <marcus@field.io>
