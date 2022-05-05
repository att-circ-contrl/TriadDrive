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
* `obsolete` -- Devices and specifications that are no longer in service.
* `procedures` -- Assorted SOPs that apply to several different devices.
* `reference` -- Assorted reference material that isn't vendor documentation.
* `vendor-docs` -- Vendor-provided documentation and datasheets.
Under vendor copyright.


Sub-folders in `drive-XXX` and `aux-XXX`:

* `bom` -- List of vendor-supplied parts needed.
* `cad` -- Mechanical design CAD files. These are in FreeCAD format.
* `cad-ext` -- Mechanical design CAD or IGES files imported from a different
folder or provided by external sources (usually Isaac).
* `datasheets` -- Vendor-supplied mechanical drawings and component information.
* `drawings` -- Mechanical drawings of various components.
* `iges` -- Exported mechanical designs in IGES format.
* `meshes` -- Exported solid models in STL format.
* `notes` -- Assorted notes that are specific to this device.
* `photos` -- Photographs of the device or of associated equipment.
* `procedures` -- SOPs that are specific to this device.
* `renders` -- Screenshots of CAD views of various mechanical assemblies.


## Specific Designs

Active Triad drive variants are as follows:

* `drive-kevin` --
This is the initial Triad drive designed by Kevin for the Womelsdorf lab.
There were two variants: the "old" variant had a 45mm long channel for the
arms and the "new" variant had a 55mm long channel.

* `drive-close-short` -- This is a short-reach design with closely-spaced
probe sites. This drive is in service (with Kevin-style clips; the M0.5
screw-mount arms are obsolete). This can hold tungsten probes, NeuroNexus
probes, and Diagnostic BioChip probes (but not Atlas probes).

* `drive-close-long` -- This is a long-reach drive with closely-spaced
probe sites. This drive is in service. It is intended to hold Atlas probes
using the same "rectangular rod" scheme as the obsolete "v2b" drive.


Relevant auxiliary components are as follows:

* `aux-cabling` -- This folder contains documentation and models for
cables and connectors that the Triad drives and probes interface with.

* `aux-clips` -- This folder contains CAD models of clips used to hold
probes and guide tubes. Some are compatible with Kevin-style clip mounts,
while others are intended for different mounting methods.

* `aux-jig-atlas-long` -- This folder contains design files for tools for
loading Atlas probes into long-reach drives (drives that use the "rectangular
rod" system for holding probes).

* `aux-jig-nnex` -- This folder contains design files for the jig used to
pre-load NeuroNexus probes into guide tubes. The same jig works with
Diagnostic BioChip probes if the block holding the probe is shimmed with
tape to raise it.

* `aux-mounts-hflex` -- This folder contains cable mounts that replace the
mounting clip of the Triad drive. These old the "heavy flex" analog signal
cables used with Atlas and NeuroNexus probes.

* `aux-probes` -- This folder contains CAD models of probes and CAD models
of printable components for making mechanical mock-ups of probes.

* `aux-washers` -- This folder contains spacer "washers" used to raise the
Triad drives above their default mounting locations.


Drives not directly tied to the Triad Drive design:

* `drive-unidrive` -- This is a proof-of-concept single-probe drive based
on the same principles as the Triad drive but designed to be easier to
manufacture.


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

* IGES models should be saved as solids (type 186), rather than as surfaces
(type 144). Surfaces are the default, but solids can have additional
operations performed on them after import (especially boolean operations).


_This is the end of the file._
