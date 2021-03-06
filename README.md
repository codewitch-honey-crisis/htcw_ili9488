# ILI9488

A GFX enabled device driver for the ILI9488

This library allows GFX to bind to an ILI9341 display so that you can use it as a draw target.

Documentation for GFX is here: https://www.codeproject.com/Articles/5302085/GFX-Forever-The-Complete-Guide-to-GFX-for-IoT

To use GFX, you need GNU C++14 enabled. You also need to include the requisite library. Your platformio.ini should look something like this:

```
[env:node32s]
platform = espressif32
board = node32s
framework = arduino
lib_deps = 
	codewitch-honey-crisis/htcw_ili9488@^0.9.0
lib_ldf_mode = deep
build_unflags=-std=gnu++11
build_flags=-std=gnu++14
```