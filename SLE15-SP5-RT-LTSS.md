---
title: SLE15-SP5-RT-LTSS branch
redirect_from: /branches/SLE15-SP5-RT-LTSS/
---
# SLE15-SP5-RT-LTSS
The persons in charge of this branch are:
Mel Gorman <[mgorman@suse.de](mailto:mgorman@suse.de?subject=SLE15-SP5-RT-LTSS%20branch)>
Frederic Weisbecker <[fweisbecker@suse.de](mailto:fweisbecker@suse.de?subject=SLE15-SP5-RT-LTSS%20branch)>
Petr Tesarik <[ptesarik@suse.com](mailto:ptesarik@suse.com?subject=SLE15-SP5-RT-LTSS%20branch)>
Jeffrey Cheung <[jcheung@suse.com](mailto:jcheung@suse.com?subject=SLE15-SP5-RT-LTSS%20branch)>

It is the above persons' responsiblity for checking in this kernel to
the build system, anyone else who wishes to do so, needs to get
permission from them first.

If there are any questions about this branch, please contact the above
mentioned maintainer.


## [packages](https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-RT-LTSS)
To install
[prebuilt kernel](https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-RT-LTSS)
from this branch run

```
zypper ar -f https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-RT-LTSS/pool \
    Kernel:SLE15-SP5-RT-LTSS
zypper in --from Kernel:SLE15-SP5-RT-LTSS kernel-default
```

Please note: The packages are built for the distribution they are
targetting. In case of the vanilla and linux-next branches, this is the
latest released openSUSE version. While the packages should work
fine on a distribution that is slightly newer or slightly older,
installing ancient kernels on the latest distributions is asking for
trouble. Same goes for the opposite case, e.g. installing the Factory
kernel on SLES 11.

## [kernel-source.git](https://github.com/SUSE/kernel-source/tree/SLE15-SP5-RT-LTSS)
There are two SUSE Kernel repositories. Development happens in the
[kernel-source](https://github.com/SUSE/kernel-source/tree/SLE15-SP5-RT-LTSS)
git repository. This tree is a quile-like series of patches against the
upstream kernel, plus spec files and various scripts. You can clone it
with

```
git clone https://github.com/SUSE/kernel-source -b SLE15-SP5-RT-LTSS
```

## [kernel.git](https://github.com/SUSE/kernel/tree/SLE15-SP5-RT-LTSS)
If you just want to hack on the sources and do not need to package the
kernel, use the [kernel](https://github.com/SUSE/kernel/tree/SLE15-SP5-RT-LTSS)
git repository. This one has the same layout as the upstream kernel. Clone
command:

```
git clone https://github.com/SUSE/kernel -b SLE15-SP5-RT-LTSS
```


