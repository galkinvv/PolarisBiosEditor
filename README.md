# PolarisBiosEditor - fork with additional data views

# Below is readme for upstream version.


### PolarisBiosEditor tweaked by vaske version 3.8 with pro timings can buy on miningbios.com
## https://www.miningbios.com

BTC donation address: 181dtEjhFWWxvHDmx2R3N41rnRPedSEUf5

works on linux with mono, executable is build against .net 3.5

one click timing feature should be used with care, it maybe not stable for you

please build the executable yourself or decompile the existing one if you don't trust

If you want to use PolarisBiosEditor on Ubuntu need to install module: sudo apt install libcanberra-gtk-module libcanberra-gtk3-module


### v1.7.3
- Fixed apply timings for Samsung memory
- Added support for New Samsung memory K4G80325FC
- Added timing for New Samsung K4G80325FC
- Applying from 1750 to upper

### v1.7.2
- Fixed apply timings for Hynix memory
- Added support for RX590
- Added support for New Hynix memory H5GC8H24AJ
- Added timing for New Hynix H5GC8H24AJ

### v1.7.1
- Updated Elpida Timing

### v1.7.0
- Added New timing for Hynix.
- Added Clock Stretch Amount.
- Added option for choosing timings on hynix Between Universal Hynix timing and Good hynix timing.
- Universal Hynix timing work on: H5GC8H24MJ, H5GQ8H24MJ, H5GQ4H24AJ.

### v1.6.9
- Fixed UI (updated design)
- Fixed and Updated all Timing's
- Added New strap for Micron and Hynix
- Added option for choosing timings on samsung between uber-mix 3.1 and 3.2, and on Micron between Good Micron timing and S Micron timing.
- Added Icon
- Added option for max. Mem. freq. (after one click timing patch button click automatically change max. mem. to 2300 MHz)

### v1.6.8
- Fixed Samsung Uber-Mix strap
- Added support for Hynix H5GQ4H24AJ
- Fixed fan mod option

### v1.6.7
- created solution and project files for ide
- support for device id 0x67ef
- better timings for micron memory
- firmware signature test / firmware signature in ascii
- editing of bios message (experimental)
- online check for new versions
- online display of developer notice

### v1.6.6
- support for rx550 device id 0x699F

### v1.6.5
- support up to 48 entrys in the timings table (more than 2 memory vendors)

### v1.6.4
- elpida timings fixed
- K4G41325FS memory support

### v1.6.3
- timing modification starts now at 1500 instead of 1750
- device id 67FF now also supported

### v1.6.2
- experimental: ubermix timings are now also applied to 4g SAMSUNG vram (K4G41325FC, K4G41325FE)
- timing modification starts now at 1750 instead of 2000

### v1.6.1
- hynix memory H5GC8H24MJ now recognized (same timings as H5GQ8H24MJ)

### v1.6
- window resizes properly now
- memory vendor detection
- one click timing patch (samsung, hynix, elpida, micron)

### v1.5
- added FanControlMode setting
- implemented some timing editor related code (not usable yet)

### v1.4.1
- replaced WPF components with Windows Forms to archive mono compatibility

Contribution from Sebohe:

### Build Dependencies

Ubuntu 16.04.2:

```
sudo apt-get install mono-complete
```

Arch Linux:

```
yaourt -Sy mono48
```
### Building

```
sh build.sh
```

### Executing

Just change your working directory to the PolarisBiosEditor and execute:

```
./run.sh
```
