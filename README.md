FieldKit.otl
============

Collection of Houdini Digital Assets.


# Libraries

## SOP

### Create
_fd_sop_create.otl_

* Trail Boundary Object _creates a bounding box from an animated input_
* Scatter Uniform (+ Point Distributor)


### Modify
_fd_sop_modify.otl_

* Displace by LFO Noise
* Displace by Map _uses a COP or Texture to displace the geometry, similar to a displacement shader SHOP._
* Normalize _the geometry into a 0-1 size along a given dimension_


### Render
_fd_sop_render.otl_

* Color Random from Ramp
* Line Shaper


### Util
_fd_sop_util.otl_

* File Cache _is a versatile multi process file caching node that works with Alembic and BGEO formats_



# Installation

Open ```$HOME/houdiniX.Y/houdini.env``` in a text editor and append the following lines:
```Bash
FIELDKIT = "//ULTRA/3D/FieldKit.otl/"
HOUDINI_OTLSCAN_PATH = "$FIELDKIT;$HFS/houdini/otls"
```