# PSR-8000 Firmware Reverse engineering

Everything is working in progress.

The only missing dump is the BIOS image of the main CPU (SH7043 internal flash), if anybody have it, please submit a pull-request to this project!

And I'm fixing mainboard and patching the main program image, attempting to read the BIOS image from the CPU.


## Dumps

`SYSTEM.bin` is word-interleaved file of XT567/XT568 main program image.

`DATA.bin` is endian-corrected file of IC3 image, which contains text or image resources of this keyboard.

`STYLE.bin` is word-interleaved file of IC4/5 style EPROM image.

`WAVE.bin` is word-interleaved file of IC6-IC9 waveform EPROM image.

Current firmware has two version tags `PSR-8000 MAIN ROM Ver.0.61 Copyright (c) YAMAHA 1997 Rev.0.00 Oct 29 1997 19:31:50` and `1011997OCT29214653`.

I've heard that `v1.12` is the latest firmware version of this keyboard but I haven't get my hands on it.


## Author

Zhiyuan Wan <h@iloli.bid>, 2025/11/19


## Special Thanks

* [PCMATOM](https://www.youtube.com/channel/UC5YGXDEsgjxsfqxB2FMREkw) - for kindly loaned the mainboard of PSR-8000 to me.
