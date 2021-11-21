# libfat-nitrofs-run-tutorial
tutorial on how to run libfat and nitrofs<br>
coming soon: tutorial on running dswifi

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
