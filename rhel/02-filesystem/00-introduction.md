# Introduction to RHEL Filesystem

## What is a Filesystem?

- A filesystem is a method and data structure that an operating system uses to control how data is stored and retrieved on a storage device.
- Without a filesystem, data placed in a storage medium would be one large block of data with no way to tell where one piece of information stops and the next begins.
- By organizing data into files, which are then grouped into directories (also known as folders), filesystems make it easy to find and access the data you need.
- Filesystems also manage metadata, which includes information about files such as their size, type, permissions, and timestamps.
- Different filesystems have different features, performance characteristics, and limitations.
- Common types of filesystems include ext4, XFS, Btrfs, NTFS, and FAT32.

## Linux Filesystem Standards

- Linux filesystems adhere to certain standards to ensure compatibility and interoperability across different distributions and systems.
- The most widely adopted standard is the Filesystem Hierarchy Standard (FHS), which defines the directory structure and directory contents in Unix-like operating systems.
- According to FHS, the root directory is denoted by a single forward slash (`/`), and all other directories and files are organized under this root.
- Key directories defined by FHS include:
  - `/bin`: Essential command binaries
  - `/boot`: Static files of the boot loader
  - `/dev`: Device files
  - `/etc`: Host-specific system configuration
  - `/home`: User home directories
  - `/lib`: Essential shared libraries and kernel modules
  - `/opt`: Optional application software packages
  - `/usr`: Secondary hierarchy for read-only user data
  - `/var`: Variable data files
- Adhering to these standards helps maintain a consistent environment across different Linux systems, making it easier for users and administrators to navigate and manage files.
- In addition to FHS, Linux also supports various filesystem types, each with its own features and use cases. Common Linux filesystems include:
  - ext4: The default filesystem for many Linux distributions, known for its robustness and performance.
  - XFS: A high-performance filesystem suitable for large files and high-capacity storage systems.
  - Btrfs: A modern filesystem that offers advanced features like snapshots, checksums, and built-in RAID support.
  - Swap: A special filesystem used for virtual memory management.
- Use `man hier` to read more about the Filesystem Hierarchy Standard.
