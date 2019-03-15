---
description: >-
  Page walks through how to encrypt an existing array in unRAID if it isn't
  already encrypted.
---

# Encrypt an Existing Array

## Prereqs / Info

As of this writing you can't currently encrypt data on the existing file-systems. You essentially need to move your data off the disk you want to encrypt then encrypt it after the data is moved off.

* [ ] Must be on version 6.4+ current version can be found [here](https://unraid.net/download).
* [ ] The unbalance plugin, info [here](https://forums.unraid.net/topic/43651-plug-in-unbalance/).
* [ ] The fix common problems plugin, info [here](https://forums.unraid.net/topic/47266-plugin-ca-fix-common-problems/).
* [ ] The Unassigned Devices plugin, info here.
* [ ] You need to have enough free space on your storage array to cover moving the data off any of your drives.

## High Level Process

1. Use unblance plugin to move the data off of the hard drive you want to encrypt.
2. Format the hard drive that is empty with an encrypted file system.
3. Repeat those steps until all hard drives have been encrypted.

