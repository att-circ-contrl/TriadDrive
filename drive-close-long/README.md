# Close-Spaced Long-Reach Drive

## Overview

This folder contains a long-reach variant of the close-spaced short-reach
drive, intended for use with Diagnostic BioChip probes. This eliminates
mechanical conflicts between the probe and guide tube, allowing the full
range of drive travel to be used (so that the probes can reach as far as
possible into tissue).


For this variant, the drive "foot" is extended to incorporate a
downward-projecting shaft similar to that of the "forks" used in
"v2b"-derived drives. This results in geometry that is difficult to machine,
but 3d printed versions should work (the shaft is 3mm thick to ensure
sufficient strength and rigidity).

Guide tubes are in the same locations as with the close-spaced short-reach
drives, so the stock (narrow) body and short-reach drive's arms are used.


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

* As of June 2022, the "wide" variants of the arms work best in the drives.


_This is the end of the file._
