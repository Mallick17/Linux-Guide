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
  - _fedora_ -- **Upstream of RHEL, RHEL gets update from fedora after thorugh testing & quality assurance.**
  - _open SUSE_
- **Debian Package Manager**
  - _Debian_
  - _ubuntu_
  - _Linux Mint_ -- **Less Bloated & Less distro than Ubuntu.**

 ## Linux Architecture
 - The Linux kernel is monolithic, meaning it operates in a single address space. It’s composed of several components: process management for executing processes, memory management for efficient memory allocation and use, device drivers for managing hardware interaction, system calls as interfaces for requesting services from the kernel, and file system management.
 - A Linux system is divided into three main parts:
   - **Hardware** - This includes all the hardware that our system runs on as well as memory, CPU, disks, etc.
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
   - The shell is a command-line interface (CLI) or scripting environment that allows users to interact with the kernel. It acts as an intermediary, translating user commands into actions the kernel can execute. For instance, when we type a command like `ls` to list files, the shell interprets this command and sends a request to the kernel. The kernel then interacts with the hardware (e.g., the hard drive) to fetch the required data and returns the results to the shell, which displays them to the user. Popular shells like **bash**, **zsh**, and **csh** offer different features and scripting capabilities.

4. **Applications**
   - Applications are the software programs users interact with directly, such as web browsers, text editors, or file managers. These applications rely on the kernel to access hardware resources and the shell to execute commands or scripts. For example, when we open a file in a text editor, the application sends a request to the kernel via the shell. The kernel retrieves the file from the hardware (e.g., the hard drive) and passes it back to the application, which then displays it to the user.
  
</details>

---

## **Basic Command Lines**

<details>
  <summary>Click to Find the fundamentals of the command line, including navigating files, directories, and performing basic operations.</summary>

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


</details>

---

## **Text Manipulation and Navigation Commands**

<details>
  <summary>Click to Find Basic text manipulation and navigation using command-line tools. These commands helps in process, filter, and transform text data efficiently.</summary>

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

</details>

---

## Linux File Systems
- The Linux file system is a hierarchical structure that organizes data and files on a Linux-based operating system.

| Directory | Description |
|-----------|-------------|
| /         | The root directory of the entire filesystem hierarchy, everything is nestled under this directory. |
| /bin      | Essential ready-to-run programs (binaries), includes the most basic commands such as `ls` and `cp`. |
| /boot     | Contains kernel boot loader files. |
| /dev      | Device files. |
| /etc      | Core system configuration directory, should hold only configuration files and not any binaries. |
| /home     | Personal directories for users, holds our documents, files, settings, etc. |
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
| /usr      | User-installed software and utilities, however, that is not to say we can't add personal directories in there. Inside this directory are sub-directories for `/usr/bin`, `/usr/local`, etc. |
| /var      | Variable directory, it's used for system logging, user tracking, caches, etc. Basically anything that is subject to change all the time. |

###  Common Desktop Filesystem Types
- **To Check out what filesystems are on our machine:**
  ```sh
  [root@rhel ~]# df -T
  ```
<details>
  <summary>Click to View Common Types of Desktop Filesystem</summary>
  
1. **ext4** - This is the most current version of the native Linux filesystems. It is compatible with the older ext2 and ext3 versions. It supports disk volumes up to 1 exabyte and file sizes up to 16 terabytes and much more. It is the standard choice for Linux filesystems.
2. **Btrfs - "Better or Butter FS"** it is a new filesystem for Linux that comes with snapshots, incremental backups, performance increase and much more. It is widely available, but not quite stable and compatible yet.
3. **XFS** - High performance journaling file system, great for a system with large files such as a media server.
4. **NTFS and FAT** - Windows filesystems
5. **HFS+** - Macintosh filesystem

- Check `df -T` to View Filesystem Information on our system.
  
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
  <summary>Click to view Detailed Anatomy of Disk,Practical Guide to Disk Partitioning, Creating a File System in the Partitioned Disk & Mount-UMount to the partioned disk.</summary>
  
#### **1. Partition Table: The Disk's Blueprint**  
- Every disk has a **partition table** that maps out:  
  - Where partitions start and end.  
  - Which partitions are bootable.  
  - Which disk sectors belong to which partition.
  - we can have multiple partitions on a disk and they can't overlap each other. If there is space that is not allocated to a partition, then it is known as free space. 
- Two main types: **MBR** (old) and **GPT** (new).  


#### **2. MBR (Master Boot Record)**  
- **Old-school standard**.  
- Can have primary, extended, and logical partitions.
- Supports up to **4 primary partitions**.  
  - Need more? Convert one primary into an **extended partition** and add **logical partitions** inside it.  
- Limited to disks **up to 2TB**.  


#### **3. GPT (GUID Partition Table)**  
- **Modern standard**.  
- No partition type nonsense—just create as many partitions as we need.  
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

- **Check out Disk Partition on our machine:**
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

### Disk Partitioning & Creating a File System in the Partitioned Disk & Mount-UMount
- Disk partitioning is a critical task for managing storage devices.
- There are several tools available for disk partitioning, each with its own strengths:
  - **`fdisk`**: A basic command-line partitioning tool. It does **not** support GPT (GUID Partition Table).
  - **`parted`**: A versatile command-line tool that supports both MBR (Master Boot Record) and GPT partitioning.
  - **`gparted`**: The GUI version of `parted`, ideal for users who prefer a graphical interface.
  - **`gdisk`**: Similar to `fdisk`, but it **only supports GPT** (no MBR).
- Partitioning a disk is a straightforward process with the right tools. Using `parted`, we can:
1. Select the target device.
2. View the current partition table.
3. Create new partitions with specific start and end points.
4. Verify and save changes.

### **Step 1: Launch `parted`**
Open our terminal and launch `parted` with root privileges:

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
Once we're done, exit the `parted` shell:

```bash
(parted) quit
```

**Output:**

```
Information: we may need to update /etc/fstab.
```

### **Step 7: Resize a Partition**
- we can also resize a partition if we don't have any space.
```bash
resize 2 1245 3456
```
- Select the partition number and then the start and end points of where we want to resize it to.

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

When we're done using the partition, unmount it using the `umount` command:

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

<details>
  <summary>Click to view Detailed Filesystem Commands</summary>

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

</details>

---

## User Management
- In traditional OS, users and groups manage access and permissions. Each user has a unique UID and a home directory (e.g., /home/username) for personal files. Groups (GID) assign shared permissions. Processes run under the owner's permissions, ensuring privacy (e.g., Jane can't access Bob's files).
- Linux includes system users (e.g., daemons) and the root user, which has full system control. Root access is powerful but risky; users can use sudo for temporary root privileges instead of logging in as root.

<details>
  <summary>Click to View User Management Commands</summary>

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


</details>

---
## Permission Commands

<details>
  <summary>Click to View File, User & Group Permission Commands</summary>
  
| **Topic**               | **Command**                                                                 | **Description**                                                                 | **Example**                                                                 |
|-------------------------|-----------------------------------------------------------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **File Permissions**    | `ls -l`                                                                     | Displays file permissions, ownership, and other details.                        | `ls -l file.txt` (Shows permissions for `file.txt`)                         |
| **Modifying Permissions** | `chmod`<br>`chmod u+x myfile`<br>`chmod u-x myfile`<br>`chmod ug+w`         | Changes file permissions for owner, group, and others.                          | `chmod 755 script.sh` (Sets `rwxr-xr-x` permissions)                       |
| **Ownership Permissions** | `chown`<br>`chown patty myfile`<br>`sudo chgrp whales myfile`<br>`sudo chown patty:whales myfile` | Changes file ownership (user and group).                                        | `chown user:group file.txt` (Changes owner to `user` and group to `group`)  |
| **Umask**               | `umask`                                                                     | Sets default permissions for newly created files and directories.               | `umask 022` (Sets default permissions to `rw-r--r--` for files)             |
| **Setuid**              | `chmod u+s`<br>`chmod 4755`                                                 | Sets the SetUID bit, allowing a file to execute with the owner's permissions.    | `chmod u+s /usr/bin/program` (Runs `program` with owner's privileges)       |
| **Setgid**              | `chmod g+s`<br>`chmod 2555`                                                 | Sets the SetGID bit, allowing a file to execute with the group's permissions.    | `chmod g+s /usr/bin/program` (Runs `program` with group's privileges)       |
| **Process Permissions** | `ps -ef`                                                                    | Displays running processes and their permissions.                               | `ps -ef` (Shows all running processes with details)                         |
| **The Sticky Bit**      | `chmod +t`<br>`chmod 1755`                                                  | Sets the sticky bit on a directory, restricting file deletion to the owner.      | `chmod +t /shared_dir` (Only owners can delete their files in `/shared_dir`)|

### Notes:
- **Permissions Notation**: 
  - `r` = read, `w` = write, `x` = execute.
  - Numeric notation: `4` = read, `2` = write, `1` = execute (e.g., `755` = `rwxr-xr-x`).
- **Special Permissions**:
  - SetUID (`u+s` or `4755`): Executes with owner's privileges.
  - SetGID (`g+s` or `2555`): Executes with group's privileges.
  - Sticky Bit (`+t` or `1755`): Restricts file deletion in directories.

</details>

---
## Processes
- Processes are the programs that are running on our machine. They are managed by the kernel and each process has an ID associated with it called the process ID (PID). This PID is assigned in the order that processes are created.
```bash
root@ip-172-31-3-50:~# ps
```
![image](https://github.com/user-attachments/assets/f5bad342-3705-402e-a8af-9265899d1f44)
- This shows we a quick snapshot of the current processes:
  - PID: Process ID
  - TTY: Controlling terminal associated with the process (we'll go in detail about this later)
  - STAT: Process status code
  - TIME: Total CPU usage time
  - CMD: Name of executable/command

<details>
  <summary>Click to view Detailed Explaination Controlling Terminal, Processes Details, Process Creation, Process Termination, Signals, Signal Process, Common Signals, Job Control</summary>

### Controlling Terminal (TTY)
- TTY is the terminal that executed the command.
- Two types: Regular terminal (e.g., TTY1) and Pseudoterminal (e.g., pts/*).
- Daemon processes have no controlling terminal (TTY = ?).
  
### Process Details
- The kernel is in charge of processes, when we run a program the kernel loads up the code of the program in memory, determines and allocates resources and then keeps tabs on each process, it knows:
  - The status of the process
  - The resources the process is using and receives
  - The process owner
  - Signal handling
  - And basically everything else
    
### Process Creation
- Process creation involves cloning an existing process using the `fork` system call, which creates a child process with a new Process ID (PID). The original process becomes the parent, identified by a Parent Process ID (PPID). The child can either continue running the parent's program or use the `execve` system call to start a new program, replacing its memory setup.
- For example, when we run `ps l` in our terminal, the shell (e.g., `bash`) is the parent process, and `ps l` is its child, sharing the shell's PID as its PPID.
- The first process, `init` (PID 1), is created during system boot. It spawns all other processes, runs with root privileges, and cannot be terminated until the system shuts down. This "mother of all processes" ensures the system runs smoothly.
```bash
root@ip-172-31-3-50:~# ps -l
```

### Process Termination
- When a process is no longer needed, it can exit using the `_exit` system call, freeing its resources. The process reports its termination status to the kernel, with `0` typically meaning success. However, the process isn't fully terminated until its parent acknowledges it using the `wait` system call, which checks the termination status. If the parent doesn't call `wait`, the process becomes a **zombie**.
- **Orphan Processes**
  - If a parent process dies before its child, the kernel assigns the child to `init` (the main system process). `Init` then handles the `wait` call, allowing the orphan to terminate properly.
- **Zombie Processes**
  - When a child process terminates but the parent hasn't called `wait`, it becomes a zombie. Zombies free their resources but remain in the process table until the parent calls `wait` (or `init` does it if the parent is gone). Too many zombies can fill the process table, blocking new processes.
    
### Signals
**Signals** are notifications sent to a process to inform it that an event has occurred. They act as software interrupts and serve various purposes:
  - **User actions**: Like pressing Ctrl-C to interrupt or Ctrl-Z to suspend a process.  
  - **Hardware/software issues**: The kernel notifies processes of problems.  
  - **Inter-process communication**: Signals allow processes to communicate.
- When a signal is generated, it stays **pending** until delivered to the process. Processes can:
  - Ignore the signal.  
  - Catch and handle it with a custom routine.  
  - Terminate the process.  
  - Block the signal (if allowed).

- **Common Signals**:  
  - **SIGHUP (1)**: Hangup.  
  - **SIGINT (2)**: Interrupt (e.g., Ctrl-C).  
  - **SIGKILL (9)**: Kill (unblockable, terminates process).  
  - **SIGSEGV (11)**: Segmentation fault.  
  - **SIGTERM (15)**: Software termination.  
  - **SIGSTOP**: Stop process.
- Signals are usually referred to by names (e.g., SIGKILL) rather than numbers, as numbers can vary. Some signals, like SIGKILL, cannot be blocked.

### Kill (Terminate)
- The `kill` command terminates processes using signals. For example:
  - `kill 12445` sends a **SIGTERM** signal (default), asking the process to exit gracefully.
  - `kill -9 12445` sends a **SIGKILL** signal, forcing the process to stop immediately without cleanup.
- **Key Signals:**
  - **SIGHUP**: Sent when the terminal closes (e.g., closing a window).
  - **SIGINT**: Interrupts the process (e.g., using `Ctrl+C`).
  - **SIGTERM**: Requests a graceful termination with cleanup.
  - **SIGKILL**: Forces an immediate stop (no cleanup).
  - **SIGSTOP**: Pauses/suspends a process.

### niceness
- When we run multiple programs on our computer, they don’t actually run simultaneously. Instead, the CPU gives each process a small time slice, switching between them quickly. The kernel manages this process scheduling, ensuring each program gets fair CPU time.
- However, we can influence this with **niceness**, a priority value for processes. A high niceness (positive number) means lower priority (being "nice" to others), while a low or negative niceness means higher priority (grabbing more CPU time).
- You can check niceness in the `NI` column using the `top` command. To set niceness:
  - Use `nice` for new processes:  
    `nice -n 5 apt upgrade`  
  - Use `renice` for existing processes:  
    `renice 10 -p 3245`
  - This lets us control how much CPU time a process gets.

### Process States
- When you run `ps aux`, the **STAT** column shows process states. Common states include:
  - **R**: Running or ready to run (waiting for CPU).
  - **S**: Sleeping, waiting for an event (e.g., user input).
  - **D**: Uninterruptible sleep (can't be killed; often requires a reboot).
  - **Z**: Zombie process (terminated but waiting for status cleanup).
  - **T**: Stopped or suspended process.

### /proc Filesystem
- The `/proc` filesystem in Linux stores process information, treating each process as a file. Each process has a directory named by its PID (Process ID) under `/proc`. For example, to view details of a process with PID 12345, you can use:
  ```bash
  cat /proc/12345/status
  ```
- This provides detailed process state and other kernel-level information, offering more insights than tools like `ps`.

### Job Control
If you're running a long command in a terminal and want to keep using the shell, you can manage processes using job control.

1. **Run a Command in the Background**:  
   Add `&` to the end of a command to run it in the background:  
   ```bash
   $ sleep 1000 &
   ```

2. **View Background Jobs**:  
   Use `jobs` to see running background jobs:  
   ```bash
   $ jobs
   ```
   Output:  
   ```
   [1]  Running  sleep 1000 &
   [2]- Running  sleep 1001 &
   [3]+ Running  sleep 1002 &
   ```
   - `+`: Most recent job.  
   - `-`: Second most recent job.

3. **Send a Running Job to the Background**:  
   Suspend the job with `Ctrl-Z`, then use `bg` to send it to the background:  
   ```bash
   $ sleep 1003
   ^Z
   [4]+ Stopped  sleep 1003
   $ bg
   [4]+ sleep 1003 &
   ```

4. **Bring a Job to the Foreground**:  
   Use `fg` with the job ID (e.g., `%1`):  
   ```bash
   $ fg %1
   ```

5. **Kill a Background Job**:  
   Use `kill` with the job ID:  
   ```bash
   $ kill %1
   ```
This lets us manage tasks without interrupting your workflow.

</details>

---

## Packages
Packages are collections of files (like programs, libraries, and documentation) bundled together into a single unit for easy installation and management. Think of them as ready-to-use software bundles, such as web browsers, text editors, or media players. These packages are created by developers (upstream providers) and distributed through **package managers** or **repositories**, making it simple to install, update, and remove software on your system. Common package formats include **.deb** (used in Debian/Ubuntu) and **.rpm** (used in Red Hat/Fedora). Packages often rely on **dependencies** (other software or libraries) to function properly, which package managers handle automatically.

<details>
  <summary>Click to view Detailed Explaination of Software Distribution, Package Repositories, Package Dependencies, rpm and dpkg, yum and apt & Compile Source Code.</summary>

### **Software Distribution**
- Your system uses **packages** (like Chrome or Photoshop) which are collections of files compiled into one. These are managed by **package managers** that install and update software. Most packages come in **.deb** (Debian/Ubuntu) or **.rpm** (Red Hat/Fedora) formats. Developers (upstream providers) create the software, and **package maintainers** review and distribute it.

### **Package Repositories**  
- Instead of downloading packages manually, you can use **repositories**—central locations storing packages online. Your system knows where to find these repositories through a sources file (e.g., `/etc/apt/sources.list` on Debian). For example, if a repository hosts `WackyWidgets` software, you can add its link to your sources file to access its packages.

### **Package Dependencies**  
- Packages often rely on other packages or **shared libraries** to function. If dependencies are missing, the package won’t work. Think of it like restaurants depending on a farm for ingredients—without the farm, they can’t operate.

### **Package Management Tools**  
- **.deb** (Debian): Use `dpkg` to install (`dpkg -i package.deb`) or remove (`dpkg -r package.deb`) packages.  
- **.rpm** (Red Hat): Use `rpm` to install (`rpm -i package.rpm`) or remove (`rpm -e package.rpm`) packages.  
- However, these tools don’t handle dependencies automatically, which is where **package management systems** like `apt` (Debian) and `yum` (Red Hat) come in. They handle installation, removal, and dependency resolution.

### **Common Commands**  
- Install: `apt install package` (Debian) or `yum install package` (Red Hat).  
- Remove: `apt remove package` or `yum erase package`.  
- Update: `apt update; apt upgrade` or `yum update`.  

### **Compiling Source Code**  
Sometimes, you’ll need to compile software from source code. Here’s how:  
1. Install build tools: `sudo apt install build-essential`.  
2. Extract the source: `tar -xzvf package.tar.gz`.  
3. Check for dependencies: `./configure`.  
4. Build the software: `make`.  
5. Install: `sudo make install` (or use `sudo checkinstall` to create a `.deb` for easier removal).
   
- In short, package managers and repositories simplify software installation, while tools like `dpkg`, `rpm`, `apt`, and `yum` handle the heavy lifting. For source code, use `make` and `checkinstall` for easier management.

</details>

---
## init
The terms **Init** is Initialization where init acts as a **MOTHER OF ALL PROCESS & It has a Process ID (PID) of 1**, **System V**, **Upstart**, and **Systemd** are all related to the initialization and management of services and processes in Unix-like operating systems (e.g., Linux). They represent different generations of **init systems**, which are responsible for booting the system, starting services, and managing system states. 

<details>
  <summary>Click to check explanation of each, their differences, and their purposes.</summary>

### **1. System V Overview**
System V (Sys V) is a traditional init system in Linux, used to start and stop essential processes sequentially via scripts. It’s identified by the presence of `/etc/inittab`. 

**Key Features:**
- **Runlevels (0-6):** Define system states (e.g., shutdown, single-user, multiuser with/without networking, GUI, reboot).
- **Scripts:** Located in `/etc/rc.d/rc[runlevel].d/` or `/etc/init.d`, scripts starting with `S` (start) or `K` (kill) execute in sequence during startup/shutdown.
- **Dependency Management:** Easy to handle since processes start/stop in order (e.g., `foo-a` before `foo-b`).

**Pros:** Simple dependency resolution.  
**Cons:** Poor performance due to sequential execution.

**Example:** In runlevel 0 (shutdown), scripts like `K10updates` and `K80openvpn` run to stop services.

**Note:** Sys V is being phased out but remains relevant for legacy services. Runlevels may appear in newer init systems for compatibility.

---

### **1.1. System V Service**
You can use the `service` command to manage System V services. Here are the basic commands:
- **List all services**:
  ```bash
  service --status-all
  ```
- **Start a service**:
  ```bash
  sudo service networking start
  ```
- **Stop a service**:
  ```bash
  sudo service networking stop
  ```
- **Restart a service**:
  ```bash
  sudo service networking restart
  ```
- These commands also work with Upstart services. While Linux is transitioning away from System V init scripts, these commands help ease the shift.

---

### **2. Upstart Overview**
- Upstart, developed by Canonical, was Ubuntu's init system before systemd replaced it. It improved on SysV by allowing event-driven job execution instead of strict, sequential startup processes.
- To check if Upstart is in use, look for the `/usr/share/upstart` directory. Jobs define actions, while events trigger them. Job configurations are in `/etc/init/`, and an example from `networking.conf` might be:
  ```  
  start on runlevel [235]  
  stop on runlevel [0]  
  ```
- The way that Upstart works is that:
  1. First, it loads up the job configurations from /etc/init
  2. Once a startup event occurs, it will run jobs triggered by that event.
  3. These jobs will make new events and then those events will trigger more jobs
  4. Upstart continues to do this until it completes all the necessary jobs

---

### **2.1. Upstart Jobs**
- Upstart manages system jobs and events, but tracking their origins can be tricky. You can control and monitor jobs using these commands:
1. **List all jobs**:  
   `initctl list`  
   Shows job names, goals (e.g., start/stop), and current statuses (e.g., waiting/running).
2. **Check a specific job's status**:  
   `initctl status <job_name>`  
   Example: `initctl status networking` → `networking start/running`.
3. **Control jobs manually**:  
   - Start: `sudo initctl start <job_name>`  
   - Stop: `sudo initctl stop <job_name>`  
   - Restart: `sudo initctl restart <job_name>`  
4. **Emit an event**:  
   `sudo initctl emit <event_name>`
- Job configurations are in `/etc/init/*.conf`, but you usually won’t need to edit them. Use the commands above to manage jobs directly.

---

### **3. Systemd Overview**
- Systemd is the modern init system for Linux. If you have `/usr/lib/systemd`, you're using it. It boots your system by achieving "targets" (goals) and their dependencies, offering flexibility and robustness.
#### Key Points:
1. **Boot Process**:
   - Loads configs from `/etc/systemd/system` or `/usr/lib/systemd/system`.
   - Sets the boot goal, usually `default.target`.
   - Activates dependencies for the target.

2. **Common Targets**:
   - `poweroff.target`: Shutdown.
   - `rescue.target`: Single-user mode.
   - `multi-user.target`: Multiuser with networking.
   - `graphical.target`: Multiuser with networking and GUI.
   - `reboot.target`: Restart.

   `default.target` typically points to `graphical.target`.

3. **Units**:
  - The main object that systemd works with are known as units. Systemd doesn't just stop and start services, it can mount filesystems, monitor your network sockets, etc and because of that robustness it has different types of units it operates. The most common units are:
    - **Service units** (`.service`): Manage services.
    - **Mount units** (`.mount`): Handle filesystem mounts.
    - **Target units** (`.target`): Group other units.
- For example, `default.target` may include `networking.service` and `crond.service`, activating all necessary units when booting.

---

### **3.1. Systemd Goals**
- A systemd *unit file* defines services, startup order, and dependencies. Here's a simplified example (`foobar.service`):

```ini
[Unit]
Description=My Foobar
Before=bar.target  # Starts before "bar.target"

[Service]
ExecStart=/usr/bin/foobar  # Command to run the service

[Install]
WantedBy=multi-user.target  # Auto-starts with this system target
```

**Key Sections:**
- **`[Unit]`**: Metadata and startup order rules.
- **`[Service]`**: Commands to manage the service (start/stop/reload).
- **`[Install]`**: Dependency rules for enabling/disabling the service.

**Essential Commands:**
- List active units: `systemctl list-units`
- Check status: `systemctl status <unit>`
- Start/Stop/Restart: `systemctl start|stop|restart <unit>`
- Enable/Disable auto-start: `systemctl enable|disable <unit>`

This is a basic overview; systemd offers advanced features like timers, sockets, and complex dependencies. Use `man systemd` or official documentation for deeper exploration.

---

### **4. Power States**
- Power States: Shutdown and Restart Commands
- To control your system's power state via the command line:
1. **Shutdown immediately:**  
   `sudo shutdown -h now`  
   This halts (powers off) the system.
2. **Shutdown in X minutes:**  
   `sudo shutdown -h +X`  
   Example: `sudo shutdown -h +2` shuts down in 2 minutes.
3. **Restart immediately:**  
   `sudo shutdown -r now`  
   Or simply use:  
   `sudo reboot`  
- These commands help manage your system's power state efficiently.

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










