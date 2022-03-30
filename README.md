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


## Specific Designs

The lineage of Triad drive variants is as follows:

* `drive-kevin` -- This is the initial Triad drive designed by Kevin for
the Womelsdorf lab. There were two variants: the "old" variant had a 45mm
long channel and the "new" variant had a 55mm long channel.

* `drive-v2b` -- This is a long-reach drive design intended for widely-spaced
Atlas probes. This design is obsolete but the "body" part and "rod" parts
are used by subsequent designs.

* `drive-v2c` -- This is a short-reach design originally intended to mount
Atlas probes in a widely-spaced pattern. This design is obsolete.

* `drive-close-short` -- This is a short-reach design with closely-spaced
probe sites. This drive is in service (with Kevin-style clips; the M0.5
screw-mount arms are obsolete). This can hold tungsten probes, NeuroNexus
probes, and Diagnostic BioChip probes (but not Atlas probes).

* `drive-close-long` -- This is a long-reach drive with closely-spaced
probe sites. This drive is in service. It is intended to hold Atlas probes
using the same "rod" scheme as the "v2b" drive.


Relevant auxiliary components are as follows:

* `aux-probes` -- This folder contains CAD models of probes and CAD models
of printable components for making mechanical mock-ups of probes.

* `aux-clips` -- This folder contains CAD models of clips used to hold
probes and guide tubes. Some are compatible with Kevin-style clip mounts,
while others are intended for different mounting methods.

* `aux-hflex-mounts` -- This folder contains cable mounts that replace the
mounting clip of the Triad drive, and that hold up to three "heavy flex"
analog signal cables. The "wide" variant mates with the wider body used by
the "v2b" drive, and the "narrow" variant mates with stock drive bodies.

* `aux-dbc-mounts` -- This folder contains cable mounts that replace the
mounting clip of a narrow-body (stock) Triad drive, and that hold up to
three Diagnostic BioChip probe boards with room for ZIF clips to attach.


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
