# Lab 0 – Inventory your own machine

## Inventory Table

| What | Value | Where I got it (Command) |
| :--- | :--- | :--- |
| **CPU Model** | Apple Silicon | `sysctl -n machdep.cpu.brand_string` |
| **CPU Cores / Threads** | 10 cores, 10 threads | `sysctl -n hw.physicalcpu hw.logicalcpu` |
| **Total Memory** | 32 GB | `system_profiler SPHardwareDataType` |
| **Memory Modules & Speed** | Integrated LPDDR5 | `system_profiler SPMemoryDataType` |
| **Disk Model & Type** | Apple SSD (NVMe) | `system_profiler SPStorageDataType` |
| **Free Space for VMs** | ~783GB | `df -h /` |
| **Firmware Type** | UEFI (iBoot / Apple) | `uname -v` |
| **Hardware Virtualization** | Present and Enabled (1) | `sysctl -n kern.hv_support` |

## What did not work
Everything went smoothly using the command line tools. No graphical windows were used.
