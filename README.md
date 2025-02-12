# Linux
Linux is an open-source operating system (OS) that's used in many industries and devices. It's similar to UNIX and is an alternative to proprietary operating systems like Microsoft Windows and macOS. 

## OS
- It is a type of software interface to establish communication between user and computer hardware devices. It allows user to communicate with devices and to perform desired functions. It performs all the basic tasks like file management, memory management, process management, handling input and output, and controlling peripheral devices such as disk drives and printers.
- The primary purposes of an Operating System are to enable applications (Software’s) to interact with a computer’s hardware and to manage a system’s hardware and software resources.

## Linux distribution
- A Linux distribution (also called as Linux distro) is a collection of software that is based upon the Linux kernel. It includes GNU tools, kernel, software modules, X-server, shell utilities, an installer, and it often as a package management system. It is an Open-source project where all the programmers are combined together and make some changes in the Linux kernel by compiling the codes and make it as a new Distros.
- Famous Linux distribution are: ubuntu, fedora, RedHat Enterprise Linux (RHEL), Arch Linux, Chrome OS and Debian.
- **RedHat Package Manager**
  - _RedHat Enterprise Linux (RHEL)_
  - _fedora_ -- **Upstream of RHEL, RHEL gets update from fedora after thorugh testing $ quality assurance.**
  - _open SUSE_
- **Debian Package Manager**
  - _Debian_
  - _ubuntu_
  - _Linux Mint_ -- **Less Bloated & Less distro than Ubuntu.**

 ## Linux Architecture
 - A Linux system is divided into three main parts:
   - **Hardware** - This includes all the hardware that your system runs on as well as memory, CPU, disks, etc.
   - **Linux Kernel** - As we discussed above, the kernel is the core of the operating system. It manages the hardware and tells it how to interact with the system.
   - **User Space** - This is where users like us will be directly interacting with the system.
![Linux-Architecture](https://github.com/user-attachments/assets/5d029620-9d08-40f6-9f10-d301c387a52e)

1. **Hardware**
   - The foundation of the Linux architecture, hardware includes physical components like the CPU, RAM, hard drive, motherboard, and peripherals. These components perform the actual computation, storage, and data processing. The hardware is the tangible layer where all operations ultimately execute.

2. **Kernel**
   - Sitting directly above the hardware, the kernel is the core of the Linux operating system. It acts as a bridge between the hardware and software layers. The kernel manages critical tasks like memory allocation, process scheduling, device communication (via drivers), and file system operations. It directly interacts with the hardware to execute low-level operations, ensuring efficient resource utilization and system stability. For example, when a program needs to read a file, the kernel handles the request by communicating with the storage hardware.

3. **Shell**
   - The shell is a command-line interface (CLI) or scripting environment that allows users to interact with the kernel. It acts as an intermediary, translating user commands into actions the kernel can execute. For instance, when you type a command like `ls` to list files, the shell interprets this command and sends a request to the kernel. The kernel then interacts with the hardware (e.g., the hard drive) to fetch the required data and returns the results to the shell, which displays them to the user. Popular shells like **bash**, **zsh**, and **csh** offer different features and scripting capabilities.

4. **Applications**
   - Applications are the software programs users interact with directly, such as web browsers, text editors, or file managers. These applications rely on the kernel to access hardware resources and the shell to execute commands or scripts. For example, when you open a file in a text editor, the application sends a request to the kernel via the shell. The kernel retrieves the file from the hardware (e.g., the hard drive) and passes it back to the application, which then displays it to the user.

## Linux File System
- The Linux file system is a hierarchical structure that organizes data and files on a Linux-based operating system.
  
## Linux File Systems

| Directory | Description |
|-----------|-------------|
| /         | The root directory of the entire filesystem hierarchy, everything is nestled under this directory. |
| /bin      | Essential ready-to-run programs (binaries), includes the most basic commands such as `ls` and `cp`. |
| /boot     | Contains kernel boot loader files. |
| /dev      | Device files. |
| /etc      | Core system configuration directory, should hold only configuration files and not any binaries. |
| /home     | Personal directories for users, holds your documents, files, settings, etc. |
| /lib      | Holds library files that binaries can use. |
| /media    | Used as an attachment point for removable media like USB drives. |
| /mnt      | Temporarily mounted filesystems. |
| /opt      | Optional application software packages. |
| /proc     | Information about currently running processes. |
| /root     | The root user's home directory. |
| /run      | Information about the running system since the last boot. |
| /sbin     | Contains essential system binaries, usually can only be run by root. |
| /srv      | Site-specific data which are served by the system. |
| /tmp      | Storage for temporary files. |
| /usr      | This is unfortunately named, most often it does not contain user files in the sense of a home folder. This is meant for user-installed software and utilities, however, that is not to say you can't add personal directories in there. Inside this directory are sub-directories for `/usr/bin`, `/usr/local`, etc. |
| /var      | Variable directory, it's used for system logging, user tracking, caches, etc. Basically anything that is subject to change all the time. |

###  Common Desktop Filesystem Types
1. **ext4** - This is the most current version of the native Linux filesystems. It is compatible with the older ext2 and ext3 versions. It supports disk volumes up to 1 exabyte and file sizes up to 16 terabytes and much more. It is the standard choice for Linux filesystems.
2. **Btrfs - "Better or Butter FS"** it is a new filesystem for Linux that comes with snapshots, incremental backups, performance increase and much more. It is widely available, but not quite stable and compatible yet.
3. **XFS** - High performance journaling file system, great for a system with large files such as a media server.
4. **NTFS and FAT** - Windows filesystems
5. **HFS+** - Macintosh filesystem
- **Check out what filesystems are on your machine:**
  ```sh
  [root@rhel ~]# df -T
  ```
<details>
  <summary>Output - Click to view filesystem information</summary>
  
  ```sh
  [root@rhel ~]# df -T
  Filesystem     Type     1K-blocks    Used Available Use% Mounted on
  devtmpfs       devtmpfs      4096       0      4096   0% /dev
  tmpfs          tmpfs       391472       0    391472   0% /dev/shm
  tmpfs          tmpfs       156592    8892    147700   6% /run
  /dev/xvda4     xfs        9164780 2651652   6513128  29% /
  /dev/xvda3     xfs         983040  274096    708944  28% /boot
  /dev/xvda2     vfat        204580    7196    197384   4% /boot/efi
  tmpfs          tmpfs        78292       4     78288   1% /run/user/1000
  ```
</details>

