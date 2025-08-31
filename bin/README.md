#### Прошивки найденные в микроконтроллерах

$\textsf{\color{blue}HC32F460}$<br>
демо-плата с HC32F460JETA - программа мигания светодиодом с разной частотой

$\textsf{\color{blue}N32G452}$<br>
самая интересная прошивка с только впаянного микроконтроллера N32G452CCL7<br>

```
значит впаял вместо  STM32F103C6T6 на плате BluePill (pin2pin совместимые), 
подключился boot слить, а там программа по основным адресам и ~67K - ух
расшифровываю
- настройка портов PG0, PG1
- настройка UART7
... что-то не то
смотрим DS
PG0,PG1,UART7 - только в lqfp-128 ( ???? lqfp-48 ! )

получается это тестовая программа всех узлов микроконтроллера до корпусирования !!!
и лог выдается на UART7 !
```
$\textsf{\color{blue}PY32F002B}$<br>
```
демо-плата (embedfire) - чип PY32F002BF15U6 
тестовая программа (заводская ?)
? тест памяти RAM
? используется порт PA6 на вход 
? значение порта PA6 закодировано в памяти USER OTP 
        0x1FFF02C0: 61  
        bit[3:1] = 0 (port A)  bit[7:4] = 6  =>  PA6
```

Information Block (768 bytes) - описание будет здесь, на примере PY32F002BF15U6
```
0x1FFF0000-0x1FFF007F:  
  0x1FFF0000 - 16 bytes - UID
  0x1FFF0020 - 1 dword - Vrefint  correction value 
               ( high 16 bit is BCD code real value 0x1204 -> Vrefint = 1.204 V)
0x1FFF0080-0x1FFF00FF:  Option bytes
0x1FFF0100-0x1FFF017F:  Factory Config 0
  0x1FFF0100 - 2 dword - константы калибровочные HSI для 24 MHz И 48 MHz  
               ( low 16 bit of dword -  [15:13] HSI_FS ; [12:0] HSI_TRIM )     
0x1FFF0180-0x1FFF01FF:  Factory Config 1
  0x1FFF01A4 - 1 dword - константа калибровочная LSI ( value - low 16 bit )
0x1FFF0200-0x1FFF027F:  Reserved
0x1FFF0280-0x1FFF02FF:  USER OTP
  - всё заполнено кодом 0xFF
  - кроме 0x1FFF02C0: 61 FF 00 00
```

$\textsf{\color{blue}STM32F100}$<br>
плата STM32VLDISCOVERY тестовая программа мигания светодиодом

$\textsf{\color{blue}STM32F103}$<br>
плата BluePill

