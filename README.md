# MCU 32-bit  Review

Небольшой обзор 32-бит микроконтроллеров (хобби такое - не профессионал).<br>
(CH32,PY32,HC32,N32,AT32,STM32, ...)<br>
(RISC-V, Cortex-M0,M0+,M3,M4,M4F, ...)

# Содержание

1. [RISC-V](README.md#risc-v)
   - [WCH CH32V/X](README.md#wch-ch32vx)
       - [CH32V003](README.md#ch32v003) [CH32X035](README.md#ch32x035) [CH32V203](README.md#ch32v203)
2. [Cortex-M0/M0+](README.md#cortex-m0m0)
   - [PUYA](README.md#puya---py32) 
       - [PY32F002A/F003/F030](README.md#py32f002af003f030) [PY32F002B/L020](README.md#py32f002bl020) [PY32F040/F071/F072](README.md#py32f040f071f072)
   - [XHSC(Huada)](README.md#xhschuada---hc32)
       - [HC32L110](README.md#hc32l110) [HC32L130](README.md#hc32l130) [HC32L072](README.md#hc32l072)
   - [HK(Hangshun)](README.md#hkhangshun---hk32)
       - [HK32F030M](README.md#hk32f030m) [HK32L0084/088](README.md#hk32l084088)
3. [Cortex-M4/M4F](README.md#cortex-m4m4f)

# RISC-V  
## WCH CH32V/X
### CH32V003 
### CH32X035 
### CH32V203 

# Cortex-M0/M0+
## PUYA - PY32
### PY32F002A/F003/F030
### PY32F002B/L020
### PY32F040/F071/F072

## XHSC(Huada) - HC32
### HC32L110
### HC32L130
### HC32L072

## HK(Hangshun) - HK32
### HK32F030M
### HK32L084/088

## WXSC - CW32
### CW32L010
### CW32F030
### CW32L031

## Cmsemicon - CMS32
### CMS32L051

## Nations(NSING) - N32
### N32G030/031/032

## ST - STM32
### STM32C011
### STM32L011
### STM32G030
### STM32G031

## Linko - LKS32
### LKS32MC037
### LKS32MC081

# Cortex-M4/M4F





```
boot - прошивки из микроконтроллеров
bin  - прошивки найденные в микроконтроллерах в основной Flash

по возможности будут расшифровки ( постепенные )
```       
#### Подробный разбор по работе с PY32F002A ( F003, F030 )
отдельная статья [PY32F002A_003_030](./PY32F002A_003_030/README.md)

#### Характеристики младших моделей (CM0,CM0+,RV32EC,RV32IMAC)
![MCU](img/mcu1.png)

#### Сравнение потребления из DS

__Зелёным - подтверждённые данные__ 

![Потребление MCU](img/power.png)