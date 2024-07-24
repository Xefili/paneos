## Overview
The PaneOS kernel is a monolithic but also modular kernel. When required, the kernel can switch to [[Kernel#High Performance Mode]] and can return to modular mode during runtime.

## Memory Handling
Since memory leaks can cause system instability, the kernel handles memory through virtualizing or through paging. It keeps track of every process's memory footprint can also does garbage collection. This is all handled by the [[Memory Control]] director of [[Orchestrator]].

## Hardware I/O
Hardware I/O is also an important function of the kernel, but is rather handled by drivers or the [[Hardware Management]] director of [[Orchestrator]].

## High Performance Mode
The kernel usually runs in modular mode to save memory. This however decreases overall speed. To address this issue, the kernel is able to switch to High Performance Mode at runtime. In this mode, the kernel loads all modules (Orchestrator critical - Drivers) and leaves module mode.
In this state, the kernel may use more RAM than usual, but may free up CPU bandwidth.