# Ethos Suite Assets

Runtime-ready image assets for [Ethos Suite Library](https://github.com/jashxn/Ethos-Suite-Library).

The `assets/` directory uses the Roblox fallback asset ID as the file name. The library downloads these PNG files once, writes them to the executor filesystem, and loads them with `getcustomasset`. If local asset loading is not available or a download fails, the matching `rbxassetid://` remains the fallback.

Packed icon sheets are rebuilt from the checked-in source SVG/PNG files with the same `ImageRectOffset` and `ImageRectSize` layout as the Tungsten-generated catalogs. Standalone dashboard, legacy, and shadow assets stay as individual PNGs.

`manifest.json` records the source catalog and dimensions for each runtime file. Third-party icon-set licenses are in `licenses/`.
