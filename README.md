# Olympus-mic-d
Contains the driver CD data documents related to the Olympus Mic-D digital microscope.

<img src="images/mic-d-in-operation.jpg" width="600">

## Contents

* install-disc: Installation CD including drivers
* olympus-mic-d-repair-manual.pdf: Obtained from http://www.alanwood.net/downloads/olympus-mic-d-repair-manual.pdf

## Driver details

Provided driver from the CD is 32-bit hence it will only work on 32-bit Windows. 

<img src="images/mic-d-in-device-manager.png" width="600">

It has been tested on 32-bit Windows 10. Simply install through Device Manager.

A video player like VLC can then be used to open the Capture Device.

The software in `setup.exe` is unnecessary as it seems like a Photo Album manager and I could not get it to work.

## Using in Linux

I tested this on Linux Mint 20 with this kernel without an additional driver required to be installed.

```bash
uname -a
Linux ... 5.4.0-74-generic #83-Ubuntu SMP Sat May 8 02:35:39 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux

lsusb 
...
Bus 001 Device 008: ID 05a9:a511 OmniVision Technologies, Inc. OV511+ Webcam
```

VLC manages to open this stream at `/dev/video0`.

