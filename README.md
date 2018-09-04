# buildroot-at91sam9m10-flashloader
modification on sam-ba .tcl patch file for loading the buildroot from windows using sam-ice segger programmer

1) download buildroot

#mkdir at91sam_buildroot
#git clone git://git.buildroot.net/buildroot
#cd buidroot

2)  check the latest stable release

#git tag

3) checkout the latest

#git checkout 2018.05

4) clean any old configuration

#make defconfig
#make clean

5) confifure and for at91sam9m10ek

#make at91sam9g45m10ek_defconfig
#make

6)wait until build is complete

7)copy all files in output/images into folder in microsoft windows OS

8)paste and replace your image files to the repository folder contenets
9) connect your board and atmel-ice
10)run the bat file to load the system on nand flash

you can monitor the progress through board serial debug rs232 port.

Thank you
