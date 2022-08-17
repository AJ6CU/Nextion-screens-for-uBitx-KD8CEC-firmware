#Nextion screens for uBitx KD8CEC firmware
 This directory contains Nextion screens for Ian Lee's for his KD8CEC firmware for the uBitx.

KD8CEC (Ian Lee, hamskey.com) developed an enhanced set of firmware for the uBitx transceiver designed by Ashhar Farham (VU2ESE) and sold by his company HF Signals Electronics Pvt. ltd (https://www.hfsignals.com/). KD8CEC created the first touchscreen UX for the uBitx using the Nextion smart screens to offload the processing and memory requirements over the already overloaded Arduino nano used by the uBitx.

Ian created a wide variety of screens, especially for the smaller Nextion screens. Larger screens were not supported and generally resulted in only a portion of the screen being used. 

There are three main folders here:
1. Original_KD8CEC  - these are the ones that Ian Lee originally designed
2. User_Contributed_Screens - these are screens that various users have enhanced or created
3. Resources - currently contains artwork for various size screens that can be leveraged for new screens

So which screens do you choose? Best answer is to try various ones and see what you like. Just be aware that for larger screen sizes (3.5+), Ian Lee's screens were not resized and you will get a black boarder on right and the bottom. This is one of the things that various uses fixed in their contributed screens.

NOTE ON FORMATS

Contained in the subdirectories, there are both ".tft" and "hmi" files. Basically, the "'hmi" files can be thought of as source for the screens that is used by the Nextion GUI Editor to generate (compile) the ".tft" files. By writing the right ".tft" file to a sdcard, and inserting it into your Nextion screen prior to turning on the power, the screen will read the ".tft" file and save the screen formats to its EEPROM.


LEGACY AND RECENT NEXTION SCREENS

There are typically two sub-directories in each section:
- legacy nextion screens
- recent nextion screens

At some point in the last few years, the manufacturer of the Nextion screens changed the firmware that ran on their screens and this required the use of a newer version of the Nextion editor to regenerate the screens that you load on to the Nextion via the SDCARD. (See: https://ubitx.net/mod-add-colour-touch-screen/ for a good set of instrutions on how to load your ".tft" file onto your screen.) You know you are trying to load an older format ".tft" on to a more recent Nextion screen when you see the following message on screen boot:

"file version is too low"

If you get this error message, you are trying to load an older ".tft" version into a recent Nextion screen with newer firmware. The good news is that generally, the ".tft" file generated for recent Nextion screens will also run on older ones (depending on how old they are...  see: https://nextion.tech/faq-items/using-legacy-nextion-devices/ for details)

In general, if you can get away with using the "Legacy" screens you should. With the upgrade of the Nextion Editor, the generated code got larger. This means that to fit in the limited memoryu of the Nextion (especially the Basic and even smaller Enhanced screens), there has been some trimming of text entry sizes and especially the information that can be contained in the QR code used for backup.


NEXTION SCREEN MODELS

Nextion currently sells the following MODELS of its screens:
- Basic
- Discovery
- Enhanced
- Intelligent

It looks to *me* that the Basic version is in the process of being replaced by the "Discovery". Similarly, the "Enhanced" version looks to *me* to be a replacement for Discovery. Unfortunately, the firmware is not compatible between each of these models so you need to find (or generate yourself) a ".tft" file that supports the size and particular model.


HOW DO I KNOW WHAT MODEL OF NEXTION I HAVE?

The model number is coded in the manufacturer part#. The format of the part# is:

NXnnnnmsss

nnnn=a number perhaps coded year?
m= 	T => Basic
	F => Discovery
	E => Enhanced
	P => Intelligent


WHAT NEXTIONS SCREEN SHOULD I BUY?

If available in your desired screen size, spend the extra money and buy the Enhanced or Intelligent. The Basic and Discovery models are slower and have inadequate memory/eeprom to hold the more recent evolutions of the screens.  ALTHOUGH THERE ARE ".tft" files for a 9", it does not appear to be avaiable nor is it supported by the Nextion editor. So DO NOT BUY the 9" model if you find one.


73
Mark
AJ6CU 
email on QRZ
