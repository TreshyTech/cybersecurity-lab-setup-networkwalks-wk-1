# 🔐 Network Walks — Week 1
## Cybersecurity Lab Setup and Environment Configuration

> Building the foundation for hands-on cybersecurity practice through virtualization, network configuration, and systematic documentation.

---

## 🎯 1. Objectives

The objectives of this practical exercise were to:

- Set up a virtual lab environment using Oracle VirtualBox.
- Prepare Kali Linux as a virtual machine for authorized cybersecurity testing.
- Configure a dedicated virtual network for communication between lab systems.
- Explore shared-folder, clipboard, and drag-and-drop integration.
- Document the configuration process and verify the lab's readiness for further practical exercises.

## 🧪 2. Purpose of the Lab

The purpose of this lab was to establish a controlled and isolated environment where cybersecurity concepts can be explored safely.

Virtualization allows different operating systems to run as virtual machines on one physical computer. This makes it possible to practice system administration, networking, security monitoring, and authorized security testing without needing separate physical computers for every task.

## 🏗️ 3. Lab Architecture

The lab uses a host computer running Oracle VirtualBox, with Kali Linux operating as a guest virtual machine.

**Architecture overview:**

```text
              HOST COMPUTER
                   |
             Oracle VirtualBox
                   |
          NetworkWalks-Kali VM
                   |
          NetworkWalks-NAT
          10.0.0.0/24 network
                   |
           Kali Linux interface
           Planned IP: 10.0.0.2
```

**Architecture notes:**
- Host machine: Windows computer
- Virtualization platform: Oracle VirtualBox
- Guest operating system: Kali Linux
- Virtual network: `NetworkWalks-NAT`
- Planned Kali IP address: `10.0.0.2/24`

*Note: The IP address and connectivity should be confirmed against the actual VM configuration before this diagram is treated as verified.*

## ⚙️ 4. Lab Configuration

| Component | Configuration |
|---|---|
| Virtualization platform | Oracle VirtualBox |
| Virtual machine | NetworkWalks-Kali |
| Guest operating system | Kali Linux |
| Network type | NAT Network |
| Network name | NetworkWalks-NAT |
| IPv4 subnet | `10.0.0.0/24` |
| Planned Kali IPv4 address | `10.0.0.2/24` |
| Shared folder | Host Downloads folder |
| Clipboard and drag-and-drop | Bidirectional, where supported |

Configuration values should be checked against the final settings in VirtualBox and Kali Linux.

## 🛠️ 5. Setup Procedure

The lab setup involved the following stages:

1. **Prepare the virtualization platform:** Install or open Oracle VirtualBox.
2. **Create the virtual machine:** Set up a dedicated Kali Linux VM for the training environment.
3. **Configure system resources:** Allocate suitable memory, processors, and virtual disk space according to the lab requirements.
4. **Configure virtual networking:** Create the `NetworkWalks-NAT` network using the specified IPv4 subnet.
5. **Connect the VM:** Attach the Kali virtual network adapter to the configured NAT Network.
6. **Configure file sharing:** Add the host Downloads folder as a VirtualBox shared folder.
7. **Enable integration features:** Configure shared clipboard and drag-and-drop where supported.
8. **Review the configuration:** Check the VM settings before proceeding to network verification.

## ✅ 6. Lab Verification

The lab should be verified before being used for further exercises.

| Verification item | How to check | Status |
|---|---|---|
| Kali VM starts successfully | Start the VM and log in |Confirmed |
| IP address is correct | Run `ip -br address` in Kali | Confirmed |
| Default route is configured | Run `ip route` | Confirmed |
| Network connectivity works | Test the configured gateway and internet access |Confirmed |
| Shared folder is accessible | Check the mounted shared folder in Kali | Confirmed |
| Clipboard integration works | Test copying text between host and guest | Confirmed |



## 💡 7. Lessons Learned

This exercise reinforced several important concepts:

- **Virtualization:** A virtual machine provides a separate computing environment for practical learning.
- **Networking:** IP addresses, subnets, gateways, and network modes determine how systems communicate.
- **Lab isolation:** A dedicated virtual network helps organize lab systems and control their connectivity.
- **Configuration management:** Small configuration errors can prevent a virtual machine from communicating as expected.
- **Documentation:** Clear screenshots and written notes make technical work easier to reproduce and troubleshoot.

## 🔗 8. Tools and Resources

- [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads) — Virtualization platform
- [Kali Linux](https://www.kali.org/get-kali/) — Security-focused Linux distribution
- [Kali Linux Documentation](https://www.kali.org/docs/) — Installation and configuration guidance
- [GitHub Docs](https://docs.github.com/) — Repository and README documentation

## 👩🏽‍💻 9. Author

**Name:** Treasure Ikpangeto  
**Program:** Network Walks Cybersecurity Training  
**Focus:** Cybersecurity fundamentals, networking, Linux, and practical lab development


## 📌 Project Information

- **Program:** Network Walks
- **Week:** 01
- **Project:** Cybersecurity Lab Setup
- **Platform:** GitHub
- **Environment:** Oracle VirtualBox and Kali Linux
- **Repository purpose:** Record lab configuration, screenshots, verification results, and lessons learned.

---




