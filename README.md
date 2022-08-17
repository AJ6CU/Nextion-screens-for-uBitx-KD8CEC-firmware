# Original Nextion screens for uBitx KD8CEC firmware
 This directory contains original Nextion screens designed by Ian Lee for his KD8CEC firmware for the uBitx.

KD8CEC (Ian Lee, hamskey.com) developed an enhanced set of firmware for the uBitx transceiver designed by Ashhar Farham (VU2ESE) and sold by his company HF Signals Electronics Pvt. ltd (https://www.hfsignals.com/). KD8CEC created the first touchscreen UX for the uBitx using the Nextion smart screens to offload the processing and memory requirements over the already overloaded Arduino nano used by the uBitx.

Ian created a wide variety of screens, especially for the smaller Nextion screens. Larger screens were not supported and generally resulted in only a portion of the screen being used. 

#NOTE ON FORMATS
Contained in the subdirectories, there are both ".tft" and "hmi" files. Basically, the "'hmi" files can be thought of as source for the screens that is used by the Nextion GUI Editor to generate (compile) the ".tft" files. By writing the right ".tft" file to a sdcard, and inserting it into your Nextion screen prior to turning on the power, the screen will read the ".tft" file and save the screen formats to its EEPROM.


#LEGACY AND RECENT NEXTION SCREENS
There are two sub-directories in this section:
- legacy nextion screens
- recent nextion screens

At some point in the last few years, the manufacturer of the Nextion screens changed the firmware that ran on their screens and this required the use of a newer version of the Nextion editor to regenerate the screens that you load on to the Nextion via the SDCARD. You know you are trying to load an older format ".tft" on to a more recent NExtion screen when you see the following message on screen boot:

"file version is too low"

If you get this error message, you are trying to load an older ".tft" version into a recent Nextion screen with newer firmware. The good news is that generally, the ".tft" file generated for recent Nextion screens will also run on older ones (depending on how old they are...  see: https://nextion.tech/faq-items/using-legacy-nextion-devices/ for details)

There are two versions of the Nextion editor:
- Nextion Editor LTS (Long Term Support) 
- V1.63.3

The ".tft" files in the legacy section are exactly the same as the ones generated originally by Ian Lee and made available in his repository:

https://github.com/phdlee/ubitx/releases/download/1.1/UBITX_Nextion_GUI_V3.zip



#NEXTION SCREEN MODELS
Nextion currently sells the following MODELS of its screens:
- Basic
- Discovery
- Enhanced
- Intelligent

It looks to *me* that the Basic version is in the process of being replaced by the "Discovery". Similarly, the "Enhanced" version looks to *me* to be a replacement for Discovery. Unfortunately, the firmware is not compatible between each of these models so you need to find (or generate yourself) a ".tft" file that supports the size and particular model.

#HOW DO I KNOW WHAT MODEL OF NEXTION I HAVE?

The model number is coded in the manufacturer part#. The format of the part# is:

NXnnnnmsss

nnnn=a number perhaps coded year?
m= 	T => Basic
	F => Discovery
	E => Enhanced
	P => Intelligent

#WHAT NEXTIONS SCREEN SHOULD I BUY?
If available in your desired screen size, spend the extra money and buy the Enhanced or Intelligent. The Basic and Discovery models are slower and have inadequate memory/eeprom to hold the more recent evolutions of the screens.

#HOW DO I CUSTOMIZE AND GENERATE MY OWN tft FILES
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
