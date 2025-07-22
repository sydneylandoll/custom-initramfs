# Custom initramfs project

A minimal initramfs written from scratch in shell.

## Directory layout
```
├── bin
├── dev
├── etc
├── mnt
│   └── root
├── proc
├── root
├── sbin
└── sys
```

## License
GPLv3 -- see the [LICENSE](./LICENSE) file

## Note
This *should* boot any distro (doesn't have to be a full distro) that contains an init system and an ext4 filesystem. It has only been tested with Arch Linux so far though. You can use QEMU to test this. First you must use cpio to create the file archive.

## Requirements
- Virtual/physical disk image with:
  - ext4 filesystem
  - init system (located in /sbin/init)
- Linux kernel image
- bootloader
