## Disclaimer
| :boom: Disclaimer          |
|:---------------------------|
|  :warning:  Lenovo is a registered trademark, I have no relation to Lenovo, I do not give advice on equipment, if you want to know more about this computer, you can find contacts on lenovo.com and ask there. |
|  :warning:  <b>You can do what is described here only at your own risk.</b> Damage to your computer may occur at any stage of these procedures. |
|  :warning: <b>Please note that many settings in this diff BIOS are stored only in the BIOS chip. If you incorrectly overclock/undervolt your CPU, you will not be able to boot until you reflash the BIOS chip.</b> |
|  :warning:  All rights reserved. |

## original

| name                                                              |  version  |   stable   | machine_type,serialdata |  initialized  | difference  |
| ----------------------------------------------------------------- | --------- | ---------  | ----------------------- | ------------- | ----------- |
| MX25U12835F_2024_GEN2_NO_SERIALKEYS_1.8V@UNDER_THE_COOLING_FAN    |    2024   |     +      |            -            |       -       |    -        |

## unlocked

| name                                                   |  version |   stable    | machine_type,serialdata |  initialized  |      difference      |
| ------------------------------------------------------ | --------- |  --------- | ----------------------- | ------------- | -------------------- |
| MX25U12835F_2024_V1_GEN2_1.8V@UNDER_THE_COOLING_FAN    | 2024, V1  |     +      |            -            |       -       | all_menu             |
| MX25U12835F_2021_V2_GEN2_1.8V@UNDER_THE_COOLING_FAN    | 2021, V2  |     +      |            +            |       +       | all_menu,extended_exit_menu,cbs,pbs     |
| MX25U12835F_2021_V1_GEN2_1.8V@UNDER_THE_COOLING_FAN    | 2021, V1  |     +      |            +            |       +       | all_menu,cbs,pbs     |

### Description of table column
| value     |                  description                 |
| --------- | -------------------------------------------- |
| <b>version</b>   |  Year of BIOS release version, V - designation of the version of the difference (a higher number means a later version) |
| <b>stable</b>    |    Is bios dump suitable for everyday use?   |
| <b>machine_type,serialdata</b> | Were the device type, serial numbers, MAC addresses previously recorded in the dump? (if you want to install this dump, you will need to manually enter the data through a hex editor or use the manufacturer's software to install them) |
| <b>initialized</b> | Was this BIOS version loaded from a working device, and therefore with some default configuration installed? |

### Difference
| value              |                  description                 |
| ------------------ | -------------------------------------------- |
| <b>all_menu</b>           |  All BIOS menus that allow you to fine-tune your devices (chipset, superio, sata, usb, pcie, ...) |
| <b>extended_exit_menu</b> |  The same exit menu but more expanded due to the ability to launch efi.                           |
| <b>cbs</b>                |  <b>CBS</b>                                                                                       |
| <b>pbs</b>                |  <b>PBS</b>                                                                                       |
