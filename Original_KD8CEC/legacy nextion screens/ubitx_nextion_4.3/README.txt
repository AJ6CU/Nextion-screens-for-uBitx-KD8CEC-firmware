#FILES FOR 4.3" SCREEN

DECODING FILE NAMES:
rule :
  ubitx + _ + Option1 + LCD Type + Option2 + .hmi

Option : Default => empty
           Template => Temp

LCD Type : 2.4" => 24
               2.8" => 28
              3.2" => 32

Option : Basic => empty
         Enhanced => _E
	 Intelligent =>_P
-----------------------------------------------------------------------------

Example : Basic 2.4 Basic Model (NX3224T024_011)
             ubtix_24.HMI  (source code)
             ubtix_24.tft   (precompiled)
             ubtix_Temp24.HMI  (Template file)

Example : Enhanced 2.8 Model (NX3224K028_011)
             ubtix_28_E.HMI (source code)
             ubtix_28_E.tft   (precompiled)
             ubtix_Temp28_E.HMI  (Template file)

Example : Intelligent 4.3 Model (NX4827P043-011)     
             ubtix_43_P.HMI (source code)
             ubtix_43_P.tft   (precompiled)
             ubtix_Temp43_P.HMI  (Template file)