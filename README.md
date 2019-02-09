![alt text](https://raw.githubusercontent.com/insanelydeepak/High-Definition-Audio-Codec-Installer-Hackintosh/master/HDA%20Codec.jpg)

# Patched AppleHDA Yosemite 10.10.2
Collection of Corrected or Patched AppleHDA for Mac OS X Yosemite Hackintosh's. 
#### New Users/First Experience with AppleHDA: 
 
1 - Identifying Your Audio codec
   
    1 - Read the manufacturer's manual or use DPCI Manager.
    2 - currently supported Codec are: (Realtek,IDT,ADI,Via,Conexant).
    3 - Example of DEVICE_ID Vs Codec_id:10ec0887=ALC887.

####  Requirements:
 
  1 - OSX Versions Supported:
 
    1- Supported Versions of System are: Yosemite 10.10
                               
    2- You must have one of the following DEVICE_ID/Codec name described below or attached here:
 
      1 - Realtek ALC to Desktop's: ALC662,ALC882,ALC883,ALC887,ALC888,ALC889,ALC889A...etc
      2 - ADI for Desktop's: ADI1988B, ADI2000B.
      3 - VIA Desktop's: VT2020_2021
      4 - Realtek ALC to Laptop's: ALC233,ALC268,ALC269,ALC270,ALC272,ALC275,ALC280...etc
      5 - Conexant for laptop's: CX20583,CX20585,CX20588,CX20590,CX20752,CX20756...etc
      6 - RTD for Laptop's: RTD 92HD66C3/65,IDT92HD75B3X5,IDT92HD81B1X5,IDT92HD87B1...etc
      7 - VIA Laptop's: VT1802/VT1802p.
      8 - Cirrus Logic Laptop's: CS4213.
      
####  Determining The Number Layout_Id/Audio_Id By Ports Motherboard:
 
  1 - Audio_ID's / LAYOUT-ID's:
         1 - Always Read README.txt included with Kext 
         2 - All-in-One Versions Contains Various patches, so try different Layout_ID as mentioned in README.txt 

      
#### Injection Of Your Audio_Id or Layout_ID:
 
  1 - Methods: Clover/DSDT/HDEnabler/Chameleon.
 
    1 - DSDT/HDEF/Layout_id = Audio_id
    2 - HDAEnablerX.kext (where "X" corresponds to the number of Audio_ID / desired Layout_ID)
    3 - Clover/Config.plist/Devices/Audio/Inject=Audio_ID
    4 - Chameleon Installer/Customize/Setting/HDEF Layout/
                               
    Note: Use only one of the methods described above.

#### Even Codec Model/Different Pinconfigs And Pathmaps:
 
    1 - Examples Vs Solution:
 
    1 - Internal Microphone do not work or Headphones.
    2 - Install AIO versio of AppleHDA and Read README.txt inject Layout_ID , Choose which suites you better.
                                   
  Note: I have created All-In-One AppleHDA which contains Various PathMap and Pinconfigs for different Output and Inputs .
  You have just changed Layout_ID as mentioned in README.txt file and get desired Output and Inputs.
  
#### Installation:
 
   1 - Requirements/mode:
 
    1 - Install in S/L/E using iKext or KextWizard.
    2 - After installing repair permissions and rebuild caches use an application of your choice.
    3 - Use this flag is mandatory:kext-dev-mode=1 (Only For Yosemite)
 

#### Correction To Get Sound After Waking From Sleep:
   
    1 - Read with attention the two guides below 
                
  1- [EAPD-Codec-Commander](https://github.com/Dolnor/EAPD-Codec-Commander) 
   
  2- [EAPD-FIX](http://forum.osxlatitude.com/index.php?/topic/3084-eapdjack-sense-fix-no-audiojack-sense-issue-after-sleep/)      

####The credit will go for all these people:  
 Mirone , Kabyl, TimeWalker75a, EMlyDinESH, Bcc9 and Others Who Contributed to Patching AppleHDA 
 
 ## Donation
If this project help you reduce time to develop, you can give me a cup of coffee :) 

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](http://paypal.me/insanelydeepak)

