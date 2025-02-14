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
 - The Linux kernel is monolithic, meaning it operates in a single address space. It’s composed of several components: process management for executing processes, memory management for efficient memory allocation and use, device drivers for managing hardware interaction, system calls as interfaces for requesting services from the kernel, and file system management.
 - A Linux system is divided into three main parts:
   - **Hardware** - This includes all the hardware that your system runs on as well as memory, CPU, disks, etc.
   - **Linux Kernel** - As we discussed above, the kernel is the core of the operating system. It manages the hardware and tells it how to interact with the system.
   - **User Space** - This is where users like us will be directly interacting with the system.
![Linux-Architecture](https://github.com/user-attachments/assets/5d029620-9d08-40f6-9f10-d301c387a52e)

<details>
  <summary>Click to View LINUX ARCHITECTURE EXPLAINED</summary>
  
1. **Hardware**
   - The foundation of the Linux architecture, hardware includes physical components like the CPU, RAM, hard drive, motherboard, and peripherals. These components perform the actual computation, storage, and data processing. The hardware is the tangible layer where all operations ultimately execute.

2. **Kernel**
   - Sitting directly above the hardware, the kernel is the core of the Linux operating system. It acts as a bridge between the hardware and software layers. The kernel manages critical tasks like memory allocation, process scheduling, device communication (via drivers), and file system operations. It directly interacts with the hardware to execute low-level operations, ensuring efficient resource utilization and system stability. For example, when a program needs to read a file, the kernel handles the request by communicating with the storage hardware.

3. **Shell**
   - The shell is a command-line interface (CLI) or scripting environment that allows users to interact with the kernel. It acts as an intermediary, translating user commands into actions the kernel can execute. For instance, when you type a command like `ls` to list files, the shell interprets this command and sends a request to the kernel. The kernel then interacts with the hardware (e.g., the hard drive) to fetch the required data and returns the results to the shell, which displays them to the user. Popular shells like **bash**, **zsh**, and **csh** offer different features and scripting capabilities.

4. **Applications**
   - Applications are the software programs users interact with directly, such as web browsers, text editors, or file managers. These applications rely on the kernel to access hardware resources and the shell to execute commands or scripts. For example, when you open a file in a text editor, the application sends a request to the kernel via the shell. The kernel retrieves the file from the hardware (e.g., the hard drive) and passes it back to the application, which then displays it to the user.
  
</details>  

## Linux File Systems
- The Linux file system is a hierarchical structure that organizes data and files on a Linux-based operating system.

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
| /usr      | User-installed software and utilities, however, that is not to say you can't add personal directories in there. Inside this directory are sub-directories for `/usr/bin`, `/usr/local`, etc. |
| /var      | Variable directory, it's used for system logging, user tracking, caches, etc. Basically anything that is subject to change all the time. |

###  Common Desktop Filesystem Types
<details>
  <summary>Click to View Common Types of Desktop Filesystem</summary>
  
1. **ext4** - This is the most current version of the native Linux filesystems. It is compatible with the older ext2 and ext3 versions. It supports disk volumes up to 1 exabyte and file sizes up to 16 terabytes and much more. It is the standard choice for Linux filesystems.
2. **Btrfs - "Better or Butter FS"** it is a new filesystem for Linux that comes with snapshots, incremental backups, performance increase and much more. It is widely available, but not quite stable and compatible yet.
3. **XFS** - High performance journaling file system, great for a system with large files such as a media server.
4. **NTFS and FAT** - Windows filesystems
5. **HFS+** - Macintosh filesystem
</details>

- **Check out what filesystems are on your machine:**
  ```sh
  [root@rhel ~]# df -T
  ```
<details>
  <summary>Click to View Filesystem Information</summary>
  
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

### Anatomy of a Disk: 
- Hard disks can be subdivided into partitions, essentially making multiple block devices.
- Disks are divided into **partitions**, creating multiple block devices.  
  - Example: `/dev/sda` = whole disk, `/dev/sda1` = first partition.  
- Partitions help organize data and allow different filesystems on the same disk.  

<details>
  <summary>Output - Click to view Anatomy of Disk Explained</summary>
  
#### **1. Partition Table: The Disk's Blueprint**  
- Every disk has a **partition table** that maps out:  
  - Where partitions start and end.  
  - Which partitions are bootable.  
  - Which disk sectors belong to which partition.
  - You can have multiple partitions on a disk and they can't overlap each other. If there is space that is not allocated to a partition, then it is known as free space. 
- Two main types: **MBR** (old) and **GPT** (new).  


#### **2. MBR (Master Boot Record)**  
- **Old-school standard**.  
- Can have primary, extended, and logical partitions.
- Supports up to **4 primary partitions**.  
  - Need more? Convert one primary into an **extended partition** and add **logical partitions** inside it.  
- Limited to disks **up to 2TB**.  


#### **3. GPT (GUID Partition Table)**  
- **Modern standard**.  
- No partition type nonsense—just create as many partitions as you need.  
- Each partition gets a **globally unique ID (GUID)**.  
- Works best with **UEFI-based booting**.  

#### **4. Filesystem Structure: The Organized Chaos**  
A filesystem is more than just files and directories. Here's the breakdown:  

1. **Boot Block**:  
   - Located in the first few sectors of the file system.  
   - Contains bootloader info for the OS.  
   - Only one boot block is actively used, even if multiple partitions have them.  

2. **Super Block**:  
   - Single block after the boot block.  
   - Stores metadata about the filesystem:  
     - Size of the inode table.  
     - Size of logical blocks.  
     - Total size of the filesystem.  

3. **Inode Table**:  
   - The **database** of the filesystem that manages our files.  
   - Each file/directory has a unique **inode entry** containing metadata (permissions, size, location, etc.).  

4. **Data Blocks**:  
   - Where the actual **file data** and **directory structures** live.  

- **Check out Disk Partition on your machine:**
  ```sh
  [root@rhel ~]# parted -l
  ```
<details>
  <summary>Output - Click to view disk partition information</summary>
  
  ```sh
  [root@rhel ~]# parted -l
  Model: Xen Virtual Block Device (xvd)
  Disk /dev/xvda: 10.7GB
  Sector size (logical/physical): 512B/512B
  Partition Table: gpt
  Disk Flags:

  Number  Start   End     Size    File system  Name  Flags
   1      1049kB  2097kB  1049kB                     bios_grub
   2      2097kB  212MB   210MB   fat16              boot, esp
   3      212MB   1286MB  1074MB  xfs                bls_boot
   4      1286MB  10.7GB  9452MB  xfs

   ```
</details>
</details>

### Disk Partitioning & Creating a File System in the Partitioned Disk & Mount-UMount
- Disk partitioning is a critical task for managing storage devices.
- There are several tools available for disk partitioning, each with its own strengths:
  - **`fdisk`**: A basic command-line partitioning tool. It does **not** support GPT (GUID Partition Table).
  - **`parted`**: A versatile command-line tool that supports both MBR (Master Boot Record) and GPT partitioning.
  - **`gparted`**: The GUI version of `parted`, ideal for users who prefer a graphical interface.
  - **`gdisk`**: Similar to `fdisk`, but it **only supports GPT** (no MBR).
- Partitioning a disk is a straightforward process with the right tools. Using `parted`, you can:
1. Select the target device.
2. View the current partition table.
3. Create new partitions with specific start and end points.
4. Verify and save changes.

<details>
  <summary>Click to View Disk Partitioning: A Practical Guide with Executed Steps</summary>

  ### **Step 1: Launch `parted`**
Open your terminal and launch `parted` with root privileges:

```bash
$ sudo parted
```

**Output:**

```
GNU Parted 3.6
Using /dev/xvda
Welcome to GNU Parted! Type 'help' to view a list of commands.
(parted)
```

---

### **Step 3: View the Current Partition Table**
To inspect the current partition table, use the `print` command:

```bash
(parted) print
```

**Output:**

```
Model: Xen Virtual Block Device (xvd)
Disk /dev/xvda: 26.8GB
Sector size (logical/physical): 512B/512B
Partition Table: gpt
Disk Flags:

Number  Start   End     Size    File system  Name  Flags
14      1049kB  5243kB  4194kB                     bios_grub
15      5243kB  116MB   111MB   fat32              boot, esp
16      116MB   1074MB  957MB   ext4               bls_boot
 1      1075MB  26.8GB  25.8GB  ext4
```

- **Number**: Partition number.
- **Start/End**: Location of the partition on the disk.
- **File system**: File system format (e.g., ext4, fat32).
- **Flags**: Special attributes (e.g., `boot`, `esp`).

---

### **Step 4: Create a New Partition**
To create a new partition, use the `mkpart` command. For example, to create a primary partition from 123MB to 4567MB:

```bash
(parted) mkpart primary 123 4567
```

**Output:**

```
Warning: The resulting partition is not properly aligned for best performance: 2097153s % 2048s != 0s
Ignore/Cancel? Ignore
```

---

### **Step 5: Verify the New Partition**
After creating the partition, verify it by printing the partition table again:

```bash
(parted) print
```

**Output:**

```
Model: Xen Virtual Block Device (xvd)
Disk /dev/xvda: 26.8GB
Sector size (logical/physical): 512B/512B
Partition Table: gpt
Disk Flags:

Number  Start   End     Size    File system  Name  Flags
14      1049kB  5243kB  4194kB                     bios_grub
15      5243kB  116MB   111MB   fat32              boot, esp
16      116MB   1074MB  957MB   ext4               bls_boot
 2      1074MB  1075MB  1048kB               ext4
 1      1075MB  26.8GB  25.8GB  ext4
```

- **Partition 2**: The newly created partition (1074MB–1075MB).

---

### **Step 6: Exit `parted`**
Once you're done, exit the `parted` shell:

```bash
(parted) quit
```

**Output:**

```
Information: You may need to update /etc/fstab.
```

### **Step 7: Resize a Partition**
- You can also resize a partition if you don't have any space.
```bash
resize 2 1245 3456
```
- Select the partition number and then the start and end points of where you want to resize it to.

### **Creating A Filesystems**
- Command to make a file system in the partitioned disk
```bash
sudo mkfs -t ext4 /dev/xvda2
```
**Output:**
```
ubuntu@ip-172-31-3-50:~$ sudo mkfs -t ext4 /dev/xvda
mke2fs 1.47.0 (5-Feb-2023)
/dev/xvda is apparently in use by the system; will not make a filesystem here!
ubuntu@ip-172-31-3-50:~$ sudo mkfs -t ext4 /dev/xvda2
mke2fs 1.47.0 (5-Feb-2023)

Filesystem too small for a journal
Creating filesystem with 255 4k blocks and 128 inodes

Allocating group tables: done
Writing inode tables: done
Writing superblocks and filesystem accounting information: done
```
- Verify the file system
  ```bash
  ubuntu@ip-172-31-3-50:~$ sudo blkid /dev/xvda2
  /dev/xvda2: UUID="b628debc-4071-40f7-881d-0ac4060be819" BLOCK_SIZE="4096" TYPE="ext4" PARTLABEL="ext4" PARTUUID="51db5af8-4c7e-4814-8075-14f065161923"
  ```

## Mounting and Unmounting a Partitioned Disk
 We'll use the partition `/dev/xvda2` and mount it to `/home/ubuntu/mydrive`.

---

## **1. Create a Mount Point**

First, create a directory to serve as the mount point for the partition:

```bash
ubuntu@ip-172-31-3-50:~$ mkdir mydrive
```
---

## **2. Mount the Partition**

Mount the partition `/dev/xvda2` to the `mydrive` directory using the `mount` command:

```bash
ubuntu@ip-172-31-3-50:~$ sudo mount -t ext4 /dev/xvda2 /home/ubuntu/mydrive
```

**Explanation:**
- `sudo`: Run the command with root privileges.
- `mount`: Command to mount a file system.
- `-t ext4`: Specifies the file system type (`ext4` in this case).
- `/dev/xvda2`: The partition to mount.
- `/home/ubuntu/mydrive`: The mount point.

---

## **3. Verify the Mount**

To confirm that the partition has been successfully mounted, use the `blkid` and `findmnt` commands.

### **Check Partition Details with `blkid`:**

```bash
ubuntu@ip-172-31-3-50:~$ sudo blkid
```

**Output:**

```
/dev/xvda16: LABEL="BOOT" UUID="91942573-b0ea-4e42-8692-2a195de77cba" BLOCK_SIZE="4096" TYPE="ext4" PARTUUID="0f03bd19-c47e-4864-9884-634fc120fb03"
/dev/xvda1: LABEL="cloudimg-rootfs" UUID="104656f3-cbcd-4c1a-bbe2-5bb510be86c0" BLOCK_SIZE="4096" TYPE="ext4" PARTUUID="2bb9818b-3393-4017-8da7-c739e7b96eac"
/dev/xvda15: LABEL_FATBOOT="UEFI" LABEL="UEFI" UUID="534B-8AD0" BLOCK_SIZE="512" TYPE="vfat" PARTUUID="1179273d-96b8-4541-b634-ffe44e498cd0"
/dev/xvda2: UUID="b628debc-4071-40f7-881d-0ac4060be819" BLOCK_SIZE="4096" TYPE="ext4" PARTLABEL="ext4" PARTUUID="51db5af8-4c7e-4814-8075-14f065161923"
/dev/loop1: BLOCK_SIZE="131072" TYPE="squashfs"
/dev/xvda14: PARTUUID="5ec5cc0b-28cf-468c-a6e5-61c8f025ccc3"
/dev/loop2: BLOCK_SIZE="131072" TYPE="squashfs"
/dev/loop0: BLOCK_SIZE="131072" TYPE="squashfs"
```

- `/dev/xvda2` is confirmed to have an `ext4` file system.

### **Check Mounted File Systems with `findmnt`:**

```bash
ubuntu@ip-172-31-3-50:~$ findmnt
```

**Output:**

```
TARGET                SOURCE    FSTYPE   OPTIONS
/                     /dev/xvda1 ext4     rw,relatime,discard,errors=remount-ro,commit=30
...
└─/home/ubuntu/mydrive /dev/xvda2 ext4     rw,relatime
```

- `/dev/xvda2` is mounted at `/home/ubuntu/mydrive`.

---

## **4. Unmount the Partition**

When you're done using the partition, unmount it using the `umount` command:

```bash
ubuntu@ip-172-31-3-50:~$ sudo umount /home/ubuntu/mydrive
```

**Verify the Unmount:**

```bash
ubuntu@ip-172-31-3-50:~$ findmnt
```

**Output:**

```
TARGET                SOURCE    FSTYPE   OPTIONS
/                     /dev/xvda1 ext4     rw,relatime,discard,errors=remount-ro,commit=30
...
```

- The `/home/ubuntu/mydrive` entry is no longer listed, confirming that the partition has been unmounted.

---

## **5. Summary of Commands**

### **Mounting:**
1. Create a mount point:
   ```bash
   mkdir mydrive
   ```
2. Mount the partition:
   ```bash
   sudo mount -t ext4 /dev/xvda2 /home/ubuntu/mydrive
   ```
3. Verify the mount:
   ```bash
   sudo blkid
   findmnt
   ```

### **Unmounting:**
1. Unmount the partition:
   ```bash
   sudo umount /home/ubuntu/mydrive
   ```
2. Verify the unmount:
   ```bash
   findmnt
   ```
---

</details>

---
## init
The terms **Init** is Initialization where init acts as a **MOTHER OF ALL PROCESS & It has a Process ID (PID) of 1**, **System V**, **Upstart**, and **Systemd** are all related to the initialization and management of services and processes in Unix-like operating systems (e.g., Linux). They represent different generations of **init systems**, which are responsible for booting the system, starting services, and managing system states. 

<details>
  <summary>Click to check explanation of each, their differences, and their purposes.</summary>
  
### **1. Init (Initialization)**
- **What**: Init is the first process that starts when a Unix-like system boots. It has a Process ID (PID) of 1 and is responsible for starting and managing other processes and services.
- **How**: Init reads configuration files (like `/etc/inittab`) to determine which processes to start and in what order.
- **Why**: Init ensures that essential system services (e.g., networking, logging, etc.) are started during boot and manages system runlevels (system states).

---

### **2. System V Overview**
- **What**: System V (SysV) is one of the earliest and most widely used init systems. It is named after Unix System V, a version of Unix.
- **How**: It uses shell scripts located in `/etc/init.d/` or `/etc/rc.d/` to start and stop services. These scripts are executed in a specific order based on runlevels (e.g., runlevel 3 for multi-user mode, runlevel 5 for graphical mode).
- **Why**: System V provides a structured way to manage services and runlevels, but it is sequential and can be slow during boot.

---

### **3. System V Service**
- **What**: A service in System V is a program or daemon that runs in the background (e.g., a web server or database).
- **How**: Services are managed using scripts in `/etc/init.d/`. Commands like `service <name> start` or `/etc/init.d/<name> start` are used to control them.
- **Why**: Services are essential for running background processes that provide functionality to the system or users.

---

### **4. Upstart Overview**
- **What**: Upstart is an event-based replacement for System V init, developed by Canonical for Ubuntu.
- **How**: Instead of relying solely on runlevels, Upstart starts and stops services based on events (e.g., hardware changes, service dependencies).
- **Why**: Upstart was designed to address the limitations of System V, such as slow boot times and lack of flexibility in handling modern hardware (e.g., hot-pluggable devices).

---

### **5. Upstart Jobs**
- **What**: Jobs in Upstart are tasks or services that can be started, stopped, or restarted.
- **How**: Jobs are defined in configuration files located in `/etc/init/`. These files specify how and when a job should run (e.g., start on network-up).
- **Why**: Upstart jobs provide more flexibility and faster boot times compared to System V scripts.

---

### **6. Systemd Overview**
- **What**: Systemd is a modern init system and service manager that has largely replaced System V and Upstart in many Linux distributions.
- **How**: Systemd uses unit files (e.g., `.service`, `.socket`, `.target`) to define and manage services, sockets, mount points, and more. It parallelizes service startup for faster boot times.
- **Why**: Systemd was created to address the shortcomings of System V and Upstart, offering better performance, dependency management, and advanced features like logging (via `journald`).

---

### **7. Systemd Goals**
- **What**: The primary goals of Systemd are to improve boot performance, simplify service management, and provide a unified way to manage system resources.
- **How**: Systemd achieves these goals by:
  - Parallelizing service startup.
  - Using declarative unit files for configuration.
  - Providing tools like `systemctl` for service management.
  - Integrating with other system components (e.g., logging, device management).
- **Why**: Systemd aims to modernize Linux systems, making them more efficient and easier to manage.

---

### **8. Power States**
- **What**: Power states refer to the different modes a system can be in, such as running, sleeping, or powered off.
- **How**: Init systems manage power states by controlling which services are running and how the system transitions between states (e.g., shutdown, reboot, suspend).
- **Why**: Proper management of power states ensures that the system operates efficiently and data is not lost during transitions.

---
</details>

### **Differences Between Init Systems**
| Feature              | System V                          | Upstart                          | Systemd                          |
|----------------------|-----------------------------------|----------------------------------|----------------------------------|
| **Boot Process**      | Sequential, slow                 | Event-based, faster             | Parallelized, fastest           |
| **Configuration**     | Shell scripts in `/etc/init.d/`  | Job files in `/etc/init/`       | Unit files in `/etc/systemd/`   |
| **Dependency Handling** | Manual                          | Event-based                     | Automatic                       |
| **Logging**           | Separate (e.g., syslog)          | Separate                        | Integrated (`journald`)         |
| **Adoption**          | Older systems                   | Ubuntu (older versions)         | Most modern Linux distributions |

---

### **Summary**
- **System V**: The traditional init system, using sequential scripts and runlevels.
- **Upstart**: An event-based init system designed for faster boot times and flexibility.
- **Systemd**: The modern init system, offering parallelized startup, advanced dependency management, and integration with other system components.

Each system was developed to address the limitations of its predecessor, with Systemd being the most feature-rich and widely adopted in modern Linux distributions.
---
## **Basic Command Lines**
Learn the fundamentals of the command line, including navigating files, directories, and performing basic operations.

| **Topic**                  | **Command**                          | **Description**                                                                 | **Example**                                                                 |
|----------------------------|--------------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **1. The Shell**           | `bash`, `sh`, `zsh`                  | Start a shell session.                                                          | `bash` (starts a Bash shell).                                               |
| **2. pwd**                 | `pwd`                                | Print the current working directory.                                            | `pwd` (shows the current directory path).                                   |
| **3. cd**                  | `cd`                                 | Change the current directory.                                                   | `cd /home` (changes to the `/home` directory).                              |
| **4. ls**                  | `ls`                                 | List directory contents.                                                        | `ls -l` (lists files with details).                                         |
| **5. touch**               | `touch`                              | Create an empty file or update the timestamp of a file.                         | `touch file.txt` (creates or updates `file.txt`).                           |
| **6. file**                | `file`                               | Determine the type of a file.                                                   | `file file.txt` (shows the file type).                                      |
| **7. cat**                 | `cat`                                | Display the contents of a file.                                                 | `cat file.txt` (prints the contents of `file.txt`).                         |
| **8. less**                | `less`                               | View file contents interactively.                                               | `less file.txt` (opens `file.txt` in a pager).                              |
| **9. history**             | `history`                            | Display command history.                                                        | `history` (shows previously executed commands).                             |
| **10. cp**                 | `cp`                                 | Copy files or directories.                                                      | `cp file.txt /backup` (copies `file.txt` to `/backup`).                     |
| **11. mv**                 | `mv`                                 | Move or rename files or directories.                                            | `mv file.txt newname.txt` (renames `file.txt`).                             |
| **12. mkdir**              | `mkdir`                              | Create a new directory.                                                         | `mkdir newdir` (creates a directory named `newdir`).                        |
| **13. rm**                 | `rm`                                 | Remove files or directories.                                                    | `rm file.txt` (deletes `file.txt`).                                         |
| **14. find**               | `find`                               | Search for files or directories.                                                | `find /home -name "*.txt"` (finds `.txt` files in `/home`).                |
| **15. help**               | `help`                               | Display help for shell built-in commands.                                       | `help cd` (shows help for the `cd` command).                                |
| **16. man**                | `man`                                | Display the manual page for a command.                                          | `man ls` (shows the manual for `ls`).                                       |
| **17. whatis**             | `whatis`                             | Display a brief description of a command.                                       | `whatis ls` (shows a one-line description of `ls`).                         |
| **18. alias**              | `alias`                              | Create a shortcut for a command.                                                | `alias ll='ls -la'` (creates an alias for `ls -la`).                        |
| **19. exit**               | `exit`                               | Exit the shell or terminal.                                                     | `exit` (closes the terminal).

---
## **Text Manipulation and Navigation**
Basic text manipulation and navigation using command-line tools. These commands helps in process, filter, and transform text data efficiently.

**Commands and Examples**

| **Topic**                  | **Command**                          | **Description**                                                                 | **Example**                                                                 |
|----------------------------|--------------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **1. stdout**              | `>`                                  | Redirect standard output to a file.                                             | `ls > output.txt` (saves `ls` output to `output.txt`).                      |
| **2. stdin**               | `<`                                  | Redirect standard input from a file.                                            | `sort < input.txt` (sorts the contents of `input.txt`).                     |
| **3. stderr**              | `2>`                                 | Redirect standard error to a file.                                             | `ls /nonexistent 2> error.txt` (saves errors to `error.txt`).               |
| **4. pipe and tee**        | `|`, `tee`                           | Pipe output to another command or file.                                         | `ls | grep txt` (finds files containing `txt`).                                 |
| **5. env**                 | `env`                                | Display environment variables.                                                  | `env` (shows all environment variables).                                    |
| **6. cut**                 | `cut`                                | Extract specific columns or fields from text.                                   | `cut -d: -f1 /etc/passwd` (extracts usernames from `/etc/passwd`).          |
| **7. paste**               | `paste`                              | Merge lines of files.                                                           | `paste file1.txt file2.txt` (merges lines from two files).                  |
| **8. head**                | `head`                               | Display the first few lines of a file.                                          | `head -n 5 file.txt` (shows the first 5 lines of `file.txt`).               |
| **9. tail**                | `tail`                               | Display the last few lines of a file.                                           | `tail -n 5 file.txt` (shows the last 5 lines of `file.txt`).                |
| **10. expand and unexpand**| `expand`, `unexpand`                 | Convert tabs to spaces and vice versa.                                          | `expand file.txt` (converts tabs to spaces).                                |
| **11. join and split**     | `join`, `split`                      | Combine or split files.                                                         | `split -l 100 file.txt` (splits `file.txt` into 100-line chunks).           |
| **12. sort**               | `sort`                               | Sort lines of text.                                                             | `sort file.txt` (sorts the contents of `file.txt`).                         |
| **13. tr**                 | `tr`                                 | Translate or delete characters.                                                 | `tr 'a-z' 'A-Z' < file.txt` (converts lowercase to uppercase).              |
| **14. uniq**               | `uniq`                               | Remove duplicate lines from sorted text.                                        | `uniq file.txt` (removes duplicate lines).                                  |
| **15. wc and nl**          | `wc`, `nl`                           | Count lines, words, and characters or number lines.                             | `wc -l file.txt` (counts lines in `file.txt`).                              |
| **16. grep**               | `grep`                               | Search for patterns in text.                                                    | `grep "error" log.txt` (finds lines containing `error`).                    |

---

## Filesystem Basic Commands

| **Topic**                  | **Command**                          | **Description**                                                                 | **Example**                                                                 |
|----------------------------|--------------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **1. Filesystem Hierarchy** | `ls`                                 | List directory contents.                                                       | `ls /` (lists root directory contents).                                     |
|                            | `tree`                               | Display directory structure in a tree format.                                  | `tree /home` (shows the directory tree for `/home`).                        |
| **2. Filesystem Types**     | `df -T`                              | Display filesystem type along with disk usage.                                 | `df -T /` (shows filesystem type for the root partition).                   |
|                            | `lsblk -f`                           | List block devices with filesystem information.                                | `lsblk -f` (displays filesystem types for all partitions).                  |
| **3. Anatomy of a Disk**    | `lsblk`                              | List block devices (disks and partitions).                                     | `lsblk` (shows disk and partition layout).                                  |
|                            | `fdisk -l`                           | List disk partitions.                                                          | `fdisk -l /dev/sda` (displays partition table for `/dev/sda`).              |
| **4. Disk Partitioning**    | `fdisk`                              | Interactive disk partitioning tool.                                            | `fdisk /dev/sda` (starts partitioning `/dev/sda`).                          |
|                            | `parted`                             | Another partitioning tool with more features.                                 | `parted /dev/sda` (starts partitioning with `parted`).                      |
|                            | `gdisk`                              | GPT partitioning tool.                                                         | `gdisk /dev/sda` (for GPT disks).                                           |
| **5. Creating Filesystems** | `mkfs`                               | Create a filesystem.                                                           | `mkfs.ext4 /dev/sda1` (creates an ext4 filesystem on `/dev/sda1`).          |
|                            | `mkswap`                             | Create a swap partition.                                                       | `mkswap /dev/sda2` (initializes `/dev/sda2` as swap).                       |
| **6. mount and umount**     | `mount`                              | Mount a filesystem.                                                            | `mount /dev/sda1 /mnt` (mounts `/dev/sda1` to `/mnt`).                      |
|                            | `umount`                             | Unmount a filesystem.                                                          | `umount /mnt` (unmounts the filesystem mounted at `/mnt`).                  |
| **7. /etc/fstab**           | `blkid`                              | Get UUID of a partition.                                                       | `blkid /dev/sda1` (displays UUID for `/dev/sda1`).                          |
|                            | `nano /etc/fstab`                    | Edit the filesystem table.                                                     | `nano /etc/fstab` (opens `/etc/fstab` for editing).                         |
| **8. swap**                 | `swapon`                             | Enable a swap partition.                                                       | `swapon /dev/sda2` (enables swap on `/dev/sda2`).                           |
|                            | `swapoff`                            | Disable a swap partition.                                                      | `swapoff /dev/sda2` (disables swap on `/dev/sda2`).                         |
|                            | `free -h`                            | Check swap usage.                                                              | `free -h` (shows memory and swap usage).                                    |
| **9. Disk Usage**           | `df`                                 | Display disk space usage.                                                      | `df -h` (shows disk usage in human-readable format).                        |
|                            | `du`                                 | Estimate file space usage.                                                     | `du -sh /home` (shows total size of `/home` directory).                     |
| **10. Filesystem Repair**   | `fsck`                               | Check and repair a filesystem.                                                 | `fsck /dev/sda1` (checks and repairs `/dev/sda1`).                          |
|                            | `e2fsck`                             | Specifically for ext2/ext3/ext4 filesystems.                                   | `e2fsck /dev/sda1` (checks ext filesystems).                                |
| **11. Inodes**              | `df -i`                              | Display inode usage.                                                           | `df -i /` (shows inode usage for the root filesystem).                      |
|                            | `ls -i`                              | Display inode numbers of files.                                                | `ls -i /home` (lists files with their inode numbers).                       |
| **12. symlinks**            | `ln -s`                              | Create a symbolic link.                                                        | `ln -s /path/to/file /path/to/symlink` (creates a symlink).                 |
|                            | `readlink`                           | Display the target of a symlink.                                               | `readlink /path/to/symlink` (shows where the symlink points).               |
|                            | `ls -l`                              | List files and show symlinks.                                                  | `ls -l /path/to/dir` (shows symlinks with their targets).                   |

---
## User Management Commands
| **Topic**                  | **Command**                          | **Description**                                                                 | **Example**                                                                 |
|----------------------------|--------------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **1. Users and Groups**     | `id`                                 | Display user and group information.                                             | `id username` (shows UID, GID, and groups).                                 |
|                            | `groups`                             | List groups a user belongs to.                                                  | `groups username` (lists groups for the user).                              |
|                            | `whoami`                             | Display the current logged-in user.                                             | `whoami` (shows the current user).                                          |
| **2. root**                 | `sudo`                               | Execute a command as the superuser (root).                                      | `sudo apt update` (runs the command with root privileges).                  |
|                            | `su`                                 | Switch to another user (default is root).                                       | `su -` (switches to the root user).                                         |
|                            | `sudo -i`                            | Start a root shell.                                                             | `sudo -i` (opens a root shell).                                             |
| **3. /etc/passwd**          | `cat /etc/passwd`                    | Display the contents of `/etc/passwd`.                                          | `cat /etc/passwd` (lists all users and their details).                      |
|                            | `grep`                               | Search for a specific user in `/etc/passwd`.                                    | `grep username /etc/passwd` (shows details for the user).                   |
| **4. /etc/shadow**          | `sudo cat /etc/shadow`               | Display the contents of `/etc/shadow`.                                          | `sudo cat /etc/shadow` (shows encrypted passwords).                         |
|                            | `sudo grep`                          | Search for a specific user in `/etc/shadow`.                                    | `sudo grep username /etc/shadow` (shows password details).                  |
| **5. /etc/group**           | `cat /etc/group`                     | Display the contents of `/etc/group`.                                           | `cat /etc/group` (lists all groups and their members).                      |
|                            | `grep`                               | Search for a specific group in `/etc/group`.                                    | `grep groupname /etc/group` (shows details for the group).                  |
| **6. User Management Tools**| `useradd`                            | Add a new user.                                                                 | `sudo useradd username` (creates a new user).                               |
|                            | `usermod`                            | Modify user properties.                                                         | `sudo usermod -aG groupname username` (adds user to a group).               |
|                            | `userdel`                            | Delete a user.                                                                  | `sudo userdel username` (deletes a user).                                   |
|                            | `passwd`                             | Change a user's password.                                                       | `sudo passwd username` (sets or changes a user's password).                 |
|                            | `groupadd`                           | Add a new group.                                                                | `sudo groupadd groupname` (creates a new group).                            |
|                            | `groupmod`                           | Modify group properties.                                                        | `sudo groupmod -n newgroupname oldgroupname` (renames a group).             |
|                            | `groupdel`                           | Delete a group.                                                                 | `sudo groupdel groupname` (deletes a group).                                |
|                            | `chage`                              | Change user password expiry information.                                        | `sudo chage -l username` (lists password expiry details).                   |

---





