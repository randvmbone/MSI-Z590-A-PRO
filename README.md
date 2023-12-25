# MSI Z590-A PRO

OpenCore EFI for MSI Z590-A PRO

![about](https://raw.githubusercontent.com/randvmbone/MSI-Z590-A-PRO/main/about.png)

### Hardware

* **MOBO:** MSI Z590-A PRO
* **CPU:** Intel Core i7-10700K
* **RAM:** G.SKILL Aegis DDR4-2666 32GB (2x16GB)
* **GPU:** SAPPHIRE NITRO+ Radeon RX Vega 64
* **SSD:** Crucial MX500 500GB
* **PHY:** EDUP EP-9602GS
* **WIFI:** fenvi FV-T919

### BIOS Settings

* Settings
	* Advanced
		* PCIe/PCI Sub-system Settings
			* Above 4G memory/Crypto Currency mining → **Enabled**
			* Re-Size BAR Support → **Enabled**
		* Integrated Peripherals
			* Onboard LAN Controller → **Disabled**
		* Super IO Configuration
			* Serial(COM) Port 0 Configuration
				* Serial(COM) Port0 → **Disabled**
        * USB Configuration
            * XHCI Hand-off → **Enabled**
            * Legacy USB Support → **Enabled**
	* Boot
		* Fast Boot → **Disabled**
* Overclocking
	* CPU Features
		* Intel VT-D Tech → **Disabled**
		* CFG Lock → **Disabled**
* Security
    * Trusted Computing
        * Security Device Supoort → **Enabled**
        * TPM Device Selection → **PTT**

### macOS Support

| Version   | macOS | Download |
| --------: | :---- | :------- |
| 14.2 | Sonoma | [Mac App Store](https://apps.apple.com/app/macos-sonoma/id6450717509?mt=12) |
| 13.6 | Ventura | [Mac App Store](https://apps.apple.com/app/macos-ventura/id1638787999?mt=12) |
| 12.7 | Monterey | [Mac App Store](https://apps.apple.com/app/macos-monterey/id1576738294?mt=12) |
| 11.7.10 | Big Sur | [Mac App Store](https://apps.apple.com/app/macos-big-sur/id1526878132?mt=12) |
| 10.15.7 | Catalina | [Mac App Store](https://apps.apple.com/app/macos-catalina/id1466841314?mt=12) |
| 10.14.6 | Mojave | [Mac App Store](https://apps.apple.com/app/macos-mojave/id1398502828?mt=12) |
| 10.13.6 | High Sierra | [Mac App Store](https://apps.apple.com/app/macos-high-sierra/id1246284741?mt=12) |

### Sonoma

* OCLP
	* ```boot-args: amfi=0x80 ipc_control_port_options=0```

### Emulate

* Coffee Lake (Required for Mojave)

	```Cpuid1Data: EA060900 00000000 00000000 00000000```
	
	```Cpuid1Mask: FFFFFFFF 00000000 00000000 00000000```

* Kaby Lake (Required for High Sierra)

	```Cpuid1Data: E9060900 00000000 00000000 00000000```
	
	```Cpuid1Mask: FFFFFFFF 00000000 00000000 00000000```
