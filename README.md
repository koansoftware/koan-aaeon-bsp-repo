# Yocto Project setup for AAEON NVIDIA AI Solutions

![aaeon.com](https://www.aaeon.com/emgz/client_logo.png)

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

The build tree should be like the following _(reduced list)_.

```
yocto-aaeon-dunfell
├── README.md -> sources/meta-aaeonboxer/README.md
├── setup-environment -> sources/meta-aaeonboxer/scripts/setup-environment
└── sources
    ├── meta-aaeonboxer
    │    └── scripts
    │        ├── deploy-aaeon.sh
    │        └── setup-environment
    ├── meta-openembedded
    ├── meta-tegra
    └── poky
```

Please continue reading the documentation in the [meta-aaeonboxer README](https://github.com/koansoftware/meta-aaeonboxer)

![boxer-8221a](https://eshop.aaeon.com/media/catalog/product/cache/image/800x800/e9c3970ab036de70892d86c6d221abfe/b/o/boxer-8221ai_3d_front_600x600.jpg)


Contributing
-------
Please use GitHub (https://github.com/koansoftware/koan-aaeon-bsp-repo) to submit issues or pull requests, or add to the documentation on the wiki. Contributions are welcome!

------

(C)2020 Copyright - KOAN sas - <https://koansoftware.com>
