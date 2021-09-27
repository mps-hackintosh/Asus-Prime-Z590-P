# Asus-Prime-Z590-P

     BELOW CONFIGS DO NOT WORK !!
     I WAS NOT ABLE TO MAKE A Z590 MOBO TO WORK WITHOUT USING A dGPU !!  
     INSTEAD OF BYING dGPU, I CHANGED THE MOTHERBOARD TO A Z490.
     BUT YOU CN TRY BELOW FRAMEBUFFER PATCHING AND SEE IF ADDING SOME (NOT ALL) OF THESE VALUES WORKS
     
```XML
<key>AAPL,ig-platform-id</key><data>BwCbPg==</data>

<key>device_type</key><string>VGA compatible controller</string>
<key>AAPL,slot-name</key><string>Internal@0,2,0</string>

<key>enable-hdmi20</key><data>AQAAAA==</data>
<key>model</key><string>Intel UHD Graphics 630</string>
<key>framebuffer-patch-enable</key><data>AQAAAA==</data>
<key>framebuffer-unifiedmem</key><data>AAAAgA==</data>
<key>hda-gfx</key><string>onboard-1</string>

<key>framebuffer-con0-enable</key><data>AQAAAA==</data>
<key>framebuffer-con1-enable</key><data>AQAAAA==</data>
<key>framebuffer-con2-enable</key><data>AQAAAA==</data>

<key>framebuffer-con0-pipe</key><data>EgAAAA==</data>
<key>framebuffer-con1-pipe</key><data>EgAAAA==</data>
<key>framebuffer-con2-pipe</key><data>EgAAAA==</data>

<key>framebuffer-con1-busid</key><data>BgAAAA==</data>
<key>framebuffer-con2-busid</key><data>BAAAAA==</data>
		
<key>framebuffer-con2-type</key><data>AAgAAA==</data>
```			
				     			
			
               

Attached is my EFI, SSDT & config.plist setup. 

But its not working. getting kernel panic 

My system config is 

    MOBO        - Asus Prime Z590-P 
    CPU         - Intel 10700K
    WIFI CARD   - FENVI T919
    RAM         - XPG DS60 32 GB
    M.2 Nvme    - XPG S40G 256GB RGB 3D NAND PCIe Gen3x4 NVMe 1.3 M.2 2280 Internal SSD
    2.5 SSD     - WD-Blue 500GB
    NO GRAPHICS CARD
    
 ! [Log Before Broken Text](https://github.com/manvendra/Asus-Prime-Z590-P/blob/main/Installation%20Logs%20Just%20before%20broken%20Letters.png)
 
 ! [Log With Broken Text](https://github.com/manvendra/Asus-Prime-Z590-P/blob/main/Installation%20Logs%20having%20Letters%20broken.png)
 
 Not sure if some logs are there between above 2 becuase it scrolls fast, second screenshot is the one where screen stops after first screenshot.
 And the second screen with broken text keep adding few blank line at botton each minute. like refreshing it
