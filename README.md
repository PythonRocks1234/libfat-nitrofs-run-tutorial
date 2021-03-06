# im tired
if i screwed up anything report at the issues tab<br>
**NOTE: this tutorial is meant to be private**<br>
**It is not a very good tutorial**<br>
**It is not official!!!!**

# libfat-nitrofs-run-tutorial
tutorial on how to run libfat, nitrofs and dswifi<br>
none of the roms or assets are mine

# what is libfat and nitrofs
[Wikipedia: libfat](https://en.wikipedia.org/wiki/Libfat "libfat")<br>
basically with libfat you can read and write to sd cards<br><br>
[ProjectWiki: nitrofs](http://blea.ch/wiki/index.php/Nitrofs "Nitrofs")<br>
with nitrofs, you can have a read only filesystem inside of the rom

# how to get libfat working
**Note: might not work on actual nintendo ds, only on [melonDS](http://melonds.kuribo64.net)**<br>
1. download melonDS here [melonDS site: download link](http://melonds.kuribo64.net/downloads.php)
2. get the bios needed to run programs
    - info is avaliable at [melonDS site: faq](http://melonds.kuribo64.net/faq.php)
    - 2 ways to obtain firmware and bios
    - 1st way (legal):<br>
         dump from actual hardware [no intro wiki](https://wiki.no-intro.org/index.php?title=Nintendo_DS(i)_Dumping_Guide)
    - 2nd way (illegal):<br>
         download at [emulator wiki](https://emulation.gametechwiki.com/index.php/Emulator_Files)
3. configure your melonDS
    - go to config, go to DS-mode, load in your files
    - should look like the below image<br>
        ![this](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/bios_loaded.png "bios loaded")
    - configure button presses and layout and other things now
4. now you need to enable DLDI (dynamically linked device interface)
    - go to config, go to DLDI, load in your files
    - click the checkbox that says "enable DLDI"
    - load in an SD card image
    - here is one at [this repo: SD card](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/sd.img)
    - if you need a bigger one make it yourself at [mediafire download link](https://www.mediafire.com/file/cfr9q8542e9lsos/Virtual_SD_Card_Maker.zip/file)
5. you are ready
    - congrats, you can now use libfat homebrew
    - test if it works at [this repo: test rom](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/libfatdir.nds) (reading)
    - [this repo: test rom](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/libfatwritetest.nds) (reading and writing)
6. notes
    - might work on desmume??
    - will not work on No$GBA (search "No$GBA libfat" for a solution)

# how to get nitrofs working
**Note: might not work on actual nintendo ds, only on [No$GBA](http://problemkaputt.de/gba.htm)**<br>
1. download the emulator (i use the debug version but it should work with gaming)
2. configure your settings (options then controls)
3. nitrofs should work now
4. test it
    - test if it works at [this repo: test rom](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/nitrodir.nds)
5. notes
    - might work on desmume??
    - will not work on melonDS (reasons at [melonDS github: one](https://github.com/Arisotura/melonDS/issues/1116) and [melonDS github: two](https://github.com/Arisotura/melonDS/issues/1043))

# how to get dswifi working
1. follow steps 1-3 of how to get libfat working (set up melonDS)
2. go to config, wifi settings, tick the two checkboxes and use "indirect mode"
3. you're gonna need piracy for this step
    - this is very legal /j
    - basically you're gonna need a nintendo ds rom that has wifi settings
    - for legal reasons i will not be uploading the rom here (dump it yourself)
    - anyway what you want to do is to go to "nintendo wfc connection"
    - i use pokemon black 2 to do the setup (i totally own a copy of pokemon black 2 yes)<br>
        ![legal](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/very_legal_game.png "setup")
    - click options then "erase nintendo wfc configuration" (no more old settings)
    - click back, go to nintendo wifi connection settings
    - click connection 1, use the melonAP access point
    - the ssid should be "melonAP"
    - auto obtain ip address can be yes
    - auto obtain dns must be set to no
    - primary dns should be "164.132.44.106" (wiimmfi server), other servers can be used
    - click test connection (it should be successful)
4. congrats
    - test if it works at [this repo: test rom](https://github.com/PythonRocks1234/libfat-nitrofs-run-tutorial/blob/main/assets/httpget.nds)
5. notes
    - will not work on desmume (they wont support wifi)
    - might work on no$gba and actual ds??
    - there will be no melonAP on an actual ds, you must make your own AP with some unsecured wifi
