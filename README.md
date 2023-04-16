# prime-asus-z490m-plus-opencore-efi
OpenCore EFI Files for Prime ASUS Z490M Plus
#  Hackintosh
This repository contains OpenCore EFI Files for Prime ASUS Z490M Plus motherboard.

I will be updating the repo as i upgrade to latest versions of macOS. Consider whatever on the `main` branch is basically I'm using currently. You can find version tags as well.

I hope this repository will help others who are looking to build a Hackintosh which are using the same hardware & software configuration.

If you want to build one for you, I highly recomend going through the [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) itself. You will have to go through the instruction multiple times. I spent a lot of time figuring out the errors I made at various points. I will share those to help others so they don't make the same and hopefully saves a lot of time and frustration.

# ⚙️ Configuration
Im only adding details relevant to the setup here. You can reach out to me if you want to know more about my setup.

## Hardware
| # | Component | Details |
| - | - | - |
| 1 | Motherboard | Asus Prime Z490M-Plus LGA 1200 |
| 2 | CPU | Intel i7 10th Generation (10700) |
| 3 | Storage (OS) | Adata XPG SX8200 Pro 256GB NVME SSD |
| 4 | Storage (Backup) | Seagate Barracuda 2 TB Internal HDD |
| 5 | Monitor | LG 29" Ultrawide - 29UM69 |
| 6 | Network | Ethernet, Android USB Tethering |

## Software
| # | Name | Details |
| - | - | - |
| 1 | OS Version | macOS Ventura 13.3.1 (22E261) |
| 1 | SMBIOS | iMac 20,1 |

## BIOS Settings
| # | Name | Value |
| - | - | - |
| 1 | Fastboot | `Disable` |

## Drivers
| # | Name | Details |
| - | - | - |
| 1 | AudioDxe.efi | Audio |
| 2 | HfsPlus.efi | HFS Volumes (macOS Installers & Recovery) |
| 3 | OpenCanopy.efi | GUI for boot menu |
| 4 | OpenRuntime.efi | - |
| 5 | ResetNvramEntry.efi | - |

## Kexts
| # | Name | Details |
| - | - | - |
| 1 | WhateverGreen.kext | Graphics |
| 2 | AppleALC.kext | Audio |
| 3 | IntelMausi.kext | Ethernet |
| 4 | HoRNDIS.kext | Android USB Tethering |
| 5 | USBMap.kext | Mapped all 8 USB ports |
| 6 | XHCI-unsupported.kext | - |
| 7 | Lilu.kext | - |
| 8 | NVMeFix.kext | - |
| 9 | RTCMemoryFixup.kext | - |
| 10 | SMCProcessor.kext | - |
| 11 | SMCSuperIO.kext | - |
| 12 | VirtualSMC.kext | - |

## SDDTs
| # | Name | Details |
| - | - | - |
| 1 | SSDT-AWAC.aml | - |
| 2 | SSDT-EC-USBX-DESKTOP.aml | - |
| 3 | SSDT-PLUG-DRTNIA.aml | - |
| 4 | SSDT-RHUB.aml | - |

## Whats not Working?
These are the hardware i already had before I install macOS. Since i have other methods, i never botherd about buying a new one.
| # | Name | Hardware | Details |
| - | - | - | - |
| 1 | Wi-Fi | TP-Link AC1200 Wireless WiFi PCIe Card | Not supported in Ventura because it uses a Realtek RTL8812AE chipset. |
| 2 | Bluetooth | TP-Link USB Bluetooth Adapter UB500 | Not supported in Ventura because it uses a Realtek RTL8761B chipset. |
