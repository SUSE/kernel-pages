---
title: SLE15-SP7-COCO branch
redirect_from: /branches/SLE15-SP7-COCO/
---
# SLE15-SP7-COCO
This is the SLE15 SP7 COCO kernel branch. It is based on the SLE15 SP7
kernel branch and provides a tech preview of Confidential Computing
host support with KVM.

The person in charge of this branch is:
Juergen Gross <[jgross@suse.de](mailto:jgross@suse.de?subject=SLE15-SP7-COCO%20branch)>

It is the above persons' responsiblity for checking in this kernel to
the build system, anyone else who wishes to do so, needs to get
permission from them first.

If there are any questions about this branch, please contact the above
mentioned maintainer.


## [packages](https://download.opensuse.org/repositories/Kernel:/SLE15-SP7-COCO)
To install
[prebuilt kernel](https://download.opensuse.org/repositories/Kernel:/SLE15-SP7-COCO)
from this branch run

```
zypper ar -f https://download.opensuse.org/repositories/Kernel:/SLE15-SP7-COCO/pool \
    Kernel:SLE15-SP7-COCO
zypper in --from Kernel:SLE15-SP7-COCO kernel-default
```

Please note: The packages are built for the distribution they are
targetting. In case of the vanilla and linux-next branches, this is the
latest released openSUSE version. While the packages should work
fine on a distribution that is slightly newer or slightly older,
installing ancient kernels on the latest distributions is asking for
trouble. Same goes for the opposite case, e.g. installing the Factory
kernel on SLES 11.

## [kernel-source.git](https://github.com/SUSE/kernel-source/tree/SLE15-SP7-COCO)
There are two SUSE Kernel repositories. Development happens in the
[kernel-source](https://github.com/SUSE/kernel-source/tree/SLE15-SP7-COCO)
git repository. This tree is a quile-like series of patches against the
upstream kernel, plus spec files and various scripts. You can clone it
with

```
git clone https://github.com/SUSE/kernel-source -b SLE15-SP7-COCO
```

## [kernel.git](https://github.com/SUSE/kernel/tree/SLE15-SP7-COCO)
If you just want to hack on the sources and do not need to package the
kernel, use the [kernel](https://github.com/SUSE/kernel/tree/SLE15-SP7-COCO)
git repository. This one has the same layout as the upstream kernel. Clone
command:

```
git clone https://github.com/SUSE/kernel -b SLE15-SP7-COCO
```


