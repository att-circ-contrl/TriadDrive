# Stock ("Kevin") Triad Drive

## Overview

This folder documents the "stock" version of the Triad drive. These were
produced by Kevin Barker of Neuronitek on a contract for Thilo's lab.


## Notes

* Most parts were made by machining, but some parts were made by EDM by a
third-party vendor (I'm not sure who Kevin used for this).

* Kevin miniaturized the drives as much as possible (at Thilo's request).
Consequences of this include additional complexity, thin walls near several
holes, and the need for extremely close tolerances.

* Kevin got part fits with tolerances about twice as good as any other
vendor I'm aware of (about 0.05 mm as far as I can tell). He did this by
a combination fo careful setup and by hand-modifying individual sets of
mating parts.

The practical upshot of this is that any parts we get made for the Triad
drives will be a bit loose, due to the fact that we can't precisely match
the fit with the existing parts.

* The models in the "`iges`" folder should be considered authoritative.
These are my best guess as to the geometry of the actual parts. NOTE - These
were exported as surfaces rather than solids, so there may be issues
importing them.

* There are two types of meshes in the "`stl`" folder. Ones with the "`-sw`"
suffix have been modified to be compatible with Shapeways' 3d printing
design rules (mostly avoiding sharp concave edges and thin walls). Ones
without the "`-sw`" suffix were exported from the original models as-is.


## Variants

* The "old" variants have 45mm bodies made from black Delrin. The "new"
variants have 55mm bodies made from white Delrin. The "new" variants are
labelled "rev 3".

* The guide tube clip geometry is different for "old" and "new" variants.
The foot's mounting for the guide tube clip is also different.

* At least one variant exists that mounts five or six probes and guide
tubes (two per arm). If I understand correctly these were used for SPME
experiments.


_This is the end of the file._
