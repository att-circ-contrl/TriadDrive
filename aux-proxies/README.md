# Mechanical Proxies

## Overview

This folder contains models of mechanical proxies of each of the drive
variants in service. These are used for planning the configuration of the
drives; proxies are mounted on a mockup chamber and adjusted to have guide
tubes in the desired locations.

(The original proxy for the stock tungsten drives was made by Brainsight
in the 2010s, I think. The new proxies are intended to be 3d printed.)

The proxies have optional obstruction templates that may be attached. Without
the templates, the goal is to show where the guide tubes will be positioned
with maximum visibility. With the templates, the goal is to see whether nearby
drives will conflict with each other.


## Specific Models

Drive proxies (representing the drive bodies and guide tubes):

* `drive-close-long` -- This represents the "close-spaced long-reach"
drive with guide tube mounts inside the chamber, using the 2.0/2.0/1.5 mm
hole pattern.

* `drive-close-short` -- This represents the "close-spaced short-reach"
drive with guide tube mounts at the chamber lip, using the 1.0/1.5/1.5 mm
hole pattern.

* `drive-stock` -- This represents the stock "kevin" drive with a bundle
of three guide tubes in contact with each other.


Cable mount proxies (representing mounts for either the "heavy flex"
cables or the Diagnostic BioChip adapter boards):

* `dbc-zif-narrow` -- This represents a Diagnostic BioChip board mount plus
attached ZIF-clips, intended for narrow-body (stock) drives.

* `dbc-zif-wide` -- This represents a Diagnostic BioChip board mount plus
attached ZIF-clips, intended for wide-body (long-reach) drives.

* `hflex-narrow` -- This represents a "heavy flex" mount intended for
narrow-body (stock) drives.

* `hflex-wide` -- This represents a "heavy flex" mount intended for
wide-body (long-reach) drives.


Obstruction templates (representing space taken up by drive arms and by
guide tube mounts):

* `close-short-1pc` -- This represents a low-profile foot for the
"close-spaced short-reach" drive that uses a single clip to hold all three
guide tubes.

* `close-short-2lv` -- This represents a standard (two-level) foot for the
"close-spaced short-reach" drive that uses one clip for each guide tube.

* `close-short-3pc` -- This represents a low-profile foot for the
"close-spaced short-reach" drive that uses one clip for each guide tube.


_This is the end of the file._
