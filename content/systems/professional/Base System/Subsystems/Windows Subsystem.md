#subsystems
## Overview
The Windows Subsystem allows execution of Windows applications. This System must be installed separately and runs apps in a container. The container will also create a virtual file system to support NTFS.

## OS requirements
The Windows Subsystem runs on any PaneOS version and only requires an x86 processor.
Windows apps need to be compiled to target Windows 10 21H2 or higher.
## Performance issues
When running PaneOS on any CPU since the Saphire Lineup, performance of apps compiled for x86-64 or amd64 run up to 60% slower due to the newer architecture used by these CPUs. To mitigate problems like this, cross-compile the app for x86-v3 or pane64-latest using the Developer Studio C++ or Rust compiler. 