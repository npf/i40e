This repository provides Linux DKMS packages for Intel i40e OOT driver, for use with Debian Jessie. Debian Jessie indeed ships with a old i40e driver which does not support recent NICs.

The i40e-XXX/src directory contains the dkms.conf file to add to the sources of the OOT driver version XXX from Intel, so that dkms deb package can be built.

i40e version XXX OOT driver sources can be downloaded from https://downloadcenter.intel.com/product/36773/Ethernet-Products → Intel® Ethernet Adapter Complete Driver Pack.

The deb directory contains ready to consum deb packages.

The following line can be added to a Debian `sources.list` file, in order to provide the deb packages stored in this repository:

```
deb [trusted=yes] https://github.com/npf/i40e/raw/master/deb /
```

