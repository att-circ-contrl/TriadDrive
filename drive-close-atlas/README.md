# Close-Spaced Drive for Atlas Probes

## Overview

This folder contains a variant of the long-reach "v2b" drive that has
close-spaced sites. This drive is intended for use with flanged Atlas probes.

The probes are mounted on rectangular "rods" that are in turn moved by
modified arms. A guide block keeps the "rods" in alignment. A "fork" extends
down into the chamber, and guide tubes are mounted to the fork. The body and
rods are identical to the "v2b" version. The guide block, arms, and fork are
new.

**NOTE** - The "Atlas" drive uses the "Atlas" sites in the site diagram
(2.0mm spacing), which differs from the more closely spaced sites used with
DBC and NeuroNexus probes (1.0mm/1.5mm spacing). Distance from the mounting
post also differs.

A variant of this drive uses clip-based arms instead of rods, omitting the
rods and upper guide block. This is intended to work with tungsten probes
using the same guide tube pattern as Atlas probes.


## Atlas Notes

* The Atlas probe cables have to bend around backwards to reach the cable
mount. This is because the original Atlas use-case had heavy flex and the
drive on opposite sides of the chamber, whereas the Triad drives have
heavy flex mounted on the drives.

* Mounting the Atlas probes is non-trivial, because they break if you look
at them funny and the thin-flex connected to them isn't much stronger.

* With a plastic foot, *the side guide tube mounts deflect*, pinching off
the middle channel and moving each guide tube inwards by about 0.4mm. The
probe mounts have enough compliance to tolerate this, but it's very much
not an ideal situation.


## Clearance and 3D Printing Notes

* Arms need to be made with tolerances better than standard shop and
printing tolerances. Otherwise the clearances needed for reliable assembly
are large enough that the arms wobble. We can't actually get arms made
with the required precision, so instead several versions of the arms are
made with nominal thicknesses varying in steps of 0.05 mm. In any given
batch, one version of any given arm should be the right thickness.

* Arms with tight clearances should be oriented with their long axes in the
Z direction for 3d printing. This gives 0.05 mm tolerances on the other axes
when using Proto Labs' "micro-resolution" printing process.

* As of June 2022, the "thick" variants of the arms work best in the drives.


_This is the end of the file._
