# 🛠️ Lab Setup: The Nested Hypervisor
This lab uses a "Nested Virtualization" stack to simulate a real enterprise environment.

## The Stack
1. **Physical Host:** Fedora Linux
2. **Type 2 Hypervisor:** Virtual Machine Manager (virt-manager) / KVM
3. **Type 1 Hypervisor (Nested):** Proxmox VE 8.x
4. **Study Nodes (LXC/VM):** - Debian 12 (Target for APT testing)
   - Rocky Linux 9 (Target for DNF testing)

## Configuration Notes
- **Nested VT-x:** Enabled on the Fedora host to allow Proxmox to run KVM.
- **Network:** Bridged networking via `vmbr0` in Proxmox.
- **CPU Type:** Set to 'Host' for maximum performance in the inner VMs.
