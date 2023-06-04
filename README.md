![Screenshot 2023-06-04 at 22 53 36](https://github.com/TuanCanCode/x99-qd4-hackintosh/assets/43199445/ad34cf58-23d3-457e-a26b-aadbe85ccd8c)


# Huananzhi X99-QD4 + Intel Xeon E5-2680 v4 + Sapphire Nitro+ RX 580 8GB
Latest working macOS: Ventura 13.4

OpenCore version: 0.9.2

## PC specifications
  - Mainboard: Huananzhi X99-QD4
  - CPU: Intel Xeon E5-2680v4 12-cores/ 24-threads
  - GPU: Sapphire Nitro+ RX 580 8GB (Native support)
  - SSD: Samsung NVME 970 Evo 256GB
  - HDD: Toshiba 1TB
  - Ram: Samsung ECC 32GB x 2 2400mhz
  - PSU: Corsair RM650 
  - Wifi + Bluetooth card: BCM94360CS2 (Native support)
  - Monitor: Cooler Master GM34-CW2 34inch 165hz
## Installations (Windows):
  - Download MacOS Image (12.0.1): https://drive.google.com/file/d/1KrvUYpbIXtJ3hR7tZpKWnGz5_kwFEtLD/view?usp=sharing and create bootable usb using balenaEtcher https://www.balena.io/etcher/
  - Mount EFI folder of boot drive by using Mini Partion Wizard https://www.partitionwizard.com/free-partition-manager.html. Select EFI folder from boot drive and then right click choose Change Volume Letter option and click Ok and Apply
  - Copy EFI folder from the repository to EFI folder in boot drive by using Explorer++ (Administator permission is required) https://explorerplusplus.com/download
  - Restart to BIOS and setup following this https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/broadwell-e.html#intel-bios-settings  ![Screen Shot 2565-04-01 at 12 21 04](https://user-images.githubusercontent.com/43199445/161199876-94898eb0-7311-47e4-afa6-a884343dee14.png)
  - Save change bios and boot to usb boot drive to start MacOS installation process

## Notes:
- The MacOS Image version is 12.0.1 after installing sucessfully, You can update to version Monterey 12.6.6 or Ventura 13.4 via OTA without any issue
- BIOS config for Above 4G decoding can make your PC not booting when enable it. If you got this issue, then reset your bios by remove your CMOS Battery or using the Clear BIOS jumper. And then re-config your bios setting and skip this setting option.
- Drive for install Hackintosh should be formatted with APFS format

## What works
- macOS Monterey
- Audio
- HDMI/DP
- All USB ports
- Ethernet
- Bluetooth Usb Dongle
- Monitor with high refresh rate 165hz

# References
Please read carefully if you wanna try it by yourself:
- Sanity check config.plist file: https://sanitychecker.ocutils.me/
- Collect file: https://dortania.github.io/OpenCore-Install-Guide/ktext.html#firmware-drivers
- Setup config.plist file: https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/haswell-e.html#starting-point
- Bios: [https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/haswell-e.html#intel-bios-settings](https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/broadwell-e.html#intel-bios-settings)
- Fix bluetooth usb dongle: https://dortania.github.io/OpenCore-Install-Guide/extras/monterey.html#bluetooth [
](https://sanitychecker.ocutils.me/)
