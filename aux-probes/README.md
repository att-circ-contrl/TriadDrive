# Probe Models

## Overview

This folder contains drawings and models for the probes used with the
Triad drives.

This is not a complete specification; that's beyond the scope of this
project. The intent is to provide enough information to allow the design of
drives that are mechanically compatible with the probes.


## Specific Probes

* Atlas probes were ordered in 2017.

These were originally intended to be used with a dense-packed semi-chronic
drive, which secured the probes and guide tubes to the drive with flanges
and tiny screws. With the Triad drive we can use different guide tubes and
clamp them normally, but the probes will have to be secured with screws (the
flanges are permanently bonded and the probe shanks are too fragile to
reliably grab).

The Atlas probes have "thin flex" ribbons that connect to our "heavy flex"
cables. The Atlas probes are permanently bonded to the heavy flex.


* NeuroNexus probes were ordered in 2018 and 2021.

They were ordered with flanges for compatibility with the Atlas drive
hardware, but in practice are secured using clips. The shanks are stainless
steel tubes, making them much easier to secure and to handle.

The NeuroNexus probes have hair-thin flex cables which are bonded to tabs
that connect to our "heavy flex" cables. These may be connected and
disconnected from the heavy flex as-desired.


* Diagnostic BioChip probes were ordered in 2022.

These do not have flanges, but instead have a 5mm collar of hypodermic
tubing for handling.

The DBC probes do not connect to "heavy flex". Instead, they have their own
ZIF-clip compatible adapter cards, which are connected to the probes using
a short length of delicate thin flex. The adapter cards need to be mounted
close to the probes and the ZIF-clips need to connect directly to the adapter
cards.


## CAD File Notes

* The presently active CAD file is "`probe-models-2022.fcstd`".

* The 2020 CAD file contains old models for NeuroNexus probes. The "sleeve"
version was an alternate implementation that wasn't made; it can be ignored.
The file has copies of the old Atlas models, but these were reconstructed
from meshes instead of from the original solid models.


_This is the end of the file._
