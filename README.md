# My-attempt-for-linux-from-Scratch
It is me trying linux from scratch to learn something new
## Here is my Motivation

## Let's talk how first I setup
Here I followed simple verison requirment for the apps metioned in LFS here are commands for you for easy run
```
    sudo apt install bash
    sudo apt install binutils
    sudo apt install coreutils
    sudo apt install diffutils
    sudo apt install findutils
    sudo apt install gawk
    sudo apt install gcc
    sudo apt install grep
    sudo apt install gzip

```
```
    sudo apt upgrade bash
    sudo apt upgrade binutils
    sudo apt upgrade coreutils
    sudo apt upgrade diffutils
    sudo apt upgrade findutils
    sudo apt upgrade gawk
    sudo apt upgrade gcc
    sudo apt upgrade grep
    sudo apt upgrade gzip

```
Refer to recent documentaiton to know the mimimun requirements and do follow them.



## Theory
#### Root
Root is the superuser account in Unix and Linux. It is a user account for administrative purposes, and typically has the highest access rights on the system.
### Super user
In Linux and Unix-like systems, the superuser account, called 'root', is virtually omnipotent, with unrestricted access to all commands, files, directories, and resources. 
### Partion
A partition is a logical division of a hard disk that is treated as a separate unit by operating systems (OSes) and file systems. 
### Swap space
Swap space in Linux is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space.



## Step by step Porcedure

### Pariton needed
Most of you if you are using SSD as your storage devices then you might not need the Swap space. 30GB is what I am going with for this project.
I have curretnly created onw ith ext-4 as file system using G-parted.

now let's set up LFS Variable,
first know of the drive you are using let it's name be here name of my partiton is nvme0n1p8
feel free to replace the name with one your drive is.

```
mkdir -pv $LFS

mount -v -t ext4 /dev/nvme0n1p8 $LFS
```
let's get necessary reosurces

```
mkdir -v $LFS/sources
```