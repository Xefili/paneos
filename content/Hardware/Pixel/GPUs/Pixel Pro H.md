## Overview
Pixel Pro H GPUs are datacenter like GPUs with a lot of general purpose and media processing power. They also feature x86_64 emulation and can simulate complex physics scenes in real time.

## Technical Overview
### Cores
- Tensor: up to 614 1st Generation AI tensor cores.
- UCA: up to 24577 2nd Generation [[UCA]] cores.
- DLFX: 1st Generation [[DLFX]] cores.
- RT: up to 182 2nd Generation [[RT]] cores.
- x86_64-v3: 8/12 Quixel 7 1900HX/AI
- Shader: 17223 2nd Generation [[Shader]] cores
#### Storage & Connectivity
Cache:
- L1: 512KB
- L2: 4096KB
- L3: 12MB
- L4: 32MB
RAM/VRAM:
- up to 128GB @ 256GB/s
- can be extended with [[Pixel-Pixel Bridge]] to connect 256 cards together (32TB @ 512GB/s[^1])
Connectivity:
- 1x HDMI, 1x DP, 1x USB-C
- 1st Generation [[Pixel-Pixel Bridge]]
- PCIe Gen5, SXM5 or [[Rack provided Power|RpP]]

[^1]: 512GB/s total speed, bidirectional speed is 256GB/s in both directions