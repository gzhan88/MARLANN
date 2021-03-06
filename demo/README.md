A simple demo SoC controlling an MARLANN coprocessor
====================================================

This demo uses two iCEBreaker boards.
One running the control SoC and a second one running MARLANN.

On the MARLANN side PMOD1 is used for the connection:

| Role | Pin Name   | IO Loc |
|:----:|:---------- | ------:|
|  CLK | `P1A1`     |      4 |
|  CSB | `P1A2`     |      2 |
|  IO0 | `P1A3`     |     47 |
|  IO1 | `P1A4`     |     45 |
|  IO2 | `P1A7`     |      3 |
|  IO3 | `P1A8`     |     48 |
|  RDY | `P1A9`     |     46 |
|  ERR | `P1A10`    |     44 |

On the ctrlsoc side two button pins from the break-off section and the flash
`IO[0123]` pins are used for the connection:

| Role | Pin Name         | IO Loc |
|:----:|:---------------- | ------:|
|  CLK | `P2_10`          |     18 |
|  CSB | `P2_9`           |     20 |
|  IO0 | `FLASH_MOSI/IO0` |     14 |
|  IO1 | `FLASH_MISO/IO1` |     17 |
|  IO2 | `FLASH_WP/IO2`   |     12 |
|  IO3 | `FLASH_HLD/IO3`  |     13 |
|  RDY | *none*           |     41 |
|  ERR | *none*           |     39 |
