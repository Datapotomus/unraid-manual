---
description: >-
  When changing the balance of the disk these are the configurations you can
  use.
---

# BTRFS raid configuration for unRAID

Single: requires 1 device only, it's also the only way of using all space from different size devices, BTRFS equivalent of JBOD, no performance gains vs single disk or RAID1 

`-dconvert=single -mconvert=raid1`

RAID0: requires 2 device, best performance, no redundancy, if used with different size devices only 2 x capacity of smallest device will be available, even if reported space is larger. `-dconvert=raid0 -mconvert=raid1`

RAID10: requires at least 4 devices, to use full capacity of a 4 device pool they all need to be the same size. 

`-dconvert=raid10 -mconvert=raid10`

_RAID5/6 are still considered experimental so use at your own risk_

RAID5: requires at least 3 devices.

`-dconvert=raid5 -mconvert=raid1`

RAID6: requires at least 4 devices. 

`-dconvert=raid6 -mconvert=raid1`

