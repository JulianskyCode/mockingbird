WARNING
============
R0A is an alpha version of this project, it may contain issues and work incorrectly!!!

If you want to manufacture the hardware by yourself, please use R01 version or do some hardware hacking by following these steps:
(Not available yet)

Known Issues:

- 1.SDC2 assigned on fault GPIO port, need to remap to PC port or CPU can't boot from SD card.
- 2.AXP209 need to control 3.3V power rail by using an EXTEN signal. If 3.3V is up without control, AXP209 I2C interface won't work(WHAT THE...!) and the processor can only work at 400MHz due to fiexed core voltage. So need to cut the wire connected to PIN1 of 3.3V SY8009 and fly it to EXTEN of AXP209. Then processor runs at 1GHz now :).
- 3.Wrong PCB footprint of SPI flash. May need some mechanical work to solder it.
