<p align="center"><img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimage.flaticon.com%2Ficons%2Fpng%2F512%2F518%2F518713.png&f=1&nofb=1"...></p>
<h1 align="center">
PS4 Linux Documentation
</h1>
<h2 align="center">
A complete documentation for Linux on the PlayStation 4
</h2>

------


# Download

### Kernel

| PS4       | Kernel     |
|--------------|-----------|
| FAT/Slim (Aeolia)  | [**4.14.93** (Most Stable - HDD Support)](https://mega.nz/file/EJhBzTIQ#rpbOcpIpulojUxRUiZjLQ7RqS6tlNc6JmcCrgSxyG-g) [**5.3.18** (BETA - Vulkan support - HDD Support)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImageAeolia) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support)](https://mega.nz/file/0wgETIxI#2nzITm4YokEQXAmm5_lHcPXKotlr3Tj1qbHutKS9BqA)|
| Slim/Fat (Belize) | [**4.14.93** (Most Stable - HDD Support) ](https://github.com/Nazky/ps4-linux/releases/download/4.19.93-belize/bzImage) [**5.3.18** (BETA - Vulkan support - HDD Support)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImage) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support)](https://mega.nz/file/0wgETIxI#2nzITm4YokEQXAmm5_lHcPXKotlr3Tj1qbHutKS9BqA) |
| Pro/Slim (Baikal) | [**4.14.93**(Most Stable - No HDD Support)](https://mega.nz/file/4FhBjbaS#zgy2TFTPN1fdWLyLZaJJBfIv2cZQOExdXvfYRVqIHNU) [**5.3.18** (BETA - Vulkan support - No HDD Support)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImageBaikal) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support)](https://mega.nz/file/Z1BywBxC#5HDoTE82zcaYdaCxlbuoNNzM4WJhdANriM0I4HEtmgs)  |

### Initramfs.cpio.gz

| Author       | Link     |
|--------------|-----------|
| [Psxita](https://www.psxita.it)  | [**MEGA**](https://mega.nz/file/IUBDiQKY#7WK2zFkUQbqJ02b9LTSAGug3NiL_8XPhprLcqVcfXxQ)
| [Hippie68](https://github.com/hippie68) | [**GitHub** ](https://github.com/hippie68/psxitarch-how-to/releases/tag/v1.00)
| [Nazky](https://twitter.com/NazkyYT) | [**MEGA**](https://mega.nz/file/E0wW3a6Y#IE9fvrjZ22Q2mJ6kM1uQaNctwj1-we4cV7xGqPBVV64) |

### Linux Distrubution

#### Prefab

| Author       | OS     |
|--------------|-----------|
| [Psxita](https://www.psxita.it) | [**Psxitarch**](https://www.psxita.it/distro/psxitarch.tar.xz)|
| [Mircoho](https://github.com/ps4gentoo)| [**Gentoo**](https://drive.google.com/uc?id=1o5zYErfHAeZnOR1beeN4syeuKW77VDjA&export=download) |
| [ItMania](https://www.youtube.com/channel/UCkVRqtCIS3Xj-E1HY4j9_EA)  | [**Fedora 32 Tron Edition**](https://drive.google.com/file/d/1bwTtP8mzlAp_mDbS1EnaMfpWrZ7gC4HV/view)
| [Modded Warfare](https://www.youtube.com/channel/UCm9COMxXKm05BQWNv-IpyPg) | [**Fedora 32** ](https://anonfiles.com/Tdi5B458x6/PS4_Fedora32_MW_Itm.tar_xz)
| [Nazky](https://twitter.com/NazkyYT) | [**CuteFish OS**](https://mega.nz/file/lhhFCAzK#IMCOCXHihX49zjOr6_tWVXeRZehI89o4HNTUASKLsJE) |

#### How to update Psxitarch ?

You can find a complete tuto [here](https://github.com/hippie68/psxitarch-how-to)

#### How to update Fedora ?

You can find a complete tuto [here](https://youtu.be/WgukYE-2vx4?t=1029)

#### How to update CuteFish OS ?

##### Using the terminal

```sudo pacman -Syyu```

##### Using Pamac

- Open the store (Add/remove software) app
- Go to "Update"
- Click on "Apply"
- Wait...
- It's update :D (you maybe have to restart the PS4)

#### How to make my own OS ?

What you need :

- A compatible OS
- A vm (virtual box, VMware, qemu, ...)
- The PS4 drivers [here](https://github.com/Hakkuraifu/PS4Linux-ArchDrivers)
- A little of knowledge

###### 1) The OS

You need a compatible OS, theoriclly all linux distrubution can be run on the PS4 if you have the drivers, since we only have the drivers for arch you need a arch based distro, i recommend Manjaro, 

