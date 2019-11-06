# Addressable LEDs (WS2812B)
Controls a string of addressable LEDs with the WS2812B, like [Neopixels](https://www.adafruit.com/category/168). This example controls 16 LEDs, which is configurable by the `LED_COUNT` value in `Src/ws2812b_conf`.

## Connections

From the LED strip, connect:

* Data -> `PA6`
* Power -> `Vin` or `Batt+`
* Ground -> `GND`

## Compiling/Flashing
See the instructions [here](../README.md)

## WS2812B API Library
Read about how to use the provided WS2812B APIs in the [ws2812b.h](./Src/ws2812b.h) file.

The API & implementation is based on [this tutorial](https://github.com/MaJerle/STM32_WS2812B_TIM_PWM_DMA),
which uses the DMA controller to send the WS2812B data using a timer PWM.