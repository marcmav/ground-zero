# *bedrock*

A playbook of the architectural root of my security model. It defines the foundational layers, principles and controls that every system must satisfy before it can be considered trusted.

## *The Defense-in-Depth Model*

Security is engineered sequentially from the system's lowest trust boundary outward to my digital identity. If a lower layer is compromised, the structural integrity of every layer above it is void.

```
[ Layer 5: Alias ] --- Identity
    [ Layer 4: Credentials ] --- Password Manager, TOTP
        [ Layer 3: Gateway ] --- Browser, Search Engine
            [ Layer 2: Network ] --- Router, Firewall, DNS
                [ Layer 1: Compute ] --- Operating System
                    [ Layer 0: Core ] --- Firmware/UEFI
```

### *Layer 0: Core*

Linux kernel
============

The Linux kernel is the core of any Linux operating system. It manages hardware,
system resources, and provides the fundamental services for all other software.

Quick Start
-----------

* Report a bug: See Documentation/admin-guide/reporting-issues.rst
* Get the latest kernel: https://kernel.org
* Build the kernel: See Documentation/admin-guide/quickly-build-trimmed-linux.rst
* Join the community: https://lore.kernel.org/

Essential Documentation
-----------------------

All users should be familiar with:

* Building requirements: Documentation/process/changes.rst
* Code of Conduct: Documentation/process/code-of-conduct.rst
* License: See COPYING

Documentation can be built with make htmldocs or viewed online at:
https://www.kernel.org/doc/html/latest/
