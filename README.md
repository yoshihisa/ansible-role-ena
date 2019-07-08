# Ansible Role - yoshihisa:ixgbevf

This Ansible role provides a ENA driver for SR-IOV using DKMS.

# Usage

In this example we configutation AWS EC2 and version 2.0.3.

```
---
- hosts: m5.large
  roles:
    - {role: yoshihisa:ena, ena_version: 2.0.3}
```

You put archive file in `files`.The archive file name should be `ena_linux_2.0.3.tar.gz`.   
You can find from [Github Release](https://github.com/amzn/amzn-drivers).  
If can not find in `files`, download from Github at runtime.

# Supprt Platforms

EL6 and 7.

# License

MIT License
