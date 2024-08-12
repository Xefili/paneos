## Overview
Orchestrator is a suite of low level management tools to handle most operating system api calls and hardware management.

## Structure
Orchestrator's structure is comprised of many modules, so called [[Directors]]. They allow the loading of individual modules to speed up execution time and reduce memory footprints.

## Failsafe
Orchestrator is _always_ available and will still work when the system is low on resources. Should a child process freeze, the program will kill and rerun the process. Orchestrator can be launched in a console window with SuperKey + CTRL + ALT + SHIFT + O.


## Technical information
Orchestrator is built into PaneOS since version 6 and kernel version 5 but works on PaneOS Legacy Version 18 or higher. The utility therefore requires API version LEGACY 25 or 5. In case of low memory, Orchestrator may execute fully in cache[^1] or move programs to the page file. If the page file is disabled, Orchestrators [[Memory Control]] director may create one temporarily.

[^1]:Requires the EXEC_FLLY_IN_CCH instruction, available on Emerald [[Gemstone CPUs]] or higher.