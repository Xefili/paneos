## Overview
The Pixel Switch is a rack mounted server-like device, used for routing and accumulating data. This data may be sent to individual [[Pixel GPU]]s for processing. Each switch requires at least one input, usually a PCIe daughter card.

## Usage Example
Since [[Rack provided Power|RpP]] Cards like [[Pixel GPU#Datacenter Cards|Pixel Datacenter GPUs]] cannot receive data over their double PCIe-like slot, they receive it over a [[Pixel-Pixel Bridge]] or [[Pixel-Quixel-Bridge]]. When using a Pixel-Pixel Bridge, a cluster of many interconnected cards may be connected to one Pixel Switch.

SXM5 and PCIe cards do not require a Pixel Switch, except for linking multiple servers together. Servers like these are called [[Sharded Nodes]].