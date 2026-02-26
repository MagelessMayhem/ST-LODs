This repository contains a variety of LOD files specifically meant to assist with updating the firmware on Seagate hard drives. **PLEASE READ BELOW BEFORE USING THESE.**

# Applying a Firmware Update

I highly suggest using openSeaChest for this task, as its `openSeaChest_Firmware` sub-command is capable of directly flashing LOD files to compatible drives. It also has the necessary checks in place to prevent firmware mismatching. You can download openSeaChest [here.](https://github.com/Seagate/openSeaChest)

To find the correct update, you will need to determine two things:
- What series your drive is from (i.e. Barracuda 7200.12);
- What platform your drive is based on. Models upon that platform are listed in the appropriate series folder.

In some cases, like with Barracuda 7200.11, you may also need to determine what _firmware branch_ your drive is on so as to prevent potential corruption. (This is also mentioned in the appropriate series folder, so that work is done for you.)

Firmware files listed here are named per the following structure:

`<PLATFORM>-<VERSION>-<# OF HEADS/DISKS>.LOD`

Again, please refer to the series folder to determine which LOD to use.

To actually apply the LOD update, first determine where your drive is with openSeaChest (you may need admin/root):

`openSeaChest_Firmware --scan`

Then with the drive handle known, you can flash the LOD:

For Windows:

`openSeaChest_Firmware -d \\.\PhysicalDriveX --downloadFW <LOD>`

For Unix-based systems, such as those on the Linux kernel:

`openSeaChest_Firmware -d /dev/sgX --downloadFW <LOD>`

Note that older Seagate drives may require using the `--downloadMode segmented` flag to have their updates applied.
