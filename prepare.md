```bash
sudo zpool create -o ashift=12 tank raidz2 ata-WDC_WD10EFRX-68FYTN0_WD-WCC4J0SEF254 ata-WDC_WD10EFRX-68FYTN0_WD-WCC4J7VF4NUS ata-WDC_WD10EFRX-68FYTN0_WD-WCC4J0TDU34X ata-WDC_WD10EFRX-68FYTN0_WD-WCC4J0SEFN9A ata-WDC_WD10EFRX-68FYTN0_WD-WCC4J0TDUPT3

sudo zpool set autoexpand=on tank
sudo zfs set atime=off tank
sudo zfs set compression=lz4 tank
```