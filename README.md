# bare metal c project for beaglebone, ti sitara am335x

## run on beaglebone

```
U-Boot# loady
## Ready for binary (ymodem) download to 0x80200000 at 115200 bps...
C
```

Now press ctl+a s , send file through ymodem.
```
U-Boot# go 0x80200000
## Starting application at 0x80200000 ...

```



## doc

check here for further information:
* http://balau82.wordpress.com/2010/02/14/simplest-bare-metal-program-for-arm/
* http://developers.stf12.net/cpp-demo/gcc-linker-script-and-stm32-a-tutorial
* http://stackoverflow.com/questions/6139952/what-is-the-booting-process-for-arm
* http://www.cs.utsa.edu/~whaley/teach/FHPO_F11/ARM/CortAProgGuide.pdf



