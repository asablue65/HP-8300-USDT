# HP-8300-USDT
# HP8300USDT-Hackintosh-EFI
Opencore EFIs for HP8300USDT

# Computer Used

* HP Elite 8300 Ultra Slim Desktop
* CPU: i7-3770S 3.1GHz
* Motherboard: Q77
* BIOS: [00.03.08 Rev.A]
* GPU: HD 4000/AMD FirePro W5170M 2G
* RAM: Samsung 8G * 2
* NVMe: Micron SATA SSD 256GB
* Wifi/Bluetooth: BCM94360HMB

# Status
![System Info](https://github.com/asablue65/HP-8300-USDT/blob/main/doc/About_This_mac.png)
* Opencore：0.8.5 offcial
* MacOS: Monterey 12.6.5
* Sleep: YES
* GPU: 
	AMD FirePro W5170M (Radeon R9 M375X)
    		* DisplayPort: YES
    		* VGAPort (Bottom): NO
	HD 4000
    		* DisplayPort (Top): NO
* Wifi/Bluetooth: YES
* Handoff: YES
* HD Audio: YES
* Computer Speaker: YES
* USB: All YES
* mSATA: YES
* SD Reader: YES
* DVDROM: YES

# Other Settings
1. Secured Mode: Disabled
2. BIOS: The Latest
3. CFG_Lock: Disabled
4. UEFI Only

## EFI layout
1. Download EFI, Opencore and all kexts needed
2. Change config.plist with your own SMBios choice（iMacPro1,1)
3. Must have boot-args: radpg=15 -lilubetaall
3. Reboot

