This directory contains the LOD firmware update files for every model within the 14th Barracuda generation eligible for a firmware update. Note the following naming schemes:

- `PHARAOH-G14` refers to Pharaoh models released as members of the 14th generation, __not__ the 12th (7200.12). Models like ST500DM002 often get confused for being 7200.12 models, so this is a necessary way to distinguish them.
- `GRENADABP-G1-9YN` refers to 1st generation GrenadaBP drives whose part numbers (P/Ns) begin with 9YN, such as ST3000DM001-9YN166.
- `GRENADABP-G1-1CH` refers to 1st generation GrenadaBP drives whose part numbers (P/Ns) begin with 1CH, such as ST3000DM001-1CH166.

Also note:

- The ST2000DM001 has both two and three-disk variants. While I have tested the `GRENADABP-G1-1CH-CC4H-2D.LOD` firmware binary on the two-disk variant of ST2000DM001-1CH164 (as an example), I have not tested the three-disk ones, so tread with caution if you own a three-disk variant.
- The ST500DM002 has both Pharaoh and 1st generation GrenadaBP variants. __PAY ATTENTION TO ITS PART NUMBER!__ If the part number begins with `1BC` or `1BD` (which the overwhelming majority of them are), it is a Pharaoh. If it instead starts with `9YN` or `1CH`, it is a GrenadaBP drive.

You can apply the necessary LOD using the following:

For Windows:

`openSeaChest_Firmware -d \\.\PhysicalDriveX --downloadFW <LOD> --downloadMode segmented`

For Unix-based systems:

`openSeaChest_Firmware -d /dev/sgX --downloadFW <LOD> --downloadMode segmented`
