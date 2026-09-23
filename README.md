# opendrop-presets-ansorre

An additional MilkDrop preset pack for [OpenDrop VJ](https://github.com/kushiemoon-dev/OpenDrop-VJ),
alongside the default [presets-cream-of-the-crop](https://github.com/projectM-visualizer/presets-cream-of-the-crop)
pack it already bundles.

## Source and conversion

These presets are converted from
[ansorre/tens-of-thousands-milkdrop-presets-for-butterchurn](https://github.com/ansorre/tens-of-thousands-milkdrop-presets-for-butterchurn),
which publishes ~15,000 MilkDrop presets pre-converted to JSON for [Butterchurn](https://github.com/jberg/butterchurn)
(a WebGL/JS MilkDrop-compatible renderer), not as `.milk` source files.

The files in this repo were regenerated from that JSON back into the `.milk` format
[libprojectM](https://github.com/projectM-visualizer/projectm) (and MilkDrop itself) reads, so the
conversion is lossy: equation syntax, variable and function names were mapped as faithfully as
possible, but a handful of JS/Butterchurn-only helper functions with no MilkDrop equivalent
(`atan2`, `round`, `log10`, `hypot`) were approximated rather than reproduced exactly.

Every preset here passed a load-and-render check against libprojectM 4.1.6 (OpenDrop VJ's pinned
version) before being included; presets that failed that check were dropped rather than shipped
broken.

## License

The upstream Ansorre repository carries no license. These are unofficial, community-made
derivatives of MilkDrop presets originally authored by many different preset artists over the
years (the file names are the original preset titles, generally `Author - Title.milk`); Ansorre's
own repository does not credit individual authors beyond what's embedded in those file names.

No license is asserted here either. This repo exists to make Butterchurn's Ansorre conversion
usable as `.milk` again, for the same non-commercial, community MilkDrop-preset-sharing use case
the original packs (MilkDrop, Butterchurn, Cream of the Crop) have always been distributed under.
If you are a preset author in this pack and want your work removed, open an issue.
