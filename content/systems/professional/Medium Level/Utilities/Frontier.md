## Overview
Frontier is a complex tool to encrypt and decrypt files and disks, as well as handle memory and data integrity.

## Disk Encryption
Frontier uses two cryptographic methods to encrypt and decrypt files on a disk. The main encryption method is the symmetrical PN4096 algorithm, the second method used for storing the key is standard RSA cryptography.

## Memory & Data Integrity
After a crash, PaneOS will check data integrity against snapshots made by [[PNFS]]. Memory integrity is largely handled by the [[Memory Control]] director, but under certain cases, Frontier may be responsible for memory checks.