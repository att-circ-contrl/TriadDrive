# Clips for Probes and Guide Tubes

## Overview

This folder contains drawings and models for some of the clips used to hold
probes and to hold guide tubes with the Triad drives.

This is not a complete list, but should cover the types that are presently
in service. Historically two other attachment methods were also used (using
screws and flanges to mount individual probes and guide tubes, and using
a larger clamp to hold multiple guide tubes at once), but clips were the
most practical system.

The guiding principles are as follows:

* It should be possible to remove individual probes and guide tubes without
disturbing the others.

* It should be possible to position probe sites close to each other (2mm or
closer).

* Nobody should have to reinstall M1 screws or do anything with M0.5
screws in order to add or remove probes or guide tubes. #0 screws are
preferred over M1 where practical.

Several fabrication methods are available:

* 3D printing was used for large clamps and is still used for the assemblies
that clips screw on to. Printed plastic parts are too weak to use for the
clips themselves and printed metal parts have resolution too poor to use,
with rare exceptions.

* CNC machining is used where practical, but has strong constraints on
geometry (in particular thickness).

* EDM is used for making thin clips with high precision out of stainless
steel, but finding vendors for this is a pain and turnaround time is long.


## Specific Clips

* The "Kevin" clips were made by EDM and were intended to hold 200 micron
tungsten probes. In practice they'll hold 125 micron probes that are
shimmed with tape, and they've been used to hold 400 micron NeuroNexus
probes (although this will eventually cause metal fatigue). These use M1
screws for mounting and for closing.

* The "6p5" straight clips are made out of CNC machined PEEK. These use #0
screws for mounting and closing and are somewhat bulkier than Kevin clips.

* The "j-clip" clips are made from 3d printed resin (Proto Labs' "ABS-like
micro-resolution" process). These are used as guide tube clamps with
certain close-spaced probe layouts. The geometry and tolerances made 3d
printing the only option. So far they've held up in use.

* The "compat-630" EDM clips are very similar to the Kevin clips and are
intended to hold 630 micron guide tubes and probe collars.

* The "cnc-630" clips were intended to hold 630 micron guide tubes and
probe collars and to be made using Proto Labs' CNC service.
**Obsolete** - They ended up being too bulky and Proto Labs wouldn't
machine the probe registration notches.

* The "3dp-630" clips were intended to hold 630 micron guide tubes and
probe collars and to be made using Proto Labs' stainless steel 3d printing
service. **NOTE** - These are very difficult to hand-tap.


_This is the end of the file._
