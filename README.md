![KoanSoftware.com](http://koansoftware.com/pub/img/koan-header.png)

(C)2020 Copyright - KOAN sas - <https://koansoftware.com>

# koan-aaeon-bsp-repo

BSP Yocto layer for AAEON Boxer - Start here to create the Yocto build environment 

Koan BSP for AAEON Boxer - Yocto Project 3.1 'dunfell' LTS
------------

To get the BSP you need to have `repo` installed and use it as:

Install the `repo` utility:

```
$: mkdir ~/bin
$: curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$: chmod a+x ~/bin/repo
```

Download the BSP source:

```
$: PATH=${PATH}:~/bin
$: mkdir yocto-aaeon-dunfell
$: cd yocto-aaeon-dunfell
$: repo init -b dunfell -u https://github.com/koansoftware/koan-aaeon-bsp-repo
$: repo sync
```

At the end of the commands you have every metadata you need to start work with.

To start a simple image build:

```
$: MACHINE=jetson-nano-qspi-sd DISTRO=poky source setup-environment build
$: bitbake core-image-minimal
```

You can use any directory to host your build.

Contributing
------------

Please use GitHub (https://github.com/koansoftware/koan-aaeon-bsp-repo) to submit issues or pull requests, or add to the documentation on the wiki. Contributions are welcome!
