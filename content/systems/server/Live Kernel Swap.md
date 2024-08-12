## Overview
In PaneOS server, you are able to perform a (live) kernel swap. This allows for switching to a newer kernel without any downtime. PaneOS server will load both kernels into memory and starts redirecting kernel calls to the updated kernel. When no processes are accessing the old kernel, it hands over drivers and temporary data to the new kernel and gets cleared from memory.

## Limitations
Only kernel versions from the same series are eligible. For example, kernel 6.x to kernel 6.4.x can be switched live on server version 7.x - 7.4.x. For higher versions, only the 6.5 to 6.9.x can be used. When doing an offline switch default requirements are used.[^1] 

## In case of power loss:
Since PaneOS server always uses a dual system partition system, it will boot from the second partition after 3 failed attempts.

[^1]:More disclosed later.