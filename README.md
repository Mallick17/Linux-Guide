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
 
<details>
  <summary>Click to View DISTRIBUTIONS in Detail</summary>

In the context of operating systems, a distribution (often called a "distro" in the Linux world) bundles the **kernel**, **core utilities**, **applications**, and **configuration settings** into a cohesive system. Below are examples of each component across different operating system distributions:

---

### **1. Core Utilities**
Core utilities are essential programs that provide basic functionality for managing files, processes, and system operations. Examples include:

- **Linux Distributions (e.g., Ubuntu, Fedora, Debian):**
  - `bash` or `zsh`: Command-line shells for interacting with the OS.
  - `coreutils`: A package containing tools like `ls`, `cp`, `mv`, `rm`, `mkdir`, `cat`, and `echo`.
  - `grep`: A utility for searching text using patterns.
  - `awk` and `sed`: Text processing tools.
  - `systemd`: A system and service manager for initializing and managing system processes.
  - `tar`, `gzip`, `zip`: Utilities for file compression and archiving.

- **macOS:**
  - `zsh` (default shell since macOS Catalina) or `bash`.
  - `launchd`: A system management daemon for starting, stopping, and managing processes.
  - `Finder`: The default file manager.
  - `Disk Utility`: A tool for managing storage devices.

- **Windows:**
  - `cmd.exe` or `PowerShell`: Command-line interfaces.
  - `File Explorer`: The default file manager.
  - `Task Manager`: A utility for managing processes and system performance.
  - `Disk Management`: A tool for managing partitions and storage.

---

### **2. Applications**
Applications are software programs that provide specific functionality to users. Examples include:

- **Linux Distributions:**
  - **Web Browsers:** Firefox, Chromium.
  - **Office Suites:** LibreOffice, OnlyOffice.
  - **Media Players:** VLC, Rhythmbox.
  - **Text Editors:** GNU Nano, Vim, Gedit.
  - **Development Tools:** GCC (GNU Compiler Collection), Python, Git.

- **macOS:**
  - **Web Browsers:** Safari, Chrome, Firefox.
  - **Office Suite:** Microsoft Office, Apple iWork (Pages, Numbers, Keynote).
  - **Media Players:** QuickTime, iTunes (now replaced by Music and TV apps).
  - **Text Editors:** TextEdit, BBEdit.
  - **Development Tools:** Xcode, Homebrew (package manager).

- **Windows:**
  - **Web Browsers:** Microsoft Edge, Chrome, Firefox.
  - **Office Suite:** Microsoft Office.
  - **Media Players:** Windows Media Player, VLC.
  - **Text Editors:** Notepad, Notepad++.
  - **Development Tools:** Visual Studio, PowerShell ISE.

---

### **3. Configuration Settings**
Configuration settings define how the operating system and its components behave. These are often stored in configuration files or managed through graphical interfaces. Examples include:

- **Linux Distributions:**
  - `/etc/fstab`: Configures filesystem mounting at boot.
  - `/etc/hosts`: Maps hostnames to IP addresses.
  - `/etc/network/interfaces` or `Netplan` (Ubuntu): Network configuration.
  - `/etc/ssh/sshd_config`: SSH server settings.
  - `~/.bashrc` or `~/.zshrc`: Shell configuration for individual users.
  - `systemctl`: Command-line tool for managing `systemd` services.

- **macOS:**
  - `plist` files (Property List): Configuration files for apps and system settings (e.g., `/Library/Preferences/`).
  - `System Preferences`: GUI for configuring system settings like network, display, and user accounts.
  - `launchctl`: Command-line tool for managing `launchd` services.
  - `~/.zshrc` or `~/.bash_profile`: Shell configuration for individual users.

- **Windows:**
  - **Registry Editor (`regedit`)**: Centralized database for system and application settings.
  - **Control Panel**: GUI for configuring system settings like network, display, and user accounts.
  - **Group Policy Editor (`gpedit.msc`)**: Configures system policies for users and computers.
  - **Task Scheduler**: Configures automated tasks.
  - `PowerShell`: Scripting and configuration management.

---

### **Examples of Popular Distributions**
Here are some examples of operating system distributions and their bundled components:

- **Linux:**
  - **Ubuntu**: Comes with GNOME desktop, Firefox, LibreOffice, and `systemd`.
  - **Fedora**: Includes GNOME desktop, Firefox, and `dnf` package manager.
  - **Debian**: Ships with a minimal set of utilities and allows users to customize during installation.

- **macOS:**
  - A proprietary OS by Apple, distributed with Safari, iWork, and Xcode.

- **Windows:**
  - **Windows 10/11**: Comes with Microsoft Edge, Office apps (trial), and Windows Defender.

---
The **kernel** is the core component of an operating system, acting as a bridge between hardware and software. It manages system resources, handles communication between hardware and processes, and ensures security and stability. Below are examples of kernels used in different operating system distributions:

---

### **1. Linux Kernel**
The Linux kernel is the most widely used open-source kernel, powering a vast array of distributions. It is highly modular and customizable.

- **Examples of Linux Distributions Using the Linux Kernel:**
  - **Ubuntu**: Uses a modified version of the Linux kernel with additional patches for stability and hardware support.
  - **Fedora**: Uses a relatively up-to-date Linux kernel with support for the latest hardware and features.
  - **Debian**: Uses a stable version of the Linux kernel, often slightly older but highly tested.
  - **Arch Linux**: Uses a vanilla Linux kernel, often the latest version, with minimal modifications.
  - **Android**: Uses a heavily modified Linux kernel optimized for mobile devices.

- **Key Features of the Linux Kernel:**
  - Supports a wide range of hardware architectures (x86, ARM, RISC-V, etc.).
  - Modular design allows for loadable kernel modules (LKMs).
  - Includes drivers for most hardware devices.
  - Supports advanced features like cgroups, namespaces (for containers), and real-time scheduling.

---

### **2. macOS Kernel (XNU)**
macOS uses a hybrid kernel called **XNU** (X is Not Unix), which combines elements of monolithic and microkernel designs. It is part of the Darwin operating system, the open-source foundation of macOS.

- **Key Features of the XNU Kernel:**
  - **Mach Microkernel**: Handles low-level tasks like memory management and inter-process communication (IPC).
  - **BSD Layer**: Provides Unix-like functionality, including file systems, networking, and security.
  - **I/O Kit**: A driver framework for hardware support.
  - **Kernel Extensions (kexts)**: Allow dynamic loading of kernel modules, though Apple is moving toward user-space drivers for security reasons.

---

### **3. Windows Kernel (NT Kernel)**
Windows uses the **Windows NT kernel**, which is a hybrid kernel designed for performance, scalability, and security. It powers all modern Windows operating systems, including Windows 10, Windows 11, and Windows Server.

- **Key Features of the Windows NT Kernel:**
  - Supports multiple hardware architectures (x86, x64, ARM).
  - Includes a Hardware Abstraction Layer (HAL) to abstract hardware differences.
  - Provides advanced security features like Kernel Patch Protection (PatchGuard) and Mandatory Integrity Control.
  - Supports symmetric multiprocessing (SMP) and real-time applications.
  - Uses a modular design with kernel-mode and user-mode components.

---

### **4. BSD Kernels**
BSD (Berkeley Software Distribution) operating systems use variants of the BSD kernel, which is derived from the original Unix kernel.

- **Examples of BSD Distributions:**
  - **FreeBSD**: Uses the FreeBSD kernel, optimized for performance and scalability.
  - **OpenBSD**: Uses the OpenBSD kernel, focused on security and correctness.
  - **NetBSD**: Uses the NetBSD kernel, designed for portability across hardware platforms.

- **Key Features of BSD Kernels:**
  - Monolithic design with modular components.
  - Strong focus on stability, security, and performance.
  - Includes advanced networking features (e.g., PF firewall in OpenBSD).
  - Supports ZFS (Zettabyte File System) for advanced storage management.

---

### **5. Other Kernels**
- **Solaris Kernel**: Used in Oracle Solaris and OpenSolaris, known for its advanced features like DTrace and ZFS.
- **MINIX Kernel**: A microkernel used in the MINIX operating system, primarily for educational purposes.
- **QNX Kernel**: A real-time microkernel used in embedded systems and automotive applications.
- **Haiku Kernel**: Used in the Haiku operating system, inspired by the BeOS kernel.

---

### **Summary of Kernel Examples**
| **Operating System** | **Kernel**          | **Type**       | **Example Distributions**       |
|-----------------------|---------------------|----------------|----------------------------------|
| Linux                 | Linux Kernel        | Monolithic     | Ubuntu, Fedora, Debian, Android |
| macOS                 | XNU                | Hybrid         | macOS                            |
| Windows               | Windows NT Kernel   | Hybrid         | Windows 10, Windows 11          |
| FreeBSD               | FreeBSD Kernel      | Monolithic     | FreeBSD                          |
| OpenBSD               | OpenBSD Kernel      | Monolithic     | OpenBSD                          |
| Solaris               | Solaris Kernel      | Monolithic     | Oracle Solaris                   |


- Each kernel is designed with specific goals in mind, such as performance, security, or real-time capabilities, and is tailored to the needs of its respective operating system and user base.

</details>

---

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

## Process Utilization

### Process Utilization Commands

| **Topic**                  | **Command**                          | **Description**                                                                 | **Example**           |
|----------------------------|--------------------------------------|-----------------------------------------------------------------------------|-----------------------|
| Tracking processes         | `top`                                | Displays real-time system resource usage                                    | `top`                 |
| Listing open files         | `lsof`                               | Lists open files and the processes using them                              | `lsof -i :80`         |
| Checking file usage        | `fuser`                              | Identifies processes using a specific file                                 | `fuser /var/log/syslog` |
| Process threads            | `ps -eLf`                            | Displays detailed thread information                                       | `ps -eLf | grep java` |
| CPU Monitoring             | `mpstat`                             | Reports CPU usage statistics                                               | `mpstat 1 5`          |
| I/O Monitoring             | `iostat`                             | Displays CPU and I/O usage statistics                                      | `iostat -x 1 5`       |
| Memory Monitoring          | `free -m`                            | Shows memory usage details                                                 | `free -m`             |
| Additional Memory Monitoring | `vmstat`                            | Reports memory, swap, and CPU statistics                                   | `vmstat 1 5`          |
| Continuous Monitoring      | `htop`                               | Interactive process monitoring                                             | `htop`                |


<details>
  <summary>Click to check explanation of Commands Used</summary>

### Monitoring Processes with `top`

- The `top` command provides a real-time view of system resource usage, helping track active processes and performance metrics.

#### Key Information Displayed in `top`

#### 1. System Overview (First Line)
- **Current Time**: System time
- **Uptime**: How long the system has been running
- **Users**: Number of logged-in users
- **Load Average**: System workload over 1, 5, and 15 minutes

#### 2. Task Summary (Second Line)
- **Total Tasks**: Number of processes
- **Running**: Active processes
- **Sleeping**: Inactive but waiting
- **Stopped & Zombie**: Terminated or waiting for cleanup

#### 3. CPU Usage (Third Line)
- **us**: User processes CPU time
- **sy**: System (kernel) CPU time
- **ni**: Niced (priority-adjusted) CPU time
- **id**: Idle CPU time
- **wa**: I/O wait time
- **hi & si**: Hardware & software interrupt time
- **st**: Stolen CPU time (for virtual machines)

#### 4. Memory & Swap Usage (Fourth & Fifth Line)
- **Total, Used, Free**: Memory and swap statistics
- **Buffers & Cached**: Memory reserved for system operations

#### Process List (Columns Explained)
- **PID**: Process ID
- **USER**: Owner of the process
- **PR & NI**: Priority & nice value
- **VIRT & RES**: Virtual & physical memory usage
- **SHR**: Shared memory usage
- **S**: Process state (R=Running, S=Sleeping, Z=Zombie, etc.)
- **%CPU & %MEM**: CPU & memory usage percentage
- **TIME+**: Total process runtime
- **COMMAND**: Process name

#### Tracking Specific Processes
- To monitor a particular process by ID:
```bash
$ top -p <PID>
```
- Use `top` to quickly analyze system performance and manage running processes effectively!

---

### Memory Monitoring with `vmstat`
The `vmstat` command provides an overview of memory, CPU, and I/O usage.

#### Example Output:
```bash
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 396528  38816 384036    0    0     4     2   38   79  0  0 99  0  0
```

#### Fields Explained:
- **procs**
  - `r`: Processes waiting to run
  - `b`: Processes in uninterruptible sleep
- **memory**
  - `swpd`: Virtual memory used
  - `free`: Free memory
  - `buff`: Memory used as buffers
  - `cache`: Memory used as cache
- **swap**
  - `si`: Memory swapped in from disk
  - `so`: Memory swapped out to disk
- **io**
  - `bi`: Blocks received from block devices
  - `bo`: Blocks sent to block devices
- **system**
  - `in`: Interrupts per second
  - `cs`: Context switches per second
- **cpu**
  - `us`: User time
  - `sy`: System (kernel) time
  - `id`: Idle time
  - `wa`: I/O wait time

---

### CPU & Disk Monitoring with `iostat`
The `iostat` command provides CPU and disk usage statistics.

#### Example Output:
```bash
avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.13    0.03    0.50    0.01    0.00   99.33

Device:            tps    kB_read/s    kB_wrtn/s    kB_read    kB_wrtn
sda               0.17         3.49         1.92     385106     212417
```

#### Fields Explained:
- **CPU Usage**
  - `%user`: CPU usage by user processes
  - `%nice`: CPU usage by niced processes
  - `%system`: CPU usage by system processes
  - `%iowait`: Time spent waiting for I/O
  - `%steal`: Time stolen by the hypervisor in VMs
  - `%idle`: Idle CPU time
- **Disk Usage**
  - `tps`: Transfers per second
  - `kB_read/s`: Data read per second
  - `kB_wrtn/s`: Data written per second
  - `kB_read`: Total data read
  - `kB_wrtn`: Total data written
</details>

---

## Logging
### System Logging
- System services, kernels, and daemons generate activity data, which is saved as logs in the `/var` directory. These logs provide a readable record of system events.
- A service called **syslog** (or **rsyslog** on newer systems) manages these logs. It uses a daemon (like `syslogd` or `rsyslogd`) to receive, filter, and store event messages. Depending on the rules, messages can be saved to files, displayed on the console, or ignored.
- While syslog is a central logging tool, many applications create their own log files. Logs typically include a **timestamp** and **event details**. For example:
```
Jan 27 07:41:32 icebox anacron[4650]: Job `cron.weekly' started
```
- This shows the `cron.weekly` job ran at the specified time. You can view such logs in `/var/log/syslog`.

### logrotate
- **The logrotate utility does log management for us. It has a configuration file that allows us to specify how many and what logs to keep, how to compress our logs to save space and more. The logrotate tool is usually run out of cron once a day and the configuration files can be found in `/etc/logrotate.d.`**

  
<details>
  <summary>Click to View Detailed explaination of Logging</summary>

### syslog
- **Syslog** manages and sends logs to the system logger. **Rsyslog** is an enhanced version used by most Linux systems. Logs collected by syslog are stored in `/var/log/syslog` (excluding auth messages).
- To see which files are logged, check the configuration in `/etc/rsyslog.d/`. For example:
```bash
less /etc/rsyslog.d/50-default.conf
```
- This file defines rules where the left column specifies the log type (selector) and the right column specifies the action (e.g., saving to a file like `/var/log/auth.log` or `/var/log/syslog`). Not all applications use rsyslog, so check the directory for specific logs.
- To test logging, use the `logger` command:
```bash
logger -s Hello
```
- Check `/var/log/syslog` to see the "Hello" entry.

### General Logging
- There are many log files you can view on your system, many important ones can be found under /var/log. We won't go through them all, but we'll discuss a couple of the major ones.
  1. `/var/log/messages`
     - This log contains all non-critical and non-debug messages, includes messages logged during bootup (dmesg), auth, cron, daemon, etc. Very useful to get a glimpse of how your machine is acting.
  2. `/var/log/syslog`
     - This logs everything except auth messages, it's extremely useful for debugging errors on your machine.

### Kernel Logging
- `/var/log/dmesg`
  - On boot-time your system logs information about the kernel ring buffer. This shows us information about hardware drivers, kernel information and status during bootup and more. This log file can be found at /var/log/dmesg and gets reset on every boot, you may not actually see any use in it now, but if you were to ever have issues with something during bootup or a hardware issue, dmesg is the best place to look. You can also view this log using the dmesg command.
- `/var/log/kern.log`
  - Another log you can use to view kernel information is the /var/log/kern.log file, this logs the kernel information and events on your system, it also logs dmesg output.

### Authentication Logging
- `/var/log/auth.log`
  - This contains system authorization logs, such as user login and the authentication method used.
    ```bash
    
</details>

---



## Cron Jobs in Linux
Cron jobs are scheduled tasks in Linux that run at specified intervals. The cron daemon (`crond`) executes these jobs based on time intervals defined in a user's crontab file.

<details>
  <summary>Click to view the steps</summary>

### Checking and Creating Cron Jobs
- To check the existing cron jobs:
```bash
$ cat /etc/crontab
```
- To list available cron jobs:
```bash
$ crontab -l
```
- To create or edit a cron job:
```bash
$ crontab -e
```

### Crontab Syntax
**A cron job follows the below format:**
```
*  *  *  *  *  command_to_execute
|  |  |  |  |
|  |  |  |  |____ Day of the week (0 - 6) [Sunday=0]
|  |  |  |_______ Month (1 - 12)
|  |  |__________ Day of the month (1 - 31)
|  |_____________ Hour (0 - 23)
|_______________ Minute (0 - 59)
```

### Example Cron Jobs
1. Run a command at 11:00 AM on the 14th of February (Friday):
```bash
0 11 14 2 5 echo "hello" > /tmp/test.txt
```

2. Run a command at 5:32 AM on the 14th of February (Friday):
```bash
32 05 14 2 5 echo "hello" > /tmp/test.txt
```

3. Run a command at 3:55 PM on the 28th of December:
```bash
55 15 28 12 * /usr/bin/echo "hello" > /path/to/file
```

4. Run a command at 3:44 PM daily:
```bash
44 15 * * * echo "test" > /path/to/file
```

## Running Cron Jobs for Other Users
- To check root’s cron jobs:
```bash
$ sudo crontab -u root -l
```

- To create or edit a cron job for another user (e.g., `mallick`):
```bash
$ crontab -u mallick -e
```

### Special Time Intervals
**Cron also supports special time intervals:**
- `@hourly` – Runs every hour
- `@daily` – Runs once a day
- `@monthly` – Runs once a month
- `@yearly` – Runs once a year

- Example: Run a command every hour:
```bash
@hourly /usr/bin/echo "hello" > /path/to/file
```
- This ensures the job executes hourly.

</details>

---

## Cron Jobs in Windows
The cron job concept is implemented through the Task Scheduler. This built-in tool enables you to automate the execution of scripts, applications, or processes based on specific triggers, much like the cron daemon does in Linux.

The Task Scheduler offers a wide range of options for scheduling tasks to run at predetermined times, making it a powerful utility for automating regular tasks such as backups, log rotations, or data processing.

### Steps
- Open Windows PowerShell.
- `SCHTASKS` to view all the scheduled tasks in the windows system.
- 


<details>
  <summary>Theoritcal Execution Steps</summary>

Got it! Your cron line:

```
32 05 14 2 5 echo "hello" > /tmp/test.txt
```

…means: write “hello” to a file at **05:32**, either when it’s **Feb 14** or it’s **Friday** (cron’s “either DOM or DOW” behavior).

Below are two simple PowerShell ways:

---

# A) Do it **once today** (easiest)

This runs the equivalent command at today’s date, a couple minutes from now.

1. Open PowerShell.

2. Paste this (it schedules a one-off job a few minutes from now and creates `C:\Temp\test.txt` with “hello”):

```powershell
# 1. Pick a time a couple minutes from now (today)
$runAt   = (Get-Date).AddMinutes(2)

# 2. Define what to run (make sure the folder exists, then write "hello")
$script  = {
  New-Item -ItemType Directory -Path 'C:\Temp' -Force | Out-Null
  Set-Content -Path 'C:\Temp\test.txt' -Value 'hello'
}

# 3. Schedule it as a one-off "Scheduled Job"
$trigger = New-JobTrigger -Once -At $runAt
Register-ScheduledJob -Name 'WriteHelloToday' -ScriptBlock $script -Trigger $trigger | Out-Null

# 4. Confirm next run time
Get-ScheduledJob -Name 'WriteHelloToday' | Select-Object Name, NextRunTime
```

3. After the time passes, verify the result:

```powershell
Get-Content 'C:\Temp\test.txt'
```

4. (Optional) Clean up:

```powershell
Unregister-ScheduledJob -Name 'WriteHelloToday' -Force
```

> Notes
> • This uses PowerShell’s **Scheduled Jobs** (no password prompts; runs under your user).
> • `Set-Content` overwrites the file (like `>`). Use `Add-Content` if you want to append (like `>>`).

---

# B) Make a **recurring schedule** like your cron

Windows doesn’t have cron, but **Task Scheduler** can match the same behavior by adding **two triggers** (OR logic): one for Fridays at 05:32 and one for Feb 14 at 05:32.

1. Open PowerShell **as your user**.

2. Run:

```powershell
# Action: run PowerShell that ensures folder exists and writes "hello"
$action = New-ScheduledTaskAction -Execute 'powershell.exe' -Argument @'
-NoProfile -WindowStyle Hidden -Command "New-Item -ItemType Directory -Path ''C:\Temp'' -Force | Out-Null; Set-Content -Path ''C:\Temp\test.txt'' -Value ''hello''"
'@

# Triggers: Friday 05:32, and Feb 14 05:32 (every year)
$tWeekly  = New-ScheduledTaskTrigger -Weekly -DaysOfWeek Friday -At 05:32
$tYearly  = New-ScheduledTaskTrigger -At 05:32 -DaysOfMonth 14 -Months February

# Principal: run as the currently logged-in user (no password prompt)
$principal = New-ScheduledTaskPrincipal -UserId $env:UserName -LogonType Interactive

# Register the task
Register-ScheduledTask `
  -TaskName 'WriteHelloCronEquivalent' `
  -Action $action `
  -Trigger @($tWeekly, $tYearly) `
  -Principal $principal `
  -Description 'Mimic cron: 32 05 14 2 5' | Out-Null

# See it
Get-ScheduledTask -TaskName 'WriteHelloCronEquivalent' | Select-Object TaskName, State
```

3. (Optional) Remove later:

```powershell
Unregister-ScheduledTask -TaskName 'WriteHelloCronEquivalent' -Confirm:$false
```

---

## Quick Windows equivalents of your shell line

* Overwrite (like `>`):

  ```powershell
  Set-Content -Path 'C:\Temp\test.txt' -Value 'hello'
  ```
* Append (like `>>`):

  ```powershell
  Add-Content -Path 'C:\Temp\test.txt' -Value 'hello'
  ```

If you want me to tailor the “today” run to an exact time (e.g., **20 Aug 2025, 15:10 IST**) just say the time you want and I’ll drop in the exact command.


---
---

**Test plan + PowerShell script + step-by-step commands**, It can verify the scheduled task (Windows “cron”) will run your `aws s3 sync` reliably in **all** important cases (success, network failure, bad creds, bucket missing, concurrent runs, interrupted transfer, dry-run, etc).

I’ll include:

* a robust `s3sync.ps1` you save and schedule,
* how to run it manually and as a Scheduled Task,
* a set of test cases (how to simulate each and what to look for),
* quick commands to inspect task state and logs.

---

# 1) Prerequisites (quick)

1. Install AWS CLI v2 and ensure `aws` is in PATH. Check:

```powershell
aws --version
```

2. Configure a safe, minimal-permission AWS profile for the scheduled job:

```powershell
aws configure --profile mysync
# enter access key, secret, region
```

3. Make folders:

```powershell
New-Item -ItemType Directory -Path C:\scripts -Force
New-Item -ItemType Directory -Path C:\Logs\s3sync -Force
New-Item -ItemType Directory -Path C:\Temp -Force
```

4. Set execution policy if scripts blocked (run as Admin if needed):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
```

---

# 2) Script to run (save as `C:\scripts\s3sync.ps1`)

This script:

* logs start/end and output to timestamped logs,
* implements a simple lock to avoid concurrent runs,
* retries with exponential backoff,
* supports `-DryRun` to test without uploading.

Save exactly (copy/paste):

```powershell
Param(
  [string]$Source = "C:\data",
  [string]$Bucket = "s3://my-bucket/path",
  [string]$Profile = "mysync",
  [switch]$DryRun,
  [int]$MaxAttempts = 3,
  [int]$BaseDelaySeconds = 10
)

# Log file
$logDir = "C:\Logs\s3sync"
if (-not (Test-Path $logDir)) { New-Item -ItemType Directory -Path $logDir -Force | Out-Null }
$timestamp = Get-Date -Format "yyyyMMdd_HHmmss"
$log = Join-Path $logDir "s3sync_$timestamp.log"

"=== s3 sync start: $(Get-Date -Format o) ===" | Tee-Object -FilePath $log -Append

# Locate aws CLI
$awsPath = (Get-Command aws -ErrorAction SilentlyContinue).Source
if (-not $awsPath) {
  "ERROR: aws CLI not found in PATH. Install AWS CLI v2 and ensure it's in PATH." | Tee-Object -FilePath $log -Append
  exit 10
}

# Simple locking (prevents concurrent runs)
$lock = "C:\Temp\s3sync.lock"
if (Test-Path $lock) {
  "Another instance detected (lock file present). Exiting." | Tee-Object -FilePath $log -Append
  exit 2
}
New-Item -ItemType File -Path $lock -Force | Out-Null

$attempt = 0
$exitCode = 1
while ($attempt -lt $MaxAttempts) {
  $attempt++
  $args = @("s3","sync",$Source,$Bucket,"--exact-timestamps","--delete")
  if ($DryRun) { $args += "--dryrun" }
  if ($Profile) { $args += @("--profile",$Profile) }

  "Attempt $attempt: aws $($args -join ' ')" | Tee-Object -FilePath $log -Append
  & $awsPath @args 2>&1 | Tee-Object -FilePath $log -Append
  $exitCode = $LASTEXITCODE
  "Exit code: $exitCode" | Tee-Object -FilePath $log -Append

  if ($exitCode -eq 0) { break }

  $sleep = [int]($BaseDelaySeconds * [math]::Pow(2, $attempt - 1))
  "Sleeping $sleep seconds before retry..." | Tee-Object -FilePath $log -Append
  Start-Sleep -Seconds $sleep
}

# Remove lock and finish
Remove-Item $lock -Force -ErrorAction SilentlyContinue
"=== s3 sync finished: $(Get-Date -Format o) ExitCode=$exitCode ===" | Tee-Object -FilePath $log -Append

exit $exitCode
```

**Notes:**

* Put the correct `$Source`, `$Bucket`, and `$Profile` when calling the script.
* `--exact-timestamps` + `--delete` are common safe options for sync; remove if you need different behavior.
* Logs go to `C:\Logs\s3sync\`.

---

# 3) Quick manual test (before scheduling)

1. Dry-run (no changes):

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1" -Source "C:\testsrc" -Bucket "s3://my-bucket/test" -Profile "mysync" -DryRun
```

Check the newest log:

```powershell
Get-ChildItem C:\Logs\s3sync\*.log | Sort-Object LastWriteTime -Descending | Select-Object -First 1 | Get-Content -Tail 200
```

2. Real run (upload small sample):

```powershell
New-Item -ItemType File -Path C:\testsrc\hello.txt -Force -Value "hello $(Get-Date)"
powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1" -Source "C:\testsrc" -Bucket "s3://my-bucket/test" -Profile "mysync"
```

Verify on S3:

```powershell
aws s3 ls s3://my-bucket/test --profile mysync
```

---

# 4) Create a Scheduled Task (the "cron" equivalent)

Example: run daily at 05:32. Replace time or create trigger as needed.

```powershell
$script = "C:\scripts\s3sync.ps1"
$action = New-ScheduledTaskAction -Execute "PowerShell.exe" -Argument "-NoProfile -ExecutionPolicy Bypass -WindowStyle Hidden -File `"$script`" -Source `"C:\testsrc`" -Bucket `"s3://my-bucket/test`" -Profile `"mysync`""
$trigger = New-ScheduledTaskTrigger -Daily -At 05:32
$principal = New-ScheduledTaskPrincipal -UserId "$env:USERDOMAIN\$env:USERNAME" -LogonType Interactive
Register-ScheduledTask -TaskName "S3SyncDaily" -Action $action -Trigger $trigger -Principal $principal -Description "Daily S3 sync"
```

If you want to test immediately, create a one-shot trigger for a few minutes from now:

```powershell
$runAt = (Get-Date).AddMinutes(3)
$triggerOnce = New-ScheduledTaskTrigger -Once -At $runAt
Register-ScheduledTask -TaskName "S3Sync_OneOffTest" -Action $action -Trigger $triggerOnce -Principal $principal -Description "One off test"
```

Start it manually:

```powershell
Start-ScheduledTask -TaskName "S3Sync_OneOffTest"
```

---

# 5) How to check task status & results (like `ps | grep`)

Get basic info:

```powershell
Get-ScheduledTask -TaskName "S3SyncDaily" | Select-Object TaskName, State
Get-ScheduledTaskInfo -TaskName "S3SyncDaily" | Select-Object LastRunTime, NextRunTime, LastTaskResult
```

* `LastTaskResult` is the task exit code (0 = success).
* To view recent logs (tail):

```powershell
Get-ChildItem C:\Logs\s3sync\*.log | Sort-Object LastWriteTime -Descending | Select-Object -First 1 | Get-Content -Tail 200
```

See currently running scheduled tasks:

```powershell
Get-ScheduledTask | Where-Object State -eq 'Running' | Select-Object TaskName
```

If you prefer an ad-hoc “grep” by name:

```powershell
Get-ScheduledTask | Where-Object TaskName -match 'S3Sync' | Select-Object TaskName, State
```

---

# 6) Test cases — how to simulate & expected results

**A. Dry-run (safety)**

* Command: use `-DryRun` param (see manual test).
* Expect: log contains `--dryrun` and no S3 changes, exit code `0`.

**B. Normal success**

* Create a small test file, run script.
* Expect: exit code `0`, log includes upload lines, `aws s3 ls` shows file.

**C. Credentials / permission failure**

* Simulate: run script with `-Profile bogusprofile` or temporarily empty env creds:

  ```powershell
  powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1" -Source C:\testsrc -Bucket s3://my-bucket/test -Profile bogusprofile
  ```
* Expect: non-zero exit code; log shows credential error or AccessDenied. ScheduledTask `LastTaskResult` non-zero.

**D. Bucket not found**

* Simulate: set Bucket to `s3://this-bucket-does-not-exist-$(Get-Random)` and run.
* Expect: non-zero exit code; log shows NoSuchBucket / 404.

**E. Network failure (simulate safely)**

* Simulate without disabling NIC by using an invalid endpoint:

  * Edit invocation in script or call:

  ```powershell
  & aws s3 sync C:\testsrc s3://my-bucket/test --profile mysync --endpoint-url http://127.0.0.1:1
  ```

  * Or add `--endpoint-url http://127.0.0.1:1` to the script args temporarily.
* Expect: connection errors in log, non-zero exit, script retries (you’ll see attempts and backoff).

**F. Interrupted large upload / resume**

* Create a big file:

  ```powershell
  fsutil file createnew C:\testsrc\bigfile.bin 200000000
  ```
* Start the script manually; while running, kill the aws process:

  ```powershell
  Get-Process -Name aws | Stop-Process -Force
  ```
* Re-run script; verify the subsequent run either finishes or resumes (AWS CLI uses multipart for big files; re-run will complete upload). Check logs and `aws s3 ls`.

**G. Concurrent runs**

* Start the task twice (Start-ScheduledTask twice) or run script in two shells. The second should exit quickly with the lock message:

```powershell
Start-ScheduledTask -TaskName "S3SyncDaily"
Start-ScheduledTask -TaskName "S3SyncDaily"
# or run script twice manually to test the lock
```

* Expect: one instance does work, second sees `Another instance detected` and exits with code `2`.

**H. Full cycle as scheduled task**

* Create the scheduled task as above with a one-off trigger a few minutes from now, then confirm:

```powershell
Get-ScheduledTaskInfo -TaskName "S3Sync_OneOffTest"
# after run
Get-ScheduledTaskInfo -TaskName "S3Sync_OneOffTest" | Select LastRunTime, LastTaskResult
```

* Check the log file for full output.

---

# 7) Useful troubleshooting snippets

* Show last 50 lines of latest log:

```powershell
Get-ChildItem C:\Logs\s3sync\*.log | Sort-Object LastWriteTime -Descending | Select-Object -First 1 |
  Get-Content -Tail 50
```

* See scheduled task event log (Task Scheduler operational events):

```powershell
Get-WinEvent -LogName "Microsoft-Windows-TaskScheduler/Operational" -MaxEvents 50 |
  Where-Object {$_.Message -match "S3SyncDaily"} | Select-Object TimeCreated, Id, Message -First 10
```

* If `LastTaskResult` ≠ 0, open the corresponding script log — it will contain exit code + aws error text.

---

# 8) Best practices / production tips

* Run task under a user account that has the AWS profile stored, or pass credentials securely (avoid plaintext in script). For EC2 use instance profile.
* Use a dedicated, least-privilege IAM user with only the needed S3 permissions.
* Keep logs for a retention window and periodically archive or rotate them.
* Add monitoring/alerting: you can add a final check that, on non-zero exit, writes an event to Windows Event Log or sends an alert (SMTP/webhook).
* Keep lock file on a local fast volume. Remove stale locks (with timestamp checks) if needed.

---

# 9) Quick checklist to run now

1. Put `s3sync.ps1` into `C:\scripts\`.
2. `aws configure --profile mysync` with test keys.
3. Create `C:\testsrc` and add `hello.txt`.
4. Manual dry-run: run script with `-DryRun`. Inspect log.
5. Manual real run: run script normally. Inspect log and `aws s3 ls`.
6. Create one-off scheduled task (run in 3 minutes). Start and confirm `LastRunTime` + `LastTaskResult`.
7. Run the test cases above (bad profile, bad bucket, endpoint override, concurrent runs). Inspect logs each time.

---

- Add Ons:
> generate the exact Register-ScheduledTask command with your real `$Source`, `$Bucket`, and desired schedule, or
> produce a small wrapper that also emails you on failure (SMTP) or posts to Slack/Teams.



</details>

---

### Clean, minimal & follows the best practices using Windows Powershell.

<details>
  <summary>Theoritical test case for s3 sync command following the best practices</summary>

## 1. Create a PowerShell script

Save this as `C:\scripts\s3sync.ps1`:

```powershell
# Simple daily S3 sync
aws s3 sync "C:\Data\Reports" "s3://my-company-backups/reports/"
```

---

## 2. Test it manually

Open PowerShell and run:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"
```

Check if files appear:

```powershell
aws s3 ls s3://my-company-backups/reports/ --recursive
```

---

## 3. Schedule it in Windows Task Scheduler

Run this in PowerShell to schedule it **daily at 05:32**:

```powershell
$action = New-ScheduledTaskAction -Execute "PowerShell.exe" -Argument "-NoProfile -ExecutionPolicy Bypass -File `"`"C:\scripts\s3sync.ps1`"`""
$trigger = New-ScheduledTaskTrigger -Daily -At 05:32
$principal = New-ScheduledTaskPrincipal -UserId "$env:USERDOMAIN\$env:USERNAME" -LogonType Interactive
Register-ScheduledTask -TaskName "S3DailySync" -Action $action -Trigger $trigger -Principal $principal -Description "Daily sync C:\Data\Reports to S3"
```

---

## 4. Verify it’s running

```powershell
Get-ScheduledTaskInfo -TaskName "S3DailySync" | Select LastRunTime, NextRunTime, LastTaskResult
```

* `LastTaskResult = 0` → success.
* Files will be in your S3 bucket.

---

✨ That’s it. **Clean, minimal, follows best practices:**

* Script is just `aws s3 sync source target`
* Scheduled via Task Scheduler
* Uses AWS CLI’s built-in behavior (timestamps, recursive copy, efficient sync)

---

> **Add Ons:**
> **Make Task Scheduler log output to a file automatically** (instead of adding logging inside the script)? That keeps the script one line, but still gives you logs for troubleshooting.

<details>
  <summary>Explaination of the above tasks line by line</summary>


# 1) Script line — what it literally runs

```powershell
aws s3 sync "C:\Data\Reports" "s3://my-company-backups/reports/"
```

**Token-by-token explanation**

* `aws`
  The AWS CLI executable. It is the program that understands `s3`, `ec2`, etc. When you type `aws` Windows finds `aws.exe` on your PATH and runs it.

* `s3`
  The AWS CLI *service* or namespace. It tells the CLI “I want to work with Amazon S3 (object storage).”

* `sync`
  The specific operation/command under `s3`. `sync` compares source and destination and copies new/changed files. It is recursive by default (it looks inside directories).

* `"C:\Data\Reports"`
  The **source** path on your local machine. Quoted because paths often contain spaces. This is where files are read from.

* `"s3://my-company-backups/reports/"`
  The **destination** S3 URI. Format:

  * `s3://` — the scheme/protocol indicating the resource is in S3.
  * `my-company-backups` — the S3 **bucket name**.
  * `/reports/` — the **prefix** (like a folder inside the bucket). The trailing slash is optional but often used to clarify you mean a prefix (not a single object).

**Behavior notes (why `sync` is used)**

* `aws s3 sync` transfers only new or changed files (it checks size and timestamps).
* It is recursive (copies nested folders).
* It **does not** delete on the destination unless you supply `--delete`.
* For big files it uses multipart uploads to allow large/resumable transfers.

---

# 2) Run the script manually

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"
```

**Token-by-token explanation**

* `powershell`
  The program used to run PowerShell scripts (on older Windows this is Windows PowerShell; on systems with PowerShell 7 you might use `pwsh` instead). This launches a PowerShell process to execute the script.

* `-NoProfile`
  Tell PowerShell **not** to load profile scripts (like `Microsoft.PowerShell_profile.ps1` or user profile). This reduces variability between runs and avoids user customizations affecting the script.

* `-ExecutionPolicy Bypass`
  PowerShell has an execution policy that can block scripts. `Bypass` temporarily ignores that policy for this session so the script can run. **Security note:** use only for trusted scripts.

* `-File "C:\scripts\s3sync.ps1"`
  Tells PowerShell to run the script file at that path. Quoted because the path may have spaces.

**Why use these flags**

* `-NoProfile` + `-ExecutionPolicy Bypass` make the scheduled run more predictable and avoid interactivity or blocking due to policy or profile code.

---

# 3) Quick verification of S3 contents

```powershell
aws s3 ls s3://my-company-backups/reports/ --recursive
```

**Token-by-token**

* `aws` — AWS CLI.
* `s3` — S3 service.
* `ls` — list objects (like `ls` or `dir` but for S3).
* `s3://...` — the bucket/prefix to list.
* `--recursive` — list objects in subfolders recursively.

Use this to confirm files landed in S3 after the run.

---

# 4) Schedule it with PowerShell — create action, trigger, principal, register

Here’s the code you used:

```powershell
$action = New-ScheduledTaskAction -Execute "PowerShell.exe" -Argument "-NoProfile -ExecutionPolicy Bypass -File `"`"C:\scripts\s3sync.ps1`"`""
$trigger = New-ScheduledTaskTrigger -Daily -At 05:32
$principal = New-ScheduledTaskPrincipal -UserId "$env:USERDOMAIN\$env:USERNAME" -LogonType Interactive
Register-ScheduledTask -TaskName "S3DailySync" -Action $action -Trigger $trigger -Principal $principal -Description "Daily sync C:\Data\Reports to S3"
```

---

## 4.1 `New-ScheduledTaskAction` — define *what* will run

```powershell
$action = New-ScheduledTaskAction -Execute "PowerShell.exe" -Argument "-NoProfile -ExecutionPolicy Bypass -File 'C:\scripts\s3sync.ps1'"
```

**What this object is**
`New-ScheduledTaskAction` creates an *action object* — a description of the program that Task Scheduler will launch when the task runs. You don’t launch anything yet; you just build a configuration object and store it in `$action`.

**Tokens**

* `$action =` — store the created action object into variable `$action`.
* `New-ScheduledTaskAction` — the cmdlet that produces an action object.
* `-Execute "PowerShell.exe"` — the program to execute. This is the executable that the task will start.
* `-Argument "...script args..."` — the single string of arguments to pass to `PowerShell.exe`. That string contains `-NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"`.

**Important quoting tip**

* In PowerShell use single quotes to avoid escaping inner double-quotes, e.g.:

  ```powershell
  -Argument '-NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"'
  ```

  That is simpler and easier to read than backtick-escaped quotes.

---

## 4.2 `New-ScheduledTaskTrigger` — define *when* it runs

```powershell
$trigger = New-ScheduledTaskTrigger -Daily -At 05:32
```

**Tokens**

* `$trigger =` — save trigger object to variable `$trigger`.
* `New-ScheduledTaskTrigger` — cmdlet to create a schedule trigger object.
* `-Daily` — trigger type: run the task every day.
* `-At 05:32` — the time of day (HH\:mm) to run the task.

Other alternatives: `-Weekly -DaysOfWeek Monday,Tuesday` or `-Once -At (Get-Date).AddMinutes(5)` for one-off testing.

---

## 4.3 `New-ScheduledTaskPrincipal` — choose the account that runs the task

```powershell
$principal = New-ScheduledTaskPrincipal -UserId "$env:USERDOMAIN\$env:USERNAME" -LogonType Interactive
```

**Tokens & meaning**

* `$principal =` — store the principal object in `$principal`.
* `New-ScheduledTaskPrincipal` — cmdlet to build an account/principal object.
* `-UserId "$env:USERDOMAIN\$env:USERNAME"` — the Windows account under which the task will run.

  * `$env:USERDOMAIN` and `$env:USERNAME` are environment variables for the domain and username of the account that runs your current PowerShell session. Together they produce something like `MYPC\alice`.
* `-LogonType Interactive` — run the task **only when** that user is logged in interactively (i.e., they have an interactive desktop session).

  * **Interactive** = no password stored in scheduler, runs in the user's session.
  * If you need the task to run when the user is not logged in, you would use `-LogonType Password` (the task stores credentials). For domain-less systems you can use the `SYSTEM` account or service accounts depending on requirement.

**Note:** If you choose `Interactive`, the scheduled job will run in the user’s session and may require that the user is logged in at the scheduled time.

---

## 4.4 `Register-ScheduledTask` — create the task in Task Scheduler

```powershell
Register-ScheduledTask -TaskName "S3DailySync" -Action $action -Trigger $trigger -Principal $principal -Description "Daily sync C:\Data\Reports to S3"
```

**Tokens**

* `Register-ScheduledTask` — cmdlet that actually writes the task into Windows Task Scheduler.
* `-TaskName "S3DailySync"` — the friendly name of the task (visible in Task Scheduler GUI).
* `-Action $action` — wire the action object (what to run).
* `-Trigger $trigger` — wire the trigger object (when to run).
* `-Principal $principal` — who will run it.
* `-Description "..."` — human-readable description visible in Task Scheduler.

After this runs, the task exists and will run based on the trigger.

---

# 5) Check task status and results

```powershell
Get-ScheduledTaskInfo -TaskName "S3DailySync" | Select LastRunTime, NextRunTime, LastTaskResult
```

**Tokens**

* `Get-ScheduledTaskInfo -TaskName "S3DailySync"` — query Task Scheduler for runtime info about that task (last run time, run result, next scheduled run).
* `|` — pipeline: send the output of the left command to the right command for further processing.
* `Select LastRunTime, NextRunTime, LastTaskResult` — pick only those three fields to display.

**What `LastTaskResult` means**

* `LastTaskResult` is a numeric exit/result code from the last run.

  * `0` is success (most of the time).
  * Non-zero indicates some kind of error — check your script log or Event Viewer for details. The code is often the exit code of the process you launched (PowerShell/your script) but Task Scheduler may also have its own codes for scheduler-level failures.

---

# 6) Cleaner quoting example you can copy/paste (recommended)

Use single quotes for the `-Argument` so you don’t have to escape quotes:

```powershell
$action = New-ScheduledTaskAction -Execute "PowerShell.exe" -Argument '-NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"'
$trigger = New-ScheduledTaskTrigger -Daily -At 05:32
$principal = New-ScheduledTaskPrincipal -UserId "$env:USERDOMAIN\$env:USERNAME" -LogonType Interactive
Register-ScheduledTask -TaskName "S3DailySync" -Action $action -Trigger $trigger -Principal $principal -Description "Daily sync C:\Data\Reports to S3"
```

---

# 7) Practical gotchas & recommendations (short)

* **AWS credentials & scheduled task account**: The scheduled task runs as the account you configure in the principal. Make sure that account has the AWS CLI profile (run `aws configure --profile <name>`) or has AWS environment variables set, or the script uses a full `--profile` argument to point to an existing profile. If you run as a different user than you used to configure AWS, the profile will not exist for that user unless you configure it for them.
* **Run whether user is logged on**: If you want the task to run when nobody’s logged in, create the principal with `-LogonType Password` and supply credentials (this will store the password). For machine-level tasks consider running under a service account or `SYSTEM` depending on security requirements.
* **Logs**: Add logging inside your script (redirect `stdout/stderr` or use `Tee-Object` to a file) because Task Scheduler output can be limited. Your earlier script with timestamped logs is perfect.
* **Permissions**: Ensure the account running the task can read the source files and write the log directory.
* **ExecutionPolicy**: `Bypass` is convenient but be aware of policy implications. Only run trusted scripts.
* **Quoting**: When building the `-Argument` string, keep it as one string. If you need nested quotes for paths, prefer single quotes around the entire `-Argument` string and double quotes around the internal path.
* **Task history**: enable Task Scheduler history or check `Get-WinEvent -LogName "Microsoft-Windows-TaskScheduler/Operational"` to debug scheduling failures.

---

# TL;DR (one-paragraph)

* `aws s3 sync "local" "s3://bucket/prefix/"` = copy new/changed files from the local folder to S3.
* `powershell -NoProfile -ExecutionPolicy Bypass -File "C:\scripts\s3sync.ps1"` = start PowerShell in a clean state and run the script file.
* `New-ScheduledTaskAction/Trigger/Principal` create objects describing *what* runs, *when*, and *who* runs it.
* `Register-ScheduledTask` writes that configuration into Task Scheduler.
* Check status with `Get-ScheduledTaskInfo` and logs inside your script for detailed errors.

---

> Add Ons:
* show the exact `Register-ScheduledTask` command to run the task **whether the user is logged on or not** (with the correct `-LogonType` and secure handling of credentials), or
* produce a one-liner `schtasks` equivalent if you prefer the older `schtasks.exe` syntax.

  
</details>

  
</details>

### Clean, minimal & follows the best practices using Task Scehduler and CMD not using Windows Powershell.

<details>
  <summary>Theoritical test case for s3 sync command following the best practices</summary>

Nice — below I’ll show **how to do the whole thing using only Task Scheduler (no PowerShell)**. I give you:

1. A small **batch wrapper** that reproduces the important behavior (logging, lock to avoid concurrent runs, retries with exponential backoff, exit codes).
2. Exact **Task Scheduler (GUI) steps** that call that batch file.
3. A **`schtasks.exe`** one-line example to create the same task from CMD (no PowerShell).
4. How to **test, inspect logs, and troubleshoot**.

---

# A — Batch wrapper (put this in `C:\scripts\s3sync.bat`)

This is the recommended way if you want to avoid PowerShell entirely but still have logging, locking and retries.

Save exactly as a plain text file `C:\scripts\s3sync.bat`:

```bat
@echo off
REM Simple S3 sync wrapper (batch) with lock, logging, retries

setlocal enabledelayedexpansion

REM === Config ===
set "SOURCE=C:\Data\Reports"
set "BUCKET=s3://my-company-backups/reports/"
set "PROFILE=mysync"
set "LOGDIR=C:\Logs\s3sync"
set "LOCK=C:\Temp\s3sync.lock"
set "MAX_ATTEMPTS=3"
set "BASE_DELAY=10"
set "AWSPATH=C:\Program Files\Amazon\AWSCLI\bin\aws.exe"
REM === End config ===

if not exist "%LOGDIR%" mkdir "%LOGDIR%"

REM Create readable timestamp using WMIC (format: YYYYMMDD_HHMMSS)
for /f "tokens=2 delims==." %%a in ('wmic os get LocalDateTime /value 2^>nul') do set "LDT=%%a"
if defined LDT (
  set "TIMESTAMP=%LDT:~0,8%_%LDT:~8,6%"
) else (
  REM fallback if WMIC unavailable
  for /f "tokens=1-3 delims=/ " %%a in ('date /t') do set "DATEPART=%%c%%a%%b"
  for /f "tokens=1-2 delims=:." %%a in ('time /t') do set "TIMEPART=%%a%%b"
  set "TIMESTAMP=%DATEPART%_%TIMEPART%"
)

set "LOG=%LOGDIR%\s3sync_%TIMESTAMP%.log"
echo === s3 sync start: %DATE% %TIME% === >> "%LOG%"

REM Check aws executable exists (use full path to avoid PATH issues)
if not exist "%AWSPATH%" (
  echo ERROR: aws CLI not found at "%AWSPATH%". Ensure aws.exe path is correct. >> "%LOG%"
  exit /b 10
)

REM Lock check to avoid concurrent runs
if exist "%LOCK%" (
  echo Another instance detected (lock file present). Exiting. >> "%LOG%"
  exit /b 2
)
echo %TIMESTAMP% > "%LOCK%"

set "ATTEMPT=0"
set "DELAY=%BASE_DELAY%"
set "EXITCODE=1"

:RETRY_LOOP
set /a ATTEMPT+=1
echo ------------------------------ >> "%LOG%"
echo Attempt %ATTEMPT%: "%AWSPATH%" s3 sync "%SOURCE%" "%BUCKET%" --exact-timestamps --delete --profile %PROFILE% >> "%LOG%"
"%AWSPATH%" s3 sync "%SOURCE%" "%BUCKET%" --exact-timestamps --delete --profile %PROFILE% >> "%LOG%" 2>&1
set "EXITCODE=%ERRORLEVEL%"
echo Exit code: %EXITCODE% >> "%LOG%"

if "%EXITCODE%"=="0" goto FINISH
if %ATTEMPT% geq %MAX_ATTEMPTS% goto FINISH

echo Sleeping %DELAY% seconds before retry... >> "%LOG%"
timeout /t %DELAY% /nobreak >nul
set /a DELAY=%DELAY%*2
goto RETRY_LOOP

:FINISH
del "%LOCK%" >nul 2>&1
echo === s3 sync finished: %DATE% %TIME% ExitCode=%EXITCODE% === >> "%LOG%"
exit /b %EXITCODE%
```

**Why this file exists**

* Task Scheduler will **launch the `.bat`**, which runs `aws.exe`.
* The batch script performs the important bookkeeping (timestamped log, lock, retries), which Task Scheduler alone cannot easily do.

---

# B — Create the task using the Task Scheduler GUI (step-by-step, no PowerShell)

1. Open **Task Scheduler** (Start → type “Task Scheduler” → Enter).

2. In the right-hand Actions pane click **Create Task…** (do **not** use “Create Basic Task” if you want full options).

3. **General tab**

   * **Name:** `S3DailySync`
   * **Description:** `Daily sync C:\Data\Reports -> s3://my-company-backups/reports/`
   * **Security options:**

     * **Choose user/account**: pick the Windows account that has the AWS CLI profile configured (see notes below).
     * If you want the task to run even when no one is logged on: select **"Run whether user is logged on or not"** (you will be prompted for the account password when saving).
     * Check **"Run with highest privileges"** if your sync requires elevated file access.
   * **Configure for:** choose your OS (e.g. Windows 10/Windows Server 2016).

4. **Triggers tab**

   * Click **New…**
   * **Begin the task:** On a schedule
   * **Settings:** Daily
   * **Start:** `05:32:00` (or your preferred time)
   * Click **OK**.

5. **Actions tab**

   * Click **New…**
   * **Action:** Start a program
   * **Program/script:** `C:\scripts\s3sync.bat`
     (Alternatively: `cmd.exe` and put `/c "C:\scripts\s3sync.bat"` in the *Add arguments* field — either works. For simplicity, use the `.bat` path directly.)
   * **Start in (optional):** `C:\scripts` (optional but can help relative paths)
   * Click **OK**.

6. **Conditions tab** (optional)

   * Uncheck **"Start the task only if the computer is on AC power"** if you want it to run on battery (for laptops).
   * Leave defaults or tweak per environment.

7. **Settings tab**

   * Check **"Allow task to be run on demand"** (handy to test).
   * For **If the task is already running, then the following rule applies:** choose **Do not start a new instance** (this protects against overlapping runs).
   * Optionally set **Stop the task if it runs longer than:** e.g. 4 hours.
   * Click **OK**. If you chose “Run whether user is logged on or not” you’ll be asked to provide the account password to register the task.

8. After creation: right-click the task → **Run** to test immediately. Inspect the log file created in `C:\Logs\s3sync\` for details.

---

# C — Create the same task purely from CMD using `schtasks.exe` (no PowerShell)

Open an elevated Command Prompt (Run as Administrator) and run (adjust user/password as needed):

```cmd
schtasks /Create /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /SC DAILY /ST 05:32 /RU "MYDOMAIN\BackupUser" /RP "P@ssw0rd!" /RL HIGHEST /F
```

**Fields explained**

* `/Create` → create a new task.
* `/TN "S3DailySync"` → task name.
* `/TR "C:\scripts\s3sync.bat"` → program to run (full path).
* `/SC DAILY` → schedule type = daily.
* `/ST 05:32` → start time.
* `/RU "user"` and `/RP "password"` → run as this user; for local SYSTEM account use `/RU "SYSTEM"` and omit `/RP`.
* `/RL HIGHEST` → run with highest privileges.
* `/F` → force create/overwrite existing task with same name.

**Quick control commands**

* Start now: `schtasks /Run /TN "S3DailySync"`
* Query: `schtasks /Query /TN "S3DailySync" /V /FO LIST`
* Delete: `schtasks /Delete /TN "S3DailySync" /F`

---

# D — How to test & inspect results (no PowerShell)

1. Manual run (CMD):

   ```cmd
   C:\scripts\s3sync.bat
   ```

   or via Task Scheduler:

   ```cmd
   schtasks /Run /TN "S3DailySync"
   ```

2. View the latest log file:

   * Open File Explorer → go to `C:\Logs\s3sync\` → open the newest `s3sync_*.log` in Notepad (double click).
   * Or from CMD:

     ```cmd
     dir /O:-D C:\Logs\s3sync\*.log
     type C:\Logs\s3sync\s3sync_YYYYMMDD_HHMMSS.log | more
     ```

     (replace filename with the real one or use the GUI to see the newest)

3. Check Task Scheduler status:

   * In GUI: Select the task and look at **Last Run Time** and **Last Run Result**.
   * From CMD:

     ```cmd
     schtasks /Query /TN "S3DailySync" /V /FO LIST
     ```

4. Check S3 contents:

   * If you want a quick check from the same account:

     ```cmd
     "C:\Program Files\Amazon\AWSCLI\bin\aws.exe" s3 ls s3://my-company-backups/reports/ --profile mysync --recursive
     ```

---

# E — Important notes & gotchas

1. **AWS credentials for the scheduled account**
   The task runs under the Windows account you specify. AWS CLI looks for credentials under that user’s `%USERPROFILE%\.aws\credentials`. Make sure you run `aws configure --profile mysync` **for that Windows user** (or place a shared credentials file and configure the environment variable `AWS_SHARED_CREDENTIALS_FILE` for the service account). If you schedule the task under `SYSTEM`, you must provide credentials in a way `SYSTEM` can read (system env vars or a shared credentials file).

2. **Full path to `aws.exe`**
   Use the full path in the batch (`AWSPATH` variable) because Task Scheduler’s environment/path may differ from your interactive shell.

3. **Permissions**
   The account that runs the task needs read access to the source folder and write access to the log folder.

4. **Locking vs Task Scheduler instance policy**
   In the batch we use a lock file to prevent concurrent runs. Task Scheduler also has a “Do not start a new instance” setting — using both is safe and gives defense-in-depth.

5. **Log rotation**
   The batch creates timestamped logs. Add a cleanup scheduled task (or a simple cleanup step) to delete logs older than X days if needed.

6. **Exit codes**
   The batch returns non-zero exit codes on error; Task Scheduler **Last Run Result** will show that numeric code. Inspect the log file and AWS error messages to know what failed.

7. **Network errors / retries**
   The batch includes retries with exponential backoff. You can tune `MAX_ATTEMPTS` and `BASE_DELAY` in the script.

---

# F — Quick troubleshooting checklist

* If `Last Run Result` is non-zero:

  * Open the newest `C:\Logs\s3sync\*.log`.
  * Ensure `aws.exe` path in the batch is correct.
  * Ensure the Windows user running the task has the AWS profile configured — run `aws configure --profile mysync` as that user.
  * If you used `Run whether user is logged on or not` and the task failed to start, re-enter the password (Task Scheduler will prompt when editing and saving).
* If no logs are created:

  * Verify `Start in` or full path in the Action is correct and that the task can read/write `C:\Logs\s3sync`.
* To debug interactively: run the batch manually in an elevated CMD so you can see output and errors instantly.

---

> Add Ons:
* produce a **minimal `.bat`** that also supports a `--DryRun` toggle via a command-line arg (so you can run `s3sync.bat dryrun`), or
* give you the exact `schtasks` command to run as `SYSTEM` (if that's your desired account), or
* show how to put AWS credentials in a shared file and set `AWS_SHARED_CREDENTIALS_FILE` for the scheduled task.

</details>

---

### Only using CMD.

<details>
  <summary>Theoritical test case for s3 sync command following the best practices</summary>

Yes — you can do this **entirely from CMD** (no PowerShell, no GUI) by using a batch wrapper + `schtasks.exe`. Below I give you a complete, copy-pasteable step-by-step plan:

* create the folders and credentials,
* create the batch script (with logging, lock, retries, dry-run),
* configure credentials (interactive `aws configure` or a shared file usable by `SYSTEM`),
* schedule with `schtasks /Create`,
* run & test from CMD,
* simulate failure cases,
* inspect logs & Task Scheduler state,
* change or delete the task with `schtasks`.

I’ll explain each command/flag so you know what every word means.

---

# 0) Assumptions & prerequisites (quick)

* Windows machine with Administrator rights to create scheduled tasks (or ability to create tasks for your user).
* AWS CLI v2 installed and `aws` available in PATH (you can check from CMD with `aws --version`).
* You want a pure CMD workflow (`.bat` + `schtasks` + standard Windows commands).

Check AWS CLI from CMD:

```cmd
aws --version
where aws
```

* `aws --version` prints CLI version.
* `where aws` shows path(s) to the `aws` executable.

---

# 1) Create needed folders (run in an elevated CMD if needed)

```cmd
mkdir C:\scripts
mkdir C:\Logs\s3sync
mkdir C:\Temp
```

* `mkdir` creates directories. These hold the script, logs, and lock file.

---

# 2) Create the batch script (recommended: edit with Notepad from CMD)

Open Notepad from CMD and paste the script (this avoids many awkward `echo` lines):

```cmd
notepad C:\scripts\s3sync.bat
```

Paste the exact contents below into Notepad and save.

---

### Copy/paste this batch file into `C:\scripts\s3sync.bat`

```bat
@echo off
REM s3sync.bat - Batch wrapper for aws s3 sync with logging, lock, retries and dry-run support
setlocal enabledelayedexpansion

REM ===== CONFIG - edit these as needed =====
set "SOURCE=C:\Data\Reports"
set "BUCKET=s3://my-company-backups/reports/"
set "PROFILE=mysync"
set "LOGDIR=C:\Logs\s3sync"
set "LOCK=C:\Temp\s3sync.lock"
set "MAX_ATTEMPTS=3"
set "BASE_DELAY=10"
REM If you want the script to use a shared credentials file (for SYSTEM), set AWS_SHARED_CREDENTIALS_FILE below:
REM set "AWS_SHARED_CREDENTIALS_FILE=C:\aws\credentials"
REM =========================================

REM Find aws executable if possible (uses PATH). If not found, fallback can be set above manually.
for /f "delims=" %%i in ('where aws 2^>nul') do set "AWSPATH=%%i"
if not defined AWSPATH (
  REM Common default path - change if your aws is installed elsewhere
  set "AWSPATH=C:\Program Files\Amazon\AWSCLI\bin\aws.exe"
)

if not exist "%AWSPATH%" (
  echo ERROR: aws CLI not found at "%AWSPATH%". Ensure aws is installed and in PATH. >&2
  exit /b 10
)

REM Parse optional first argument - if "dryrun" then pass --dryrun to aws
set "DRYFLAG="
if /I "%~1"=="dryrun" set "DRYFLAG=--dryrun"

if not exist "%LOGDIR%" mkdir "%LOGDIR%"

REM Create timestamp (YYYYMMDD_HHMMSS) using WMIC (works on many Windows versions)
for /f "tokens=2 delims==." %%a in ('wmic os get LocalDateTime /value 2^>nul') do set "LDT=%%a"
if defined LDT (
  set "TIMESTAMP=%LDT:~0,8%_%LDT:~8,6%"
) else (
  REM fallback: crude timestamp if WMIC not available
  for /f "tokens=1-2 delims= " %%a in ('echo %date% %time%') do set "TMPDT=%%a_%%b"
  set "TIMESTAMP=%TMPDT::=%"
  set "TIMESTAMP=%TIMESTAMP: =_%"
)

set "LOG=%LOGDIR%\s3sync_%TIMESTAMP%.log"
echo === s3 sync start: %DATE% %TIME% === >> "%LOG%"

REM Lock to prevent concurrent runs
if exist "%LOCK%" (
  echo Another instance detected (lock file present). Exiting. >> "%LOG%"
  exit /b 2
)
echo %TIMESTAMP% > "%LOCK%"

set /a ATTEMPT=0
set EXITCODE=1
set DELAY=%BASE_DELAY%

:RETRY_LOOP
set /a ATTEMPT+=1
echo ------------------------------ >> "%LOG%"
echo Attempt %ATTEMPT%: "%AWSPATH%" s3 sync "%SOURCE%" "%BUCKET%" --exact-timestamps --delete %DRYFLAG% --profile %PROFILE% >> "%LOG%"
"%AWSPATH%" s3 sync "%SOURCE%" "%BUCKET%" --exact-timestamps --delete %DRYFLAG% --profile %PROFILE% >> "%LOG%" 2>&1
set "EXITCODE=%ERRORLEVEL%"
echo Exit code: %EXITCODE% >> "%LOG%"

if "%EXITCODE%"=="0" goto FINISH
if %ATTEMPT% geq %MAX_ATTEMPTS% goto FINISH

echo Sleeping %DELAY% seconds before retry... >> "%LOG%"
timeout /t %DELAY% /nobreak >nul
set /a DELAY=%DELAY%*2
goto RETRY_LOOP

:FINISH
del "%LOCK%" >nul 2>&1
echo === s3 sync finished: %DATE% %TIME% ExitCode=%EXITCODE% === >> "%LOG%"
exit /b %EXITCODE%
```

**What this does**

* Creates timestamped logs (`C:\Logs\s3sync\...`).
* Prevents concurrent runs via a lock file (`C:\Temp\s3sync.lock`).
* Retries up to `MAX_ATTEMPTS` with exponential backoff (`BASE_DELAY` doubled each retry).
* Supports `dryrun` when you call `s3sync.bat dryrun`.
* Uses `--exact-timestamps` and `--delete` options for `aws s3 sync` (edit if you want different behaviour).
* Returns non-zero exit codes for Task Scheduler to record.

---

# 3) Configure AWS credentials entirely from CMD

Two options: interactive `aws configure` for a user, or create a shared credentials file for `SYSTEM` or other accounts.

## Option A — configure for the user account (interactive)

Run in CMD as the user who will run the scheduled task:

```cmd
aws configure --profile mysync
```

You’ll be prompted for:

* AWS Access Key ID
* AWS Secret Access Key
* Default region name
* Default output format (you can press Enter for json)

**Meaning**

* This writes `%USERPROFILE%\.aws\credentials` and `%USERPROFILE%\.aws\config` for that user. The batch uses `--profile mysync` to pick these credentials.

## Option B — create a shared credentials file for SYSTEM or another account (non-interactive CMD)

If you plan to run the task as `SYSTEM` or don't want to store creds in a user profile, create a shared credentials file and restrict its ACLs.

**Create folder & file (replace `AKIA...` and `secret` with your keys):**

```cmd
mkdir C:\aws
(
  echo [mysync]
  echo aws_access_key_id=AKIAREPLACEWITHKEY
  echo aws_secret_access_key=REPLACE_WITH_SECRET
  echo region=us-east-1
) > C:\aws\credentials
```

**Secure the file so only SYSTEM and Administrators can read:**

```cmd
icacls C:\aws /inheritance:r
icacls C:\aws /grant "NT AUTHORITY\SYSTEM:R"
icacls C:\aws /grant "BUILTIN\Administrators:R"
icacls C:\aws /remove "Users"
```

(Adjust ACLs as per your security policy.)

**Tell the batch to use that file**
Either uncomment / add the line in the batch script near top:

```bat
set "AWS_SHARED_CREDENTIALS_FILE=C:\aws\credentials"
```

or set it inside the scheduled task environment (below I show how the batch can set it itself).

**Security note:** storing long-lived keys on disk has risks. If possible prefer short-lived credentials, instance profiles, or a service account with least privilege.

---

# 4) Test the batch manually (from CMD)

Dry-run (no changes):

```cmd
C:\scripts\s3sync.bat dryrun
```

Real run:

```cmd
C:\scripts\s3sync.bat
```

Check newest log (list newest files):

```cmd
dir /b /o:-d C:\Logs\s3sync\*.log
```

Open latest log (use the filename returned above):

```cmd
type C:\Logs\s3sync\s3sync_20250820_053200.log | more
```

(Replace file name with the actual one.)

---

# 5) Create the scheduled task from CMD with `schtasks.exe` (no PowerShell)

### Option 1 — Run as a specific Windows user (task will run whether user logged on or not)

This will prompt you to enter the password (or you can include password after `/RP`, but that stores it in scheduler):

```cmd
schtasks /Create /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /SC DAILY /ST 05:32 /RU "MYDOMAIN\BackupUser" /RP "P@ssw0rd!" /RL HIGHEST /F
```

### Option 2 — Run as SYSTEM (no password required)

```cmd
schtasks /Create /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /SC DAILY /ST 05:32 /RU "SYSTEM" /RL HIGHEST /F
```

If using `SYSTEM`, ensure your `C:\aws\credentials` file exists and is readable by `SYSTEM` (see step 3 Option B) **or** the batch sets `AWS_SHARED_CREDENTIALS_FILE`.

---

### `schtasks` tokens explained (word-by-word)

* `schtasks` — the Windows command-line tool to create/query/modify scheduled tasks.
* `/Create` — create a new task.
* `/TN "S3DailySync"` — Task Name (friendly name). Put it in quotes if it has spaces.
* `/TR "C:\scripts\s3sync.bat"` — TaskRun: command that will be executed when the task runs; here it points to the batch file (full path recommended).
* `/SC DAILY` — Schedule type; `DAILY` means every day. Other options: ONCE, WEEKLY, MONTHLY, MINUTE, HOURLY.
* `/ST 05:32` — Start Time (HH\:mm, 24-hour).
* `/RU "MYDOMAIN\BackupUser"` — Run as User account. Use `SYSTEM` to run as the local System account.
* `/RP "P@ssw0rd!"` — Run Password — the password for the `/RU` account. Omit when `/RU SYSTEM`.
* `/RL HIGHEST` — Run Level: `HIGHEST` runs with highest privileges (elevated). Alternatives: LIMITED.
* `/F` — Force: overwrite existing task with same name without confirmation.

---

# 6) Start, query, change, and delete tasks from CMD

Start task now:

```cmd
schtasks /Run /TN "S3DailySync"
```

Query task details:

```cmd
schtasks /Query /TN "S3DailySync" /V /FO LIST
```

* `/V` verbose
* `/FO LIST` format as list (easy to read)

Change a task (example: change start time to 03:00 or change the action):

```cmd
REM Change only the start time
schtasks /Change /TN "S3DailySync" /ST 03:00

REM Change the action (TaskRun) to pass an argument (e.g., dryrun)
schtasks /Change /TN "S3DailySync" /TR "C:\scripts\s3sync.bat dryrun"
```

Delete the task:

```cmd
schtasks /Delete /TN "S3DailySync" /F
```

**Note:** `/Change` supports a subset of properties (time, runas, runlevel, taskrun). For complex updates, delete and `Create` again or use an XML import.

---

# 7) Test cases & how to simulate (all from CMD)

Below are ways to simulate the important real-world cases and what to expect.

## A. Dry-run

```cmd
C:\scripts\s3sync.bat dryrun
```

Expect: log contains `--dryrun` lines, no S3 changes, exit code 0.

## B. Normal success

Create test file and run:

```cmd
echo hello > C:\Data\Reports\hello.txt
C:\scripts\s3sync.bat
```

Expect: `Exit code: 0` in the log and `aws s3 ls` will show object:

```cmd
aws s3 ls s3://my-company-backups/reports/ --profile mysync --recursive
```

## C. Bad credentials / permissions

* Option 1: Run with a nonexistent profile:

  ```cmd
  REM temporarily set PROFILE to bogus in the batch by editing the file, or run aws directly:
  "C:\Program Files\Amazon\AWSCLI\bin\aws.exe" s3 sync "C:\Data\Reports" s3://my-company-backups/reports/ --profile bogusprofile
  ```
* Option 2: Rename the credentials file `C:\aws\credentials` (if using shared).
  Expect: `AccessDenied` or credential error in the log; non-zero exit code.

## D. Bucket not found

```cmd
"C:\Program Files\Amazon\AWSCLI\bin\aws.exe" s3 sync "C:\Data\Reports" s3://this-bucket-does-not-exist-12345 --profile mysync
```

Expect: `NoSuchBucket` / 404 message in log; non-zero exit.

## E. Network failure (safe simulation)

Run the sync with an invalid endpoint to force connection failures:

```cmd
"C:\Program Files\Amazon\AWSCLI\bin\aws.exe" s3 sync "C:\Data\Reports" s3://my-company-backups/reports/ --profile mysync --endpoint-url http://127.0.0.1:1
```

Expect: connection errors in log and the batch retries (see Attempt 1,2... and backoff).

## F. Interrupted large upload (manual)

* Create a large file:

  ```cmd
  fsutil file createnew C:\Data\Reports\bigfile.bin 200000000
  ```
* Start the batch in a separate CMD window:

  ```cmd
  C:\scripts\s3sync.bat
  ```
* While `aws` runs, find and kill the aws process:

  ```cmd
  tasklist | findstr aws
  taskkill /IM aws.exe /F
  ```
* Re-run the batch:

  ```cmd
  C:\scripts\s3sync.bat
  ```

Expect: AWS CLI will use multipart uploads; re-run should finish the upload or resume; logs show progress.

## G. Concurrent runs

Start the task twice rapidly:

```cmd
C:\scripts\s3sync.bat
C:\scripts\s3sync.bat
```

The second run should detect the lock file and exit with code `2`. Log will contain `Another instance detected`.

---

# 8) Inspecting logs & scheduler events (CMD)

List logs (newest first):

```cmd
dir /O:-D C:\Logs\s3sync\*.log
```

Show the latest log:

```cmd
for /f "delims=" %f in ('dir /b /o:-d C:\Logs\s3sync\*.log') do @type "C:\Logs\s3sync\%f" & goto :done
:done
```

(If used inside a `.bat` file, double `%` for the loop variable: `%%f`.)

View Task Scheduler operational events (Task Scheduler history) via `wevtutil` (search for the task name in messages):

```cmd
wevtutil qe "Microsoft-Windows-TaskScheduler/Operational" /c:50 /f:text | findstr /I "S3DailySync"
```

* `wevtutil qe` queries the event log.
* `/c:50` returns up to 50 events.
* `findstr` filters by the task name.

Also you can use:

```cmd
schtasks /Query /TN "S3DailySync" /V /FO LIST
```

to see `Last Run Time` and `Last Result`.

---

# 9) Modify task: change time, action, or user (CMD)

Change start time:

```cmd
schtasks /Change /TN "S3DailySync" /ST 03:00
```

Change the command the task runs (pass dry-run):

```cmd
schtasks /Change /TN "S3DailySync" /TR "C:\scripts\s3sync.bat dryrun"
```

Change run-as user/password (re-create recommended if complex):

```cmd
schtasks /Create /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /SC DAILY /ST 05:32 /RU "MYDOMAIN\BackupUser" /RP "NewPassword!" /RL HIGHEST /F
```

(Using `/Create /F` will overwrite the existing task.)

---

# 10) Best practices & security notes (CMD-oriented)

* Use the **least-privilege IAM** credentials for S3 access.
* Prefer running task under a dedicated service account (not an interactive user).
* If you must store credentials on disk, use a shared file and restrict ACLs (`icacls`) to only the accounts that must access it.
* Keep `aws` path absolute in the batch to avoid PATH issues under Task Scheduler.
* Use timestamped logs and rotate or delete old logs periodically.
* Use the lock file and Task Scheduler option “If the task is already running: Do not start a new instance” (you can set this in GUI — for pure CMD you can recreate the task with XML specifying the behavior; easier: keep locking in the batch).
* Monitor non-zero `Last Run Result` values and send alerts if important (you can extend the batch to send an email or log an event with `eventcreate`).

---

# 11) Quick checklist — copy/paste to run now from CMD

```cmd
REM 1) Make folders
mkdir C:\scripts
mkdir C:\Logs\s3sync
mkdir C:\Temp

REM 2) Create the batch (open Notepad, paste batch code)
notepad C:\scripts\s3sync.bat

REM 3) Configure AWS profile interactively for the user who will run the task:
aws configure --profile mysync

REM 4) Test dry-run:
C:\scripts\s3sync.bat dryrun

REM 5) Test real run:
C:\scripts\s3sync.bat

REM 6) Create scheduled task (run as SYSTEM or specify user+password)
schtasks /Create /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /SC DAILY /ST 05:32 /RU "SYSTEM" /RL HIGHEST /F

REM 7) Start now to test scheduled run:
schtasks /Run /TN "S3DailySync"

REM 8) Query status:
schtasks /Query /TN "S3DailySync" /V /FO LIST
```

---

# 12) Final notes / quick answers to likely follow-ups

* If you want the task created for a domain account but you **don’t want to include the password on the command line**, run the `schtasks /Create` without `/RP` — Windows will prompt for it, or create via GUI.
* If you want to run even when the user isn’t logged on, you must provide credentials (or use `SYSTEM`).
* If you’d like, I can produce the **exact `schtasks` XML** (create /delete via XML import), which gives you even finer control (task history limits, multiple triggers, start boundary, stop boundary). Tell me whether you want the task as `SYSTEM` (recommended for server automation) or as a specific domain/local user so I tailor the credentials/ACL guidance.

---

> Add Ons:
* produce the final `C:\scripts\s3sync.bat` file with your exact `SOURCE` and `BUCKET` values substituted, and show the exact `schtasks` command to create the task as `SYSTEM` or as your user (pick one), **or**
* give you the `schtasks` XML export so you can re-import the exact same task on other machines.

</details>

---

### Clean, Minimal and Follows Best Practices using CMD

<details>
  <summary>Theoritical test case for s3 sync command following the best practices</summary>

Got it 👍 — if you want **only CMD (Command Prompt)** and not PowerShell, here’s the **clean + best-practice** way:

---

## 1. Create a batch file

Save as `C:\scripts\s3sync.bat`:

```bat
@echo off
aws s3 sync "C:\Data\Reports" "s3://my-company-backups/reports/"
```

That’s the **entire script** — clean, just `aws s3 sync`.

---

## 2. Test manually

Open **CMD** and run:

```cmd
C:\scripts\s3sync.bat
```

Check S3:

```cmd
aws s3 ls s3://my-company-backups/reports/ --recursive
```

---

## 3. Schedule it with Task Scheduler (CMD version)

In CMD, register the task to run daily at 05:32:

```cmd
SCHTASKS /Create /SC DAILY /TN "S3DailySync" /TR "C:\scripts\s3sync.bat" /ST 05:32
```

---

## 4. Verify scheduled task

```cmd
SCHTASKS /Query /TN "S3DailySync" /V /FO LIST
```

---

## 5. Logging (optional, still clean)

If you want logs without touching the `.bat`, update the task with output redirection:

```cmd
SCHTASKS /Create /SC DAILY /TN "S3DailySync" /TR "cmd.exe /c C:\scripts\s3sync.bat >> C:\Logs\s3sync.log 2>&1" /ST 05:32 /F
```

Then view logs:

```cmd
type C:\Logs\s3sync.log
```

---

✅ That way:

* Batch script = **1 line clean**
* Scheduling = via `SCHTASKS` (native CMD tool)
* Logging = optional, handled outside script

---

> Add Ons
We can make the **log file rotate daily in CMD** (like `s3sync_20250820.log`) so we don’t overwrite.


</details>  
