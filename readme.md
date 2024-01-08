[TMC_BLDC 软件部分](https://github.com/Sandman6z/TMC_BLDC)

[TMC_BLDC 硬件部分](https://github.com/Sandman6z/TMC_BLDC_Hardware)

ADI manufacturer provides supporting API for changing the standard library to HAL library.

[GitHub - trinamic/TMC-API: TRINAMIC's IC API](https://github.com/trinamic/TMC-API)

Manufacturer Reply:
使用的时候， 您只需要按照您的MCU平台重新写一个SPI的读写函数就行了。 
您如果使用的STM32， 应该还好写。只在您的main.c里面重新写写一个SPI读写函数即可， 
其余功能您可以直接调用这些api来写您自己的应用程序。 
// => SPI wrapper
extern xxxxx
// <= SPI wrapper

//spi access
...