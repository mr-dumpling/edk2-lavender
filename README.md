
Attempt to create a minimal EDK2 for Xiaomi Redmi Note 7.

Based on zhuowei's port for Pixel3XL (https://github.com/Pixel3Dev/edk2-pixel3/).

## Status 

Nothing works yet.. wow, what a surprise!

Anyway, if anyone is willing to help, please join our Discord server [DanctNIX](https://discord.gg/AvtdRJ3).

## Building
Tested on Ubuntu 18.04.

First, clone EDK2.

```
cd ..
git clone https://github.com/tianocore/edk2.git --recursive
git clone https://github.com/tianocore/edk2-platforms.git
```

You should have all three directories side by side.

Next, install dependencies:

18.04:

```
sudo apt install build-essential uuid-dev iasl git nasm python3-distutils gcc-aarch64-linux-gnu abootimg
```

Also see [EDK2 website](https://github.com/tianocore/tianocore.github.io/wiki/Using-EDK-II-with-Native-GCC#Install_required_software_from_apt)

Finally, ./build.sh.

Then fastboot flash boot uefi.img.

# Credits, from the original fork

This is based on zhuowei's [edk2-pixel3](https://github.com/Pixel3Dev/edk2-pixel3).  
SimpleFbDxe screen driver is from imbushuo's [Lumia950XLPkg](https://github.com/WOA-Project/Lumia950XLPkg).  
Special thanks to @lemon1ice, @gus33000 and @imbushuo for guidance.
