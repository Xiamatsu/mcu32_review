##  Обзор и тестирование семейства контроллеров PY32F002A,F003,F030

### Введение
Данные чипы построены на одном кристалле и имеют все свойства старшей модели PY32F030. Ограничение есть только на возможности назначения функций на существующие порты в корпусе. 
(например управление LED сегментными индикаторами возможно только в корпусах 32pin - а это только PY32F030)<br>

Вся внутренняя переферия
```
LSI - 32.768kHz
LSE - 0-1000kHz  (F030: lqfp32, qfn32, tssop20 pinout1 )
HSI - 4,8,16,22.12,24MHz (есть калибровочные константы)
HSE - 4-32MHz
PLL - x2 (from HSI or HSE)
DMA - 3ch, IWDG, WWDG, SysTick, RTC
Timers (16b): Adv:1, GP:4, LP:1, 
2x USART, 2х SPI, 1x I2C
ADC 12bit (10+2ch) (1Msps), 2x Comp
Max Frequency: 48MHz
1.7 - 5.5 V
Hardware CRC-32 module
Support 4-digit 8-segment common-cathode LED digital tube (F030)
```

Дополнительные сведения по серии из [Factory Config](../boot/py32f0xx/README.md)

