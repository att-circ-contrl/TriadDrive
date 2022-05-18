# Close-Spaced Long-Reach Drive

## Overview

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
BioChip probes using the Atlas hole pattern.


## Notes

* The Atlas probe cables have to bend around backwards to reach the cable
mount. This is because the original Atlas use-case had heavy flex and the
drive on opposite sides of the chamber, whereas the Triad drives have
heavy flex mounted on the drives.

* Mounting the Atlas probes is non-trivial, because they break if you look
at them funny and the thin-flex connected to them isn't much stronger.

* Arms with tight clearances should be oriented with their long axes in the
Z direction for 3d printing. This gives 0.05 mm tolerances on the other axes.

* **FIXME** - As of 18 May 2022, the Atlas silicon arms have wide clearances.
This results in wobble. The Atlas tungsten arms have tighter clearances; this
should be back-ported to the silicon arms if the tight-clearance arms work.


_This is the end of the file._
