# Womelsdorf Lab Probe Drives

## Overview

This project covers the design of the probe drives used by the Womelsdorf
lab. As of 2022, these are mostly derivatives of the "Triad drive" 3-probe
drive commissioned in **FIXME - year** from Kevin Barker of Neuronitek.

The original "Triad" drive has three BNM07-1207 Namiki motors, each with a
105x reduction gear (SPG07-105). These drive #0-80 threaded rods, which move
probe-holding "arms" along paths defined by the outer shell of the drive
(the "body") and an internal "girder" with precisely-machined channels.

Derivative variants of the "Triad" drive replace the arms, the outer shell
of the drive, and the foot of the drive, but keep the basic architecture the
same and do not modify the motor section.

Alternate drive designs that are not direct derivatives of the "Triad" drive
are noted where present.

## Folders

Top-level folders:

* `aux-XXX` -- CAD files and notes specific to a given auxiliary tool.
* `drive-XXX` -- CAD files and notes specific to a given drive variant.
* `notes` -- Assorted notes that apply to several different devices.
* `procedures` -- Assorted SOPs that apply to several different devices.
* `vendor-docs` -- Vendor-provided documentation and datasheets.
Under vendor copyright.


Sub-folders in `drive-XXX` and `aux-XXX`:

* `cad` -- Mechanical design CAD files. These are in FreeCAD format.
* `cad-ext` -- Mechanical design CAD or IGES files imported from a different
folder or provided by external sources (usually Isaac).
* `drawings` -- Mechanical drawings of various components.
* `iges` -- Exported mechanical designs in IGES format.
* `meshes` -- Exported solid models in STL format.
* `notes` -- Assorted notes that are specific to this device.
* `photos` -- Photographs of the device or of associated equipment.
* `procedures` -- SOPs that are specific to this device.
* `renders` -- Screenshots of CAD views of various mechanical assemblies.


## Remarks

* I've been repeatedly reassured that the Womelsdorf Lab owns all of the IP
for the original drives that we commissioned, so there should be no IP issues
with derived variants.

* Kevin is a superb engineer. Every aspect of his original design is there
for a reason, and the reasons are not always obvious. Kevin also gets
precision about twice as good as standard "shop" precision (better than
0.1mm, vs typical shop precision of 0.15 mm or worse). The downside to this
is that understanding the original design was nontrivial and third-party
parts typically have wobble due to worse tolerances.

* I have a love/hate relationship with the `FreeCAD` program. It works
_just_ well enough that it isn't worth my time to learn a new program, but
it has strange ideas about how many operations should be done and it
lacks several features that would be helpful for building and testing
models. If you need to modify existing mechanical models, I suggest
importing `.iges` models into your preferred CAD program.


_This is the end of the file._
