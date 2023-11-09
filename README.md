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
It is stored in the file `paleomap-pixels-xxx.tab`,
in which `xxx` is used to indicate the resolution.

### Plate motion model

The plate motion model
(or rotation model)
was the PaleoMap model of Scotese (2016).

The model is stores in the file `paleomap-motion-xxx-5.tab`,
in which `xxx` is the pixel resolution,
and 5 is the time resolution (in million years).

### Paleolandscape

The landscape features are taken from Scotese and Wright (2018) paleoDEMs,
available at [EarthByte page](https://www.earthbyte.org/paleodem-resource-scotese-and-wright-2018/).
The digitalization uses the following convention
to make more or less compatible with the [EarthByte model](https://github.com/js-arias/gm-earthbyte):

Elevation      | Key | Environment
-------------- | --- | -----------
4000m or more  |   6 | collision mountains
1500 to 2000m  |   4 | highlands
0 to 1500m     |   3 | lowlands
-200 to 0m     |   2 | continental shelf
-2000 to -200m |   1 | oceanic plateaus

Note that this paleolandscape does not include glacial ice sheets.

The model is stored in the file `paleomap-landscape-xxx-5.tab`,
in which `xxx` is the pixel resolution
and 5 is the time resolution (in million years).

A color key,
which is compatible with color-blindness,
and can be used with `plates timepix map` command
is stored in the file `paleomap-landscape-key.tab`.

## Citation and data license

This model is the direct process of the Scotese (2016),
and Scotese and Wright (2018) models.
As such,
the original publications should be cited when the model is used.
Relevant papers are given in this file
and provided as bibTeX.

It is not required to cite this repository,
but if you do not include the model in the supplementary material
of your publication,
it might be a good idea to link this repository
and help others to replicate or re-use your analysis.

Data from PaleoMap project
(Scotese, 2016;
Scotese and Wrigth, 2018)
is distributed under the CC-BY 4.0 license,
that can be found in the LICENSE file.

## Disclaimer

As the models are a product of a pixelation of vectorial models,
it is possible that some pixels will not be defined
particularly in the boundaries of plates.
Depending on the usage given to the models,
this problems will be only annoying
(for example,
a deep ocean pixel in the middle of a continent),
or it can be critical
(if the feature of interest is near this absent pixels).
So be careful when using the models.

## References

Scotese, C.S.
(2016)
PALEOMAP PaleoAtlas for GPlates.
URL: <https://www.earthbyte.org/paleomap-paleoatlas-for-gplates/>.

Scotese, C.S., Wrigth, N.
(2018)
PALEOMAP Paleodigital elevation models (PaleoDEMs) for Phanerozoic.
URL: <https://www.earthbyte.org/paleodem-resource-scotese-and-wright-2018/>.
