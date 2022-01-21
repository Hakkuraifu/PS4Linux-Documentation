<p align="center"><img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimage.flaticon.com%2Ficons%2Fpng%2F512%2F518%2F518713.png&f=1&nofb=1"...></p>
<h1 align="center">
PS4 Linux Documentation
</h1>
<h2 align="center">
A complete documentation for Linux on the PlayStation 4
</h2>

------

# What you need.

## Files.

### Kernel.

| PS4       | Kernel     |
|--------------|-----------|
| FAT (Aeolia)  | [**4.14.93** (Most Stable - HDD Support - By Psxita)](https://mega.nz/file/EJhBzTIQ#rpbOcpIpulojUxRUiZjLQ7RqS6tlNc6JmcCrgSxyG-g) [**5.3.18** (BETA - Vulkan support - HDD Support - By Mircoho)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImageAeolia) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support - by codedwrench)](https://mega.nz/file/0wgETIxI#2nzITm4YokEQXAmm5_lHcPXKotlr3Tj1qbHutKS9BqA)|
| Slim/Fat (Belize) | [**4.14.93** (Most Stable - HDD Support - By tihmstar)](https://github.com/Nazky/ps4-linux/releases/download/4.19.93-belize/bzImage) [**5.3.18** (BETA - Vulkan support - HDD Support - By Mircoho)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImage) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support - by codedwrench))](https://mega.nz/file/0wgETIxI#2nzITm4YokEQXAmm5_lHcPXKotlr3Tj1qbHutKS9BqA) |
| Pro/Slim (Baikal) | [**4.14.93** (Most Stable - HDD Support - By Psxita)](https://mega.nz/file/4FhBjbaS#zgy2TFTPN1fdWLyLZaJJBfIv2cZQOExdXvfYRVqIHNU) [**5.3.18** (BETA - Vulkan support - No HDD Support - By Mircoho)](https://github.com/ps4boot/ps4-linux/releases/download/v1/bzImageBaikal) [**5.15.12** (ALPHA - NO STABLE - Vulkan support - No HDD Support - by codedwrench)](https://mega.nz/file/Z1BywBxC#5HDoTE82zcaYdaCxlbuoNNzM4WJhdANriM0I4HEtmgs)  |

### Initramfs.cpio.gz.

| Author       | Link     |
|--------------|-----------|
| [Psxita](https://www.psxita.it)  | [**MEGA**](https://mega.nz/file/IUBDiQKY#7WK2zFkUQbqJ02b9LTSAGug3NiL_8XPhprLcqVcfXxQ)
| [Hippie68](https://github.com/hippie68) | [**GitHub** ](https://github.com/hippie68/psxitarch-how-to/releases/tag/v1.00)
| [Nazky](https://twitter.com/NazkyYT) | [**MEGA**](https://mega.nz/file/E0wW3a6Y#IE9fvrjZ22Q2mJ6kM1uQaNctwj1-we4cV7xGqPBVV64) |

## Linux Distrubution.

### Prefab.

| Author       | OS     |
|--------------|-----------|
| [Psxita](https://www.psxita.it) | [**Psxitarch**](https://www.psxita.it/distro/psxitarch.tar.xz)|
| [Mircoho](https://github.com/ps4gentoo)| [**Gentoo**](https://drive.google.com/uc?id=1o5zYErfHAeZnOR1beeN4syeuKW77VDjA&export=download) |
| [ItMania](https://www.youtube.com/channel/UCkVRqtCIS3Xj-E1HY4j9_EA)  | [**Fedora 32 Tron Edition**](https://drive.google.com/file/d/1bwTtP8mzlAp_mDbS1EnaMfpWrZ7gC4HV/view)
| [Modded Warfare](https://www.youtube.com/channel/UCm9COMxXKm05BQWNv-IpyPg) | [**Fedora 32** ](https://anonfiles.com/Tdi5B458x6/PS4_Fedora32_MW_Itm.tar_xz)
| [Nazky](https://twitter.com/NazkyYT) | [**CuteFish OS**](https://mega.nz/file/lhhFCAzK#IMCOCXHihX49zjOr6_tWVXeRZehI89o4HNTUASKLsJE) |

### How to update Psxitarch ?

You can find a complete tuto [here](https://github.com/hippie68/psxitarch-how-to).

### How to update Fedora ?

You can find a complete tuto [here](https://youtu.be/WgukYE-2vx4?t=1029).

### How to update CuteFish OS ?

##### Using the terminal

```sudo pacman -Syyu```

It's update :D (you maybe have to restart the PS4).

##### Using Pamac

- Open the store (Add/remove software) app.
- Go to "Update".
- Click on "Apply".
- Wait...
- It's update :D (you maybe have to restart the PS4).

## How to make my own OS ?

What you need :

- A compatible OS.
- A vm (virtual box, VMware, qemu, ...) or a PC/Laptop.
- The PS4 drivers [here](https://github.com/Hakkuraifu/PS4Linux-ArchDrivers).
- A brain :p.

#### 1) The OS.

You need a compatible OS, theoriclly all linux distrubution can be run on the PS4 if you have the drivers, since we only have the drivers for arch you need a arch based distro, i recommend Manjaro but you can try any others.

#### 2) Installing PS4 drivers Using precompiled drivers.

After installing the OS on a vm (or a real PC/Laptop) you need to add the PS4Xploit repo.

```sudo echo -e "\n[ps4xploit-repo-arch]\nSigLevel = Optional TrustAll\nServer = https://PS4Xploit.zd.lu/Linux/Repo/x86_64" >> /etc/pacman.conf```

Then update the repos.

```sudo pacman -Syyu```

And install the drivers.

```sudo pacman -Syy mesa-ps4 lib32-libdrm-ps4 lib32-mesa-ps4 libdrm-ps4 xf86-video-amdgpu-ps4```

(if you want to compile the driver locally take a look [here](https://github.com/Hakkuraifu/PS4Linux-ArchDrivers#how-i-install-the-drivers-), it's also recommended to use "Auto-Login")

#### 3) Backup the OS.

After installing the drivers and customized the OS like you want you can now backup the OS to be able to install it on the PS4.

First it's recommended to go to the root folder.

```cd /```

Now you can backup the OS (you maybe have to change the command depending of the OS you use).

(Reaplce 'DistroName' by the name of you'r distro).

```sudo tar -cvf DistroName.tar.xz --exclude=/DistroName.tar.xz --exclude=/var/cache --one-file-system / -I "xz -9"```

 MAX SIZE <=3.2GB.


#### 4) Installing the OS.

⚠️ USE A >=16GB USB 3.0 DEVICE !!!!!!!!!!!!!!!!!!!!!! ⚠️

- Format the USB 3.0 Device to fat32 (you can use [this software](http://ridgecrop.co.uk/index.htm?guiformat.htm)).

- Put the bzimage, the initramfs.cpio.gz and the OS in the root of the USB 3.0 Device.

- Rename the OS to 'psxitarch.tar.xz' (if you use the initramfs.cpio.gz from Nazky rename the os to arch.tar.xz).

- Launch the 1GB Linux payload using one of the trusted host in the list below.

- When rescushell start run ```exec install-psxitarch.sh``` (if you use the initramfs.cpio.gz from Nazky run ```exec install-arch.sh```) and wait.

- When the installation is done the OS is going to boot automaticlly, if the OS not boot run ```exec start-psxitarch.sh``` (if you use the initramfs.cpio.gz from Nazky run ```exec start-arch.sh```) and wait (you need to run```exec start-arch.sh``` twice everytime you reboot the OS).

#### Optional - Installing the OS on the HDD.

⚠️ USE A COMPATIBLE PS4 !!!!!!!!!!!!!!!!!!!!!! ⚠️

- Use a FTP Client and transfert the bzimage, the initramfs.cpio.gz from Nazky and the OS to /usr/system/boot.
- Run any Linux GB using one of the trusted host in the list below. 
- When rescushell start run ```exec install-HDD.sh``` and set how many GB you want to give to linux.
- Wait..
- When the installation is done the os is going to boot automaticlly, if the OS not boot press **CTRL + D** or run ```exec start-arch.sh```.

#### Optional - Unistalling.

To unistalling a OS install on a USB Device just format the USB Device.

#### Optional - Unistalling the OS on the HDD.
To unistalling a OS install on the HDD just delete the **Arch.img** file in /usr/home.

## Trust host to use.

This list can change in the futur.

- http://ps4xploit.zd.lu | by [Nazky](https://twitter.com/NazkyYT)
- http://kmeps4.site | By [Kameleon](https://twitter.com/KameleonRe)
- http://prb123.ir | By [PRB](https://twitter.com/Prb29327239)


## Little F.A.Q

### I have a black screen 
It's a 'bug' in the 5.x kernel you need to refresh the HDMI the most easy way it's to wait until you get no signal then moved the mouse or pressed a key on the keyboard.

### I still have a black screen even with the kernel 4.14
Make sure you'r display is compatible with the 1080p resolution, if you still have a black screen try a others monitor.

### I don't have WIFI or BT
This can be caused by the kernel or the distro, not real fix here use a wifi or/and a bt dongle.

### Some apps not launch why ?
FlatPak apps seems to have some problems with the ps4, and Snaps apps is not working, not real fix here use AUR.

### I can't use my controller as a mouse why ?
Some distro don't have ds4drv preinstall (Cutefish for the exemple here) use the store (pamac) to install ds4drv (it's recommend to install the motion control one) then open a terminal, connect you'r ds4 in usb and run  ```ds4drv --hidraw ```.
