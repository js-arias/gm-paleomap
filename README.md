# PaleoMap model

This model is imported from the GPlates version
of the *PaleoMap* model
that can be downloaded from the [EarthByte page](https://www.earthbyte.org/paleomap-paleoatlas-for-gplates/).

## Time frame

The rotations are defined from 540 million years ago
(up to 600 for the plate motion model)
to today,
in time stages of 5 million years.

## Pixelation

The model is available in three resolutions:
e360 (360 pixels in the equatorial ring),
e180,
and e120.

## File descriptions

All the files are prefixed as `paleomap-*`
usually followed by the pixelation resolution,
the size of the time step,
and the kind of file.

### Pixelated features

It is based on the plate polygons
from the PaleoMap model.
It is stored in the file `paleomap-pixels-xxx.tab`
in which `xxx` is used to indicate the resolution.

### Plate motion model

The plate motion model
(or rotation model)
was the PaleoMap model of Scotese (2016).

The model is stores in the file `paleomap-motion-xxx-5.tab`,
in which `xxx` is the pixel resolution,
and 5 is the time resolution (in million years).

## References

Scotese, C.S.
(2016)
PALEOMAP PaleoAtlas for GPlates.
URL:<https://www.earthbyte.org/paleomap-paleoatlas-for-gplates/>.
