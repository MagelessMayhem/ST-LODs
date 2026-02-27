This directory contains the LOD update files for every Maxtor DiamondMax 22 model. Like Barracuda 7200.11, DiamondMax 22 uses the Brinks and Moose platforms, but is only on one firmware branch: MX1x.

Therefore, the only advice is only follows:
- If your drive model has a firmware version of MX1x that is prior to MX1A (for example, MX15), you will want to update it to MX1A.

The firmware can be updated using the following command:

For Windows:

`openSeaChest_Firmware -d \\.\PhysicalDriveX --downloadFW <LOD> --downloadMode segmented`

For Unix-based systems:

`openSeaChest_Firmware -d /dev/sgX --downloadFW <LOD> --downloadMode segmented`
