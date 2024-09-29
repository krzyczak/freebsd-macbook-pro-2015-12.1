# freebsd-macbook-pro-2015-12.1
MacBookPro12,1 FreeBSD config

# Enable ASMC
For the ASMC to work the kernel needs to be recompiled with the patch.
```bash
cd /usr/src
pathc -p0 < asmc.patch

make buildkernel KERNCONF=GENERIC
make installkernel KERNCONF=GENERIC
```
