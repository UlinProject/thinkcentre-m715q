<div id="header" align="center">
  
  <b>[thinkcentre-m715q]</b>
  
  (Modification kit for small PC m715q..)
  </br></br>
<div id="badges">
  <a href="https://github.com/denisandroid">
    <img src="https://github.com/UlinProject/img/blob/main/short_32/uproject.png?raw=true" alt="uproject"/>
  </a>
</div>
</div>

## Description:
This is a collection of mods that can be performed on the m715q to get the most out of these little computers. Mods require some level of skill and equipment, depending on which mod is performed.

## Disclaimer:
Do everything outlined here at your own risk. Damage to your computer can occur at any step during these procedures.

All rights reserved.

## Specifications:

### Gen1:
| name | value |
| ---- | ----- |
| board | m715q GEN 1 |
| cpu_0 | AMD PRO A12-8870E (x4 2.9 (turbo: one x1 3.8Ghz)) |
| cpu_1 | AMD PRO A10-8770E (x4 2.8 (turbo: one x1 3.5Ghz)) |
| mem | DDR4-2400, max: 32Gb (officially) |
| bios | Winbond 25q64fwsig (8mb) |

### Gen2:
| name | value |
| ---- | ----- |
| board | m715q GEN 2 |
| cpu0 | AMD Ryzen 5 PRO 2400GE (x4x2 3.2Ghz (overclock: 3.6Ghz) (turbo: one x1 3.8Ghz)) |
| cpu1 | AMD Ryzen 3 PRO 2200GE (x4 3.2Ghz (overclock: 3.6Ghz) (turbo: one x1 3.6Ghz)) |
| mem | DDR4-2933, max: 32Gb (officially) |
| bios | MX25U12835F (16mb) |

## Converting a Gen1 board to a Gen2 board:
Although the boards are slightly different, a Gen1 board can easily be converted to a Gen2 board, allowing access to the new processors and features.

The GEN1 board has a Winbond 25q64fwsig BIOS chip (see photos for chip location). You should replace this chip with a 16MB BIOS chip, such as the MX25U12835F or W25Q128FWSIG.

BIOS chips are rated for 1.8V only. Do not attempt to solder a 3.3V chip. You will also need a 1.8V module for your programmer to flash the chip (flashing at 3.3V may damage the chip or result in an incomplete flash).

The BIOS chip should be flashed with a stock BIOS or a modified BIOS from the repository (note that these have test serial numbers embedded in them)

## Unlocked BIOS:
Please note that there is an unlocked BIOS dump available in the repository, taken from a public source. It can do many things, such as enable overclocking and allocate video memory (up to 10GB, I think).

It can be directly flashed to a GEN2 system. For GEN1 systems, see instructions on converting a GEN1 system to a GEN2 system.

Please note that many settings in this unlocked BIOS are stored only in the BIOS chip. If you incorrectly overclock/undervolt your CPU, you will not be able to boot until you reflash the BIOS chip.

<i>If you don't want to flash a GEN2 system, you can download Smokeless_UMAF to a USB stick from an external source and load TianocoreBios from there with some features unlocked. However, you will only get full functionality from an unlocked BIOS (and note that incorrect settings in Smokeless, as well as settings in the flashed BIOS, can damage the board, in the best case you will have to flash the BIOS chip).</i>

## Overclocking and Undervolting (applies to both 2400GE and 2200GE):
Please note that this list is not complete (lower frequencies can be undervolted even more).
Added lower voltages for higher frequencies. Also added 1.0 GHz and added overclock to 3.6 GHz (you can just leave 3.6 off your list if you don't need it).

|0|        1|        2|         3|          4|
|--------| --------| --------|  --------|   --------|
|3600 Mhz| 3200 Mhz| 2300 Mhz|  1600 Mhz | 1000 Mhz |
|1.293750| 1.293750| 97500 v|   87500 v |  77500 v |
|90|       80|       8a (138)|  80 |       50 (80) |
|8|        8|        C (12)|    10 |       10 (16) |
|29|       29|       5C (92) v| 6C |       7C (124) v |

<i>Please note that overclocking does not affect turbo mode (which is only available on one core).</i>

### For extreme overclocking (in case of an error, reflash the BIOS):

| Voltage | Ghz |
| ------- | --- |
| 1,3 ≤ 1,288 | <b>3.929</b> |
| 1,35 ≤ 1,344 | <b>3.979</b> |
| 1,4 ≤ 1,394 | <b>4.054</b> |
| 1,45 ≤ 1,444 | <b>4.076</b> |
| 1,5 ≤ 1,494 | <b>4.129</b> |

## Processor scalping (tested on 2200GE and 2400GE):

Few people know that AMD APUs have thermal paste inside, and quite a thick layer at that, and this thermal paste dries out over time. For effective scalping, it is recommended to soak the processor in a solvent for 10-20 minutes, then cut off the sealant with a razor blade (be extremely careful or skip the scalping step, or better yet, buy a ready-made scalping kit for such processors). It is important not to scratch the printed circuit board, as this can damage the APU. Next, you can apply a thin layer of liquid metal to the processor, for example, with cotton swabs, or try not to use the processor cover (not tested and most likely impossible) and glue the processor cover onto the sealant (or the cover is not glued, but there is a risk of metal leakage outside the processor). <i>You can also isolate the APU components by coating them with varnish.</i>

<i>Please note that we only applied liquid metal to the CPU itself under its heat spreader, it is completely chemically stable as the CPU cover is nickel plated copper. </i>

<i><b>DO NOT</b> try to apply liquid metal between the cooler and the CPU cover, even if it is copper (pure copper will absorb the liquid metal over time and impair cooling)</i>














