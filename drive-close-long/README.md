# Close-Spaced Long-Reach Drive

## Overview

This folder contains two different drive designs: A variant of the "v2b"
design intended for close-spaced Atlas probes, and a variant of the
close-spaced short-reach design intended for Diagnostic BioChip probes.


## Atlas Close-Spaced Long-Reach Drive

This is a modification of the "stock" Triad drive that shares many features
in common with the "v2b" Triad drive. The probes are mounted on rectangular
"rods" that are in turn moved by modified arms. A guide block keeps the "rods"
in alignment. A "fork" extends down into the chamber, and guide tubes are
mounted to the fork.

The body and rods are identical to the "v2b" version. The guide block, arms,
and fork are new.

This design is intended to work with Atlas probes.

A variant of this drive uses clip-based arms instead of rods, omitting the
rods and upper guide block. This is intended to work with tungsten probes
using the same hole pattern as Atlas probes, and to work with Diagnostic
BioChip probes using the (wider) Atlas hole pattern.


## Diagnostic Bio-Chip Close-Spaced Long-Reach Drive

This is a modification of the close-spaced short-reach drive. The "foot"
is extended to incorporate a downward-projecting shaft similar to that of
the "forks" used in "v2b"-derived drives. This results in geometry that is
difficult to machine, but 3d printed versions should work (the shaft is 3mm
thick to ensure sufficient strength and rigidity).

This version of the drive puts guide tubes in the same locations as the
close-spaced short-reach drives, so the stock (narrow) body and short-reach
drive's arms are used.


## Atlas Notes

* The Atlas probe cables have to bend around backwards to reach the cable
mount. This is because the original Atlas use-case had heavy flex and the
drive on opposite sides of the chamber, whereas the Triad drives have
heavy flex mounted on the drives.

* Mounting the Atlas probes is non-trivial, because they break if you look
at them funny and the thin-flex connected to them isn't much stronger.

* **FIXME** - As of 18 May 2022, the Atlas silicon arms have wide clearances.
This results in wobble. The Atlas tungsten arms have tighter clearances; this
should be back-ported to the silicon arms if the tight-clearance arms work.


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


_This is the end of the file._
