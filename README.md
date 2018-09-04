# buildroot-at91sam9m10-flashloader
modification on sam-ba .tcl patch file for loading the buildroot from windows using sam-ice segger programmer

- download BUildroot

mkdir at91sam_buildroot
git clone git://git.buildroot.net/buildroot
cd buidroot

- check the latest stable release
git tag

- checkout the latest
git checkout 2018.05

- clean any old configuration
make defconfig
make clean

- confifure and for at91sam9m10ek

make at91sam9g45m10ek_defconfig
make

wait until build is complete
copy all files in output/images into folder in microsoft windows OS

place the the files attached on the same folder , connect your board and atmel-ice
run the bat file to load the system on nand flash

you can monitor the progress through board serial debug rs232 port.

Thank you
