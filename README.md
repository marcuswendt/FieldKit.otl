FieldKit.otl
============

Collection of Houdini Digital Assets.

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

1. Clone the repository onto a local or network drive e.g. //ULTRA/3D/FieldKit.otl/

2. Open ```$HOME/houdiniX.Y/houdini.env``` in a text editor and append the following lines:
```Bash
FIELDKIT = "<PATH TO YOUR GIT CLONE HERE>"
HOUDINI_OTLSCAN_PATH = "$FIELDKIT;$HFS/houdini/otls"
```

3. Relaunch Houdini and it should have picked up the assets. Use Windows> Operator Type Manager> Scanned OTL Libraries to check.