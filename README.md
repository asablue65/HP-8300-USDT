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
* STORAGE: Micron SATA SSD 256GB
* Wifi/Bluetooth: BCM94360HMB

# Status
![System Info](https://github.com/asablue65/HP-8300-USDT/blob/main/doc/About_This_mac.png)
* Opencore：0.8.5 offcial
* MacOS: Monterey 12.6.5
* Sleep & Wake: YES
* GPU: AMD FirePro W5170M (Radeon R9 M375X), DisplayPort (Bottom): YES, VGAPort: NO
* GPU: intel HD 4000, DisplayPort (Top): NO
* Wifi/Bluetooth: YES
* Handoff: YES
* HD Audio: YES
* Computer Speaker: YES
* Audio in for MIC: NO
* USB: All YES
* mSATA: YES
* SD Reader: YES
* DVDROM: YES

# Other Settings
1. SecureBoot Mode: Disabled
2. BIOS: The Latest
3. CFG_Lock: Disabled
4. UEFI Only

## EFI layout
1. Download EFI, Opencore and all kexts needed
2. Change config.plist with your own SMBios choice（iMacPro1,1)
3. Must have boot-args: radpg=15 -lilubetaall
3. Reboot

Extra 1: For OS Ventura Installation (Opencore 0.9.0)
1. Add "amfi_get_out_of_my_way=0x1" or "amfi=0x80" to boot-args,
 or Replace "amfi=0x80" with "-amfipassbeta" and add AMFIPass.kext to Kexts
2. Download Opencore Legacy Patcher and apply Post-Install Root Patch

Extra 2: For OS Sonoma Installation
1. Updating kexts and bootloader to the latest versions (Opencore 0.9.6)
2. Edit the config.plist and set SecureBootModel to "Disabled" (in Misc/Security section)
3. In Kernel section, block com.apple.iokit.IOSkywalkFamily (and set MinKernel to 23.0.0)
4. Add the kexts and a dependency in the OC's appropriate folder and declare them in the config.plist (and set MinKernel to 23.0.0)
	IOSkywalkFamily.kext
	IO80211FamilyLegacy.kext
	IO80211FamilyLegacy.kext/Contents/PlugIns/AirPortBrcmNIC.kext
5. Use a soft unlock for SIP: set csr-active-config to "03080000" in NVRAM
6. Add "amfi=0x80" to boot-args
 or Replace "amfi=0x80" with "-amfipassbeta" and add AMFIPass.kext to Kexts,
7. Download Opencore Legacy Patcher and apply Post-Install Root Patch

* After OCLP is installed is possible to set SecureBootModel as you like and enable SIP (set csr-active-config to "00080000")

![System Info](https://github.com/asablue65/HP-8300-USDT/blob/main/doc/Ventura.png)
![System Info](https://github.com/asablue65/HP-8300-USDT/blob/main/doc/Sonoma.png)

