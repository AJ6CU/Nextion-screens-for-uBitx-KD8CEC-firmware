# Nextion screens for uBitx KD8CEC firmware
 This directory contains various Nextion screens for Ian Lee's KD8CEC firmware for the uBitx.

KD8CEC (Ian Lee, hamskey.com) developed an enhanced set of firmware for the uBitx transceiver designed by Ashhar Farham (VU2ESE) and sold by his company HF Signals Electronics Pvt. ltd (https://www.hfsignals.com/). KD8CEC created the first touchscreen UX for the uBitx using the Nextion smart screens to offload the processing and memory requirements over the already overloaded Arduino nano used by the uBitx.

Ian created a wide variety of screens, especially for the smaller Nextion screens. Larger screens were not supported and generally resulted in only a portion of the screen being used.

The "Ian Lee Original Screens" are in the folder "Original_KD8CEC".  Screens that have been designed by others are in the folder "User_Contributed_Screens". In general, the original screens are you best choice for the smaller screens (<3.2") that are "BASIC". Larger screens, and especially "ENHANCED" or "INTELLIGENT" models have more memory and are faster you should check out the "User_Contributed_Section". They tend to have more functions and, more importantly, they fill out the full screen. Many of Ian's screens in the larger models are just non-resized versions of the smaller screens

#NOTE ON FORMATS
Contained in the subdirectories, there are ".tft" and "hmi" files. Basically, the "'hmi" files can be thought of as source for the screens that is used by the Nextion GUI Editor to generate (compile) the ".tft" files. By writing the right ".tft" file to a sdcard, and inserting it into your Nextion screen prior to turning on the power, the screen will read the ".tft" file and save the screen formats to its EEPROM. 


#NEXTION SCREEN MODELS
Nextion currently sells the following MODELS of its screens:
- Basic
- Discovery
- Enhanced
- Intelligent

It looks to *me* that the Basic version is in the process of being replaced by the "Discovery". Similarly, the "Enhanced" version looks to *me* to be a replacement for Discovery. Unfortunately, the firmware is not compatible between each of these models so you need to find (or generate yourself) a ".tft" file that supports the size and particular model.

***************************************************************************
NOTE!!!!  Not all the screens have been tested on platforms provided. In particular, the newer Intelligent and Discovery screens have generally not been tested and we are relying on the Nextion Compiler to correctly generate the files!  Be aware of this potential problem if you buy one of these newer models. There is one existent proof (4.3 screen) where this worked. So I am confident that there should be "no problems" ;-)
***************************************************************************

#HOW DO I KNOW WHAT MODEL OF NEXTION I HAVE?
The model number is coded in the manufacturer part#. The format of the part# is:

NXnnnnmsss

nnnn=a number perhaps coded year?
m= 	T => Basic
	F => Discovery
	E => Enhanced
	P => Intelligent

sss=	screen size e.g. 032 is a 3.2 inch screen

If you need to reach me, you can look my email address up on QRZ. I also frequently monitor the BTIX20 group on groups.io
73
Mark
AJ6CU
