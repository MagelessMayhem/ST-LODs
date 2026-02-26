This directory contains the LOD update files for every Barracuda 7200.11 model. There are two platforms that this series uses, being Brinks and Moose.

You **DO NOT** need a firmware update if:

- you already have a Brinks drive, i.e. ST31500341AS, that is on firmware SD1A/CC1H or later (later versions such as CC4G and SD1B);
- you already have a Moose drive, i.e. ST3500320AS or ST31000340AS, that is on an SDxA firmware version or later. The use of "x" is necessary because four different firmware branches exist which all end at an SDxA version.

You **DO** need a firmware update if your drive's firmware is anything prior to SDxA or CC1H. A well-known example of a "faulty" firmware version is SD15, which was released well before SD1A.

# What is my drive's firmware branch?

For Moose drives, you'll usually want to pay attention to the first three or four characters of the firmware version:
- If the firmware version is either SD1x, SD81, or AD14, you'll want to use SD1A.
- If the firmware version is SD2x, you'll want to use SD2A.
- If the firmware version is SD3x, you'll want to use SD3A.
- If the firmware version is SD4x, you'll want to use SD4A.

For Brinks drives:
- If the firmware version is SD1x, you'll want to use SD1A or SD1B.
- If the firmware version is CC1x (and is critically __prior to__ CC1H), you'll want to use CC1H.
