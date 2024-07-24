## Overview
Memory Control is a [[Directors|Director]] running under [[Orchestrator]]. It is used to handle memory operations like garbage collection and memory allocation. 
It also works in conjunction with the [[Crash Handler]] to create memory dumps.

## Usage
In normal circumstances, you will not need to use this utility. Should you still need to handle memory operations manually, use it with the following syntax:
`orchestrator direct memcntrl -[option] <argument> --[option]-[argument]`
Option can be a memory operation like shift, rearrange or free up. Arguments are almost always pointers to specific blocks or lists of blocks. 

### Block size
Memory block size is dependant on the amount of physical and virtual memory installed on the system. A block may range from 4KB to 16MB.

## Restriction & Memory Safety
This tool can be used to read any memory and modify almost all parts of the memory during the operation of the system. Therefore, this tool can reveal sensitive information and may only be accessed by the administrator user and cannot be invoked with an elevated application.