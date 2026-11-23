# Lenovo M920X Tiny
# Tiny5-Hackintosh-EFI
Opencore EFI for M920X Tiny

# Computer Used

* Lenovo M920X Tiny Desktop
* CPU: i7-9700T 4.3GHz
* Motherboard: Q370
* BIOS: [1.0.0.121]
* GPU: AMD RX560 4GB
* RAM: Samsung 8G * 2
* STORAGE: Segate SN580 NVME 512GB
* Wifi/Bluetooth: BCM94360NG

# Status
![System Info](https://github.com/asablue65/Lenovo-M920X-Tiny/blob/main/doc/Tahoe.png)
* Opencore：1.0.8 offcial
* MacOS: Tahoe 26.7.2
* Sleep & Wake: YES
* eGPU: AMD RX560 4GB
* iGPU: intel HD630
* Wifi/Bluetooth: YES
* Handoff: YES
* HD Audio: YES
* Computer Speaker: YES
* Audio in for MIC: NO
* USB: All YES

# Other Settings
1. SecureBoot Mode: Disabled
2. BIOS: The Latest
3. CFG_Lock: Disabled
4. UEFI Only

## EFI layout
1. Download EFI, Opencore and all kexts needed
2. Change config.plist with your own SMBios choice（iMa20,1)
3. Must have boot-args: -amfipass, csr-active-config to "03080000"
4. Reboot

* No OCLP root patch required