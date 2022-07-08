# Nextion screens for uBitx KD8CEC firmware
 This repository contains improved Nextion screens that support the original KD8CEC firmware for the uBitx.

KD8CEC (Ian Lee, hamskey.com) developed an enhanced set of firmware for the uBitx transceiver designed by Ashhar Farham (VU2ESE) and sold by his company HF Signals Electronics Pvt. ltd (https://www.hfsignals.com/). KD8CEC created the first touchscreen UX for the uBitx using the Nextion smart screens to offload the processing and memory requirements over the already overloaded Arduino nano used by the uBitx.

Ian created a wide variety of screens, especially for the smaller Nextion screens. Larger screens were not supported and generally resulted in only a portion of the screen being used. 

This work reflects an extension of his work into areas:
1. Additional screen sizes are natively supported (e.g. 5, 7, and 9 etc.)
2. "Enhancements" to the UX that IMHO made it easier to use and fixed some inconsistency.

I have not made any attempt to support the smaller screens that Ian originally supported.

This work is open source and I have included the original Nextion GUI tool input files.  

Note: All compiled with Nextion Editor V0.53. The Nextion Editor LTS (Long Term Support) should be used to edit these files. https://nextion.tech/nextion-editor/#_section2

The current version of the Nextion Editor is 1.63.3. These files have NOT been imported to this release. The FAQ suggested that the firmware on the screen might need to be upgraded on older models to use 1.63.3.  When I have time, will take a look at this. Meanwhile, if you are curious, please try it and report back!

There are two directories:
1. Prebuilt  - these are prebuilt files to uploade to your Nextion screens
2. Source - the input file for the Nextion editor

73
Mark
AJ6CU
