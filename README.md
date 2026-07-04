#Hardened Gentoo for i7-7700

Environment: Gentoo Linux (CLI Only)

A comprehensive, scratch-built Gentoo Linux environment optimized specifically
for the Intel Core i7-7700 architecture, featuring strict security hardening and manual system configuration.

## 1. Core System Architecture (Chroot)_
Deployed using a Gentoo Stage 3 tarball, focusing on manual configuration of core components:

*Compiler Optimizations: Configured make.conf with specific CFLAGS tailored for the Intel i7-7700 (Kaby Lake/Skylake) for
optimal performance.

*Kernel Compilation: Manually configured and compiled the Linux kernel (gentoo-sources) selecting only the necessary modules
and drivers for the hardware.

*Systen Initilization: Set up OpenRC as the init system.

## 2. Security Hardening Configurations
Implemented core security principles to protect the environment against unauthorized access and network-based attacks.

### Stateful Firewall (UFW)
Configured a strict access control policy:
*Default policy: deny incoming, allow outgoing
*Explicitly allowed port 22 (SSH) for secure access.

### SSH Daemon Harening
Secured /etc/ssh/sshd_config against brute-force attacks:
*Disabled Root Login: PermitRootLogin no
*Disabled Passwords: PasswordAuthentication no
*Enforced Key-Based Auth: Required Ed25519 keys.

## 3. Skills Demonstrated
*Advanced Linux System Administration
*Source-based package management (Portage)
*Custom Kernel configuration
*Network filtering and remote access security.
*AI-Assisted Administration: Leveraged AI (Google Gemini Flash/Pro) for troubleshooting, configuration guidance, and system optimization.
