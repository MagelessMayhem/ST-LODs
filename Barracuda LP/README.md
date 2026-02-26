This directory contains the LOD update files for every Barracuda LP model. Every model is based on the Hepburn platform, so there only exists one directory: Hepburn.

The following LODs are available, with compatible models:

- `HEPBURN-CC35-2H.LOD`, which is only compatible with the ST3500412AS;
- `HEPBURN-CC35-4H.LOD`, which is only compatible with the ST31000520AS;
- `HEPBURN-CC35-8H.LOD`, which is compatible with both ST31500541AS and ST32000542AS.

To install any of the LODs, use the following (assuming you scanned the drive list with openSeaChest previously):

Windows:

`openSeaChest_Firmware -d \\.\PhysicalDriveX --downloadFW <LOD> --downloadMode segmented`

Unix-based systems:

`openSeaChest_Firmware -d /dev/sgX --downloadFW <LOD> --downloadMode segmented`
