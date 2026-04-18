# 🛠️ Lab Setup: The Nested Hypervisor
This lab uses a "Nested Virtualization" stack to simulate an enterprise data center environment.

## Repository Information
- **Official Project Name:** LPI-Linux-Essentials-Study-Plan
- **Primary Host:** Fedora Linux


## The Hardware/Software Stack
1. **Physical Host:** Fedora Linux
2. **Layer 1 (L1) Hypervisor:** KVM/QEMU via `virt-manager`.
3. **Layer 2 (L2) Hypervisor:** Proxmox VE 8.x (Nested).
4. **Guest VMs:** - Debian 12
   - Rocky Linux 9

## Technical Configuration
- **CPU Passthrough:** The Proxmox VM is set to `Host` CPU type in `virt-manager` to enable Nested VT-x/AMD-V.
- **Verification:** `cat /sys/module/kvm_intel/parameters/nested` returns `Y`.
- **Networking:** Virtual Bridge (`vmbr0`) handles traffic between the Debian/Rocky guests and the Fedora host.
