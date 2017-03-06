## config.txt - Onboard analogue audio (3.5mm jack)

The onboard audio output has a few config options which alter the way the analogue audio is driven and whether some firmware features are enabled or not.

### disable_audio_dither

By default, a 1.0LSB dither is applied to the audio stream if it is routed to the analogue audio output. This can create audible background "hiss" in some situations, such as if the ALSA volume is set to a low level. Set this to `1` to disable dither application.

### pwm_sample_bits

Adjust the bit depth of the analogue audio output. The default bit depth is `11`. Selecting bit depths below `8` will result in nonfunctional audio, as settings below `8` result in a PLL frequency too low to support. This is generally only useful as a demonstration of how bit depth affects quantisation noise.






*This article uses content from the eLinux wiki page [RPiconfig](http://elinux.org/RPiconfig), which is shared under the [Creative Commons Attribution-ShareAlike 3.0 Unported license](http://creativecommons.org/licenses/by-sa/3.0/)*