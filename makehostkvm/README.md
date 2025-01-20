This will configure a Debian 12 host to act as a KVM hypervisor.  It will find the NIC with the Default Route and make a "br0" bridge.

Add your user to user account to libvirt group

```bash
adduser <youruser> libvirt
```

Reboot and cleanup networking config if necessary.  This playbook takes a guess at the right thing but it may be not a perfect fit in all cases.  It does not setup IPv6.
