### Operating System

## Purpose

The operating system is the foundation of the security stack. Every other security control depends on the OS enforcing permissions, isolation, updates, and resource access.

## Requirements

An operating system should:

- Receive frequent security updates
- Support full-disk encryption
- Provide strong process isolation
- Have a transparent security model
- Minimize telemetry
- Allow user control
- Have a large security-conscious community

## Recommendations

### Linux
(nerd: hm, actually linux is not an operating system, its a kernel.)
(me: i know bro)

#### Arch Linux

Pros:
- Minimal by default
- User-controlled
- Fast security updates
- Extensive documentation

Cons:
- Requires maintenance
- User mistakes can reduce security

#### Fedora

Pros:
- Strong security defaults
- SELinux enabled by default
- Frequent updates

Cons:
- Less minimal than Arch

## Not Recommended

### End-of-Life Systems

Operating systems that no longer receive security updates should not be used.

Examples:
- Windows 7
- Ubuntu releases past support
- Unmaintained Linux distributions

## Hardening Principles

### Full-Disk Encryption

Enable encryption during installation whenever possible.

Benefits:
- Protects data at rest
- Mitigates device theft

### Principle of Least Privilege

- Use non-root accounts
- Avoid unnecessary sudo usage
- Limit installed software

### Software Sources

Prefer:
- Official repositories
- Verified maintainers

Avoid:
- Random installation scripts
- Untrusted repositories

### Updates

Install security updates promptly.

Security patches are most effective when applied quickly.

### Service Minimization

Disable services that are not needed.

Examples:
- Unused SSH servers
- Remote desktop services
- Legacy protocols

## My Baseline

Current Recommendation:
- Fedora for most users
- Arch Linux for advanced users

Required Controls:
- Full-disk encryption
- Automatic security updates
- Firewall enabled
- Strong account password
- Password manager
- Multi-factor authentication
