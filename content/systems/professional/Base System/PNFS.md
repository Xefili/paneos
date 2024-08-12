## Overview
PNFS, short for Pane File System is a file system, designed for PaneOS. It is very similar to the ext4 system. The system is classified as a journaling file system and is very robust to crashes and corruption. It also allows for effortless hot swapping on supported devices.

## RAID & more
PNFS supports multiple RAID configurations, such as Mirror, Parity and Striped Volumes. To configure PaneOS to use a certain RAID configuration, use [[pnUtils]] to create two or more partitions and [[pndeploy]] to install PaneOS with the `-R <mirror|parity|striped> auto` flag.
The command for this is:
```bash
pndeploy -I paneosx86-v3.iso -D 0 -R <mirror|parity|striped> --edition-professional
```
