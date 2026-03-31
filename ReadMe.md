# Haiku OS - FDT Support Development Fork

This repository is a development fork of the official [Haiku Operating System](https://github.com/haiku/haiku). 

The primary focus of this fork is the implementation and enhancement of **Flattened Device Tree (FDT)** support within the Haiku kernel and bootloader. This work is essential for improving Haiku's hardware discovery capabilities on non-x86 architectures, specifically **ARM** and **RISC-V**.

---

## 🚀 Project Overview

In architectures like ARM and RISC-V, hardware is not "self-discoverable" (unlike PCI on x86). The operating system relies on an **FDT** (passed as a `.dtb` blob) to understand the memory map, CPU topology, and peripheral addresses.

### Key Objectives:
* **FDT Parsing:** Enhancing the existing FDT parsing logic in the Haiku bootloader.
* **Driver Mapping:** Streamlining how the Haiku driver model interacts with FDT nodes to initialize platform devices.
* **Libfdt Integration:** Ensuring robust integration with `libfdt` while adhering to Haiku's strict coding standards.
* **Architecture Parity:** Bringing ARM/RISC-V boot sequences closer to the stability found in the x86_64 port.

## 🛠 Current Status
