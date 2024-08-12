## Overview
The Crash Handler is responsible for handling critical system exceptions and errors.

## How it works
1. Lock all CPU cores except one. If only one is present, the system must be reset manually.
2. Dump registers and cache (L1-L4) and clear stack for this core.
3. Dump memory and page file to minimize data loss.
4. (_try to_) Show crash screen.
5. Reset entire CPU and force restart.

On boot, the system will perform a full self check and will try to repair any critical system files which may have caused the error. Should a driver be the cause of the exception, the system will boot into safe mode.

During the boot stage, the system might also apply a shadow copy or use a system restore point. This can skipped by holding down ESC during the `Preparing for disk repair.` screen.

After 3 consecutive crashes, the system will boot into recovery mode and provides an elevated terminal with the SYSTEM user signed in. In an emergency, the [[Pane Foundation user]] may also be accessed.

## Data (Loss)
During a crash, as much data is tried to be saved to disk and PaneOS will try to reopen programs which had unsaved data to properly save it. This doesn't always work and is quite unreliable due the nature of the crash. You can recover some data from the cache and memory dump, although this data will be in either binary (cache & register) of hexadecimal (memory & page file).