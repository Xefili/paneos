## Overview
Orchestrator is a suite of low level management tools to handle most operating system api calls and hardware management.

## Structure
Orchestrator's structure is comprised of many modules, so called [[Directors]]. They allow the loading of individual modules to speed up execution time and reduce memory footprints.

## Failsafe
Orchestrator is _always_ available and will still work when the system is low on ressources. Should a child process freeze, the program will kill and rerun the process. Orchestrator can be launched in a console window with SuperKey + CTRL + ALT + SHIFT + O.


## Technical information
Orchestrator is built into PaneOS since version 6 and kernel version 5. The utility therefore requires API version LEGACY 25 or 5.