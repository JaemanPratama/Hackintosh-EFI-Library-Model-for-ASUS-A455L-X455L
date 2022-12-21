<img align="right" src="https://raw.githubusercontent.com/acidanthera/OpenCorePkg/master/Docs/Logos/OpenCore_with_text_Small.png" alt="OpenCore 0.8.7" width="225">

# HACKINTOSH ASUS A455L | X455L
[![](https://img.shields.io/badge/Reposity-JaemanPratama-informational?style=flat&logo=apple&logoColor=white&color=9debeb)](https://github.com/JaemanPratama)
[![](https://img.shields.io/badge/Asus-A455L-informational?style=flat&logo=Asus&logoColor=white&color=green)](https://www.asus.com/id/)
[![](https://img.shields.io/badge/Telegram-HackintoshLover-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/HackintoshLover)
[![](https://img.shields.io/badge/Facebook-HackintoshIndonesia-informational?style=flat&logo=facebook&logoColor=white&color=3a4dc9)](https://www.facebook.com/groups/hackintosh.indonesia)
[![](https://img.shields.io/badge/Github-Issues-informational?style=flat&logo=Github&logoColor=white&color=8a178a)](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/issues)

<img align="right" src="https://help.apple.com/assets/61E8950FFC2FB340377F9335/61E89511FC2FB340377F933E/en_US/ba4de10ea93536361680a5dea7896f66.png" alt="Critter" height="180" width="175"></a>




Versi MacOS yang didukung   :
- OS X 10.11 (El Capitan)
- macOS 10.12 (Sierra)
- macOS 10.13 (High Sierra)
- macOS 10.14 (Mojave)
- macOS 10.15 (Catalina)
- macOS 11 (Big Sur)
- macOS 12 (Monterey)
- macOS 13 (Ventura) 



**:warning: Saya tidak akan bertanggung jawab atas kesalahan dalam operasi Anda!**


**Silakan lakukan riset jika Anda memiliki masalah sebelum mengganti EFI Anda dengan milik saya. Lihat [Dortania](https://dortania.github.io/getting-started/) sebelum melakukan apa pun. Saya tidak bertanggung jawab atas kehilangan apapun, termasuk namun tidak terbatas pada Kernel Panic, perangkat gagal untuk boot atau tidak dapat berfungsi secara normal, kerusakan penyimpanan atau kehilangan data**

Versi stabil menggunakan `OpenCore 0.8.3`, dan versi beta EFI menggunakan `OpenCore 0.8.7`.

```
Laptop ini adalah laptop low end, dengan spesifikasi ini,
Anda tidak dapat melakukan pekerjaan berat, daya tahan baterai sekitar 2-3 jam, 
Ini bagus tapi bukan yang terbaik, jika Anda ingin lebih,
Anda dapat memilih spesifikasi yang lebih tinggi,
tetapi pertimbangkan ini panduan mungkin berbeda untuk perangkat keras Anda.
```



## Model Perangkat Yang Telah Didukung EFI Ini:
***EFI ini dapat digunakan untuk macOS versi sebelumnya (tidak disarankan)***

### [ASUS X455LA](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases/tag/X455LA)

[![OpenCore](https://img.shields.io/badge/OpenCore-v0.8.7-blue?style=flat&logo=okta)](https://github.com/acidanthera/OpenCorePkg)

[![MacOS High Sierra](https://img.shields.io/badge/macOS-10.13.2-yellow.svg)](https://www.apple.com/li/macos/high-sierra/)
[![MacOS Mojave](https://img.shields.io/badge/macOS-10.14.2-brown.svg)](https://www.apple.com/li/macos/mojave/)
[![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-green.svg)](https://www.apple.com/li/macos/catalina/)
[![MacOS Big Sur](https://img.shields.io/badge/macOS-11.6.7-red.svg)](https://www.apple.com/macos/big-sur/)
[![MacOS Monterey](https://img.shields.io/badge/macOS-12.5-violet.svg)](https://www.apple.com/macos/monterey/)
[![MacOS Ventura](https://img.shields.io/badge/macOS-13.1-orange.svg)](https://www.apple.com/li/macos/ventura/)

<img align="right" src="https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/blob/main/Image/Untitled-3.png" width="30%">


| **Kategori**   | **Komponen**                 		
|----------------|--------------------------------------|
|**CPU**		       |2.0GHz Intel Core i3-5005U	 		            |										      
|**GPU**		       |Intel HD 5500				     		 										       |
|**RAM**         |4 + 2 GB 1600 MHz DDR3               		   |
|**SDD**         |MidasForce 256 GB SATA	 		                |
|**Layar**       |14 Inch HD LED	1366x768	 		               |										      
|**Wi-Fi/BT**    |AR9565/AR956X	  			     		                |	     
|**Bluetooth**   |3012	  			     		                         | 	  
|**Ethernet**    |Realtek RTL8111				 		                    |										      
|**Audio** 		    |Conexant CX20751/2				 		                 |
|**Input**       |PS2 Keyboard & ETD0108 ELAN Interface Touchpad |						



## Apa yang berhasil

#### CPU

Manajemen daya XCPM didukung secara native. HWP juga diaktifkan sepenuhnya.

Cek lagi dengan menggunakan aplikasi intel power gadget

#### Baterai

Tampilan daya berfungsi normal.

#### Wifi

Model nirkabel OEM adalah `Atheros ar9565`. Sarankan untuk menggantinya dengan wifi yang didukung).

> Wifi atheros hanya bekerja di MacOS mojave sampai dengan Bigsur saja.

> Fitur airplay di macOS bigsur dan diatasnya tidak berfungsi lagi


#### USB

Berfungsi normal.

#### Ethernet

Berfungsi normal.

#### Layar

Model Integrated Graphics adalah `Intel HD Graphics 5500`
VRAM telah diatur ke 3072 MB.

MacOS saat ini tidak mendukung teknologi nvidia \
Menggunakan `SSDT-DDGPU` untuk menonaktifkannya supaya menghemat daya baterai

HDMI terpasang dengan `Intel HD Graphics 5500` dan berfungsi normal.

#### Audio

Didorong oleh AppleALC dengan `layout-id: 28`. Semuanya bekerja normal.

#### Keyboard

Berfungsi normal kecuali tombol <kbd>Insert</kbd> <kbd>pause break</kbd>

Saat keyboard berhenti bekerja (not respond), solusinya adalah dengan `sleep wake` dan `restart` agar keyboard bekerja kembali

#### SSD

SSD SATA berfungsi normal dan TRIM otomatis diaktifkan dengan menggunakan `trimforce.kext`

#### Bluetooth

Berfungsi normal.

```
Memaksakan Mematikan Bluetooth di Prefensi System itu akan membuat bluetooth menjadi tidak terdeteksi 
Solusi untuk masalah tersebut adalah dengan merestart atau sleep and wake
```


#### Trackpad 

Masih memiliki banyak masalah

```
Solusi terbaik saat ini dengan menggunakan ApplePs2SmartTouchpad.kext
```


### [ASUS X455LJ](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases/tag/X455LJ)

[![OpenCore](https://img.shields.io/badge/OpenCore-v0.8.7-blue?style=flat&logo=okta)](https://github.com/acidanthera/OpenCorePkg)


[![MacOS High Sierra](https://img.shields.io/badge/macOS-10.13.2-yellow.svg)](https://www.apple.com/li/macos/high-sierra/)
[![MacOS Mojave](https://img.shields.io/badge/macOS-10.14.2-brown.svg)](https://www.apple.com/li/macos/mojave/)
[![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-green.svg)](https://www.apple.com/li/macos/catalina/)
[![MacOS Big Sur](https://img.shields.io/badge/macOS-11.6.7-red.svg)](https://www.apple.com/macos/big-sur/)
[![MacOS Monterey](https://img.shields.io/badge/macOS-12.5-violet.svg)](https://www.apple.com/macos/monterey/)
[![MacOS Ventura](https://img.shields.io/badge/macOS-13.1-orange.svg)](https://www.apple.com/li/macos/ventura/)

<img align="right" src="https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/blob/main/Image/Untitled-1.png" width="30%">

| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |2.20GHz Intel Core i5-5200U		            |										      
|**GPU**		       |Intel HD 5500				     		 										       |
|**DGPU**		       |Nvidia 920M			     		 										       |
|**RAM**         |4 + 4 GB DDR3L               		   |
|**SDD**         |Sandisk SSD Plus 120GB 		                |
|**Layar**       |14 Inch HD LED	1366x768	 		               |										      
|**Wi-Fi/BT**    |Atheros AR9565  			     		                |	     
|**Bluetooth**   |Built In 			     		                         | 	  
|**Ethernet**    |Realtek RTL8111				 		                    |										      
|**Audio** 		    |Built In 						 		                 |
|**Input**       |PS2 Keyboard & PS2 Touchpad |

## Apa yang berhasil

#### CPU

Manajemen daya XCPM didukung secara native. HWP juga diaktifkan sepenuhnya.

Cek lagi dengan menggunakan aplikasi intel power gadget

#### Baterai

Tampilan daya berfungsi normal.

#### Wifi

Model nirkabel OEM adalah `Atheros ar9565`. Sarankan untuk menggantinya dengan wifi yang didukung).

> Wifi atheros hanya bekerja di MacOS mojave sampai dengan Bigsur saja.

> Fitur airplay di macOS bigsur dan diatasnya tidak berfungsi lagi

#### USB

Berfungsi normal.

#### Ethernet

Berfungsi normal.

#### Layar

Model Integrated Graphics adalah `Intel HD Graphics 5500`
VRAM telah diatur ke 3072 MB.

MacOS saat ini tidak mendukung teknologi nvidia \
Menggunakan `SSDT-DDGPU` untuk menonaktifkannya supaya menghemat daya baterai

HDMI terpasang dengan `Intel HD Graphics 5500` dan berfungsi normal.

#### Audio

Didorong oleh AppleALC dengan `layout-id: 28`. Semuanya bekerja normal.

#### Keyboard

Berfungsi normal kecuali tombol <kbd>Insert</kbd> <kbd>pause break</kbd>

Saat keyboard berhenti bekerja (not respond), solusinya adalah dengan `sleep wake` dan `restart` agar keyboard bekerja kembali

#### SSD

SSD SATA berfungsi normal dan TRIM otomatis diaktifkan dengan menggunakan `trimforce.kext`

#### Bluetooth

Berfungsi normal.

```
Memaksakan Mematikan Bluetooth di Prefensi System itu akan membuat bluetooth menjadi tidak terdeteksi 
Solusi untuk masalah tersebut adalah dengan merestart atau sleep and wake
```


#### Trackpad 

Masih memiliki banyak masalah

```
Solusi terbaik saat ini dengan menggunakan ApplePs2SmartTouchpad.kext
```

### [ASUS A455LB](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases/tag/A455LB) 

[![OpenCore](https://img.shields.io/badge/OpenCore-v0.8.7-blue?style=flat&logo=okta)](https://github.com/acidanthera/OpenCorePkg)

[![MacOS High Sierra](https://img.shields.io/badge/macOS-10.13.2-yellow.svg)](https://www.apple.com/li/macos/high-sierra/)
[![MacOS Mojave](https://img.shields.io/badge/macOS-10.14.2-brown.svg)](https://www.apple.com/li/macos/mojave/)
[![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-green.svg)](https://www.apple.com/li/macos/catalina/)
[![MacOS Big Sur](https://img.shields.io/badge/macOS-11.6.7-red.svg)](https://www.apple.com/macos/big-sur/)
[![MacOS Monterey](https://img.shields.io/badge/macOS-12.5-violet.svg)](https://www.apple.com/macos/monterey/)
[![MacOS Ventura](https://img.shields.io/badge/macOS-13.1-orange.svg)](https://www.apple.com/li/macos/ventura/)

<img align="right" src="https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/blob/main/Image/Asus%20A455L%20Background%20Remove.png?raw=true" width="30%">


| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |2.20GHz Intel Core i5-5200U  |										      
|**GPU**		       |Intel HD 5500				     		 										       |
|**DGPU**		       |Nvidia 940M			     		 										       |
|**RAM**         |4 + 4 1600MHz GB DDR3L               		   |
|**SDD**         |Apacer AS340 PANTHER 240GB SATA III SSD + HDD 1TB 		                |
|**Layar**       |14 Inch HD LED	1366x768	 		               |										      
|**Wi-Fi/BT**    |Atheros AR9565  			     		                |	     
|**Bluetooth**   |Built In 			     		                         | 	  
|**Ethernet**    |Realtek RTL8111				 		                    |										      
|**Audio** 		   |Conexant CX20751/2					 		                 |
|**Input**       |PS2 Keyboard & Focaltech PS2 Touchpad |

## Apa yang berhasil

#### CPU

Manajemen daya XCPM didukung secara native. HWP juga diaktifkan sepenuhnya.

Cek lagi dengan menggunakan aplikasi intel power gadget

#### Baterai

Tampilan daya berfungsi normal.

#### Wifi

Model nirkabel OEM adalah `Atheros ar9565`. Sarankan untuk menggantinya dengan wifi yang didukung).

> Wifi atheros hanya bekerja di MacOS mojave sampai dengan Bigsur saja.

> Fitur airplay di macOS bigsur dan diatasnya tidak berfungsi lagi

#### USB

Berfungsi normal.

#### Ethernet

Berfungsi normal.

#### Layar

Model Integrated Graphics adalah `Intel HD Graphics 5500`
VRAM telah diatur ke 3072 MB.

MacOS saat ini tidak mendukung teknologi nvidia \
Menggunakan `SSDT-DDGPU` untuk menonaktifkannya supaya menghemat daya baterai

HDMI terpasang dengan `Intel HD Graphics 5500` dan berfungsi normal.

#### Audio

Didorong oleh AppleALC dengan `layout-id: 28`. Semuanya bekerja normal.

#### Keyboard

Berfungsi normal kecuali tombol <kbd>Insert</kbd> <kbd>pause break</kbd>

Saat keyboard berhenti bekerja (not respond), solusinya adalah dengan `sleep wake` dan `restart` agar keyboard bekerja kembali

#### SSD

SSD SATA berfungsi normal dan TRIM otomatis diaktifkan dengan menggunakan `trimforce.kext`

#### Bluetooth

Berfungsi normal.

```
Memaksakan Mematikan Bluetooth di Prefensi System itu akan membuat bluetooth menjadi tidak terdeteksi 
Solusi untuk masalah tersebut adalah dengan merestart atau sleep and wake
```


#### Trackpad 

Masih memiliki banyak masalah

```
Solusi terbaik saat ini dengan menggunakan ApplePs2SmartTouchpad.kext
```

### [ASUS A455LF](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases/tag/A455LF) 

[![OpenCore](https://img.shields.io/badge/OpenCore-v0.8.7-blue?style=flat&logo=okta)](https://github.com/acidanthera/OpenCorePkg)

[![MacOS High Sierra](https://img.shields.io/badge/macOS-10.13.2-yellow.svg)](https://www.apple.com/li/macos/high-sierra/)
[![MacOS Mojave](https://img.shields.io/badge/macOS-10.14.2-brown.svg)](https://www.apple.com/li/macos/mojave/)
[![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-green.svg)](https://www.apple.com/li/macos/catalina/)
[![MacOS Big Sur](https://img.shields.io/badge/macOS-11.6.7-red.svg)](https://www.apple.com/macos/big-sur/)
[![MacOS Monterey](https://img.shields.io/badge/macOS-12.5-violet.svg)](https://www.apple.com/macos/monterey/)

<img align="right" src="https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/blob/main/Image/Untitled-2.png" width="30%">

| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |1,7GHz Intel Core i3-4005U  |										      
|**GPU**		       |Intel HD 4400				     		 										       |
|**DGPU**		       |Nvidia 930M			     		 										       |
|**RAM**         |4 + 4 1600MHz GB DDR3L               		   |
|**SDD**         |SSD SATA III  		                |
|**Layar**       |14 Inch HD LED	1366x768	 		               |										      
|**Wi-Fi/BT**    |Built In 	  			     		                |	     
|**Bluetooth**   |Built In 			     		                         | 	  
|**Ethernet**    |Realtek RTL8111				 		                    |										      
|**Audio** 		   |Sonic Master Audio					 		                 |
|**Input**       |PS2 Keyboard & Asus PS2 Touchpad |

## Apa yang berhasil

#### CPU

Manajemen daya XCPM didukung secara native. HWP juga diaktifkan sepenuhnya.

Cek lagi dengan menggunakan aplikasi intel power gadget

#### Baterai

Tampilan daya berfungsi normal.

#### Wifi

Model nirkabel OEM adalah `Atheros ar9565`. Sarankan untuk menggantinya dengan wifi yang didukung).

> Wifi atheros hanya bekerja di MacOS mojave sampai dengan Bigsur saja.

> Fitur airplay di macOS bigsur dan diatasnya tidak berfungsi lagi

#### USB

Berfungsi normal.

#### Ethernet

Berfungsi normal.

#### Layar

Model Integrated Graphics adalah `Intel HD Graphics 4400`
VRAM telah diatur ke 3072 MB.

MacOS saat ini tidak mendukung teknologi nvidia \
Menggunakan `SSDT-DDGPU` untuk menonaktifkannya supaya menghemat daya baterai

HDMI terpasang dengan `Intel HD Graphics 4400` dan berfungsi normal.

#### Audio

Didorong oleh AppleALC dengan `layout-id: 28`. Semuanya bekerja normal.

#### Keyboard

Berfungsi normal kecuali tombol <kbd>Insert</kbd> <kbd>pause break</kbd>

Saat keyboard berhenti bekerja (not respond), solusinya adalah dengan `sleep wake` dan `restart` agar keyboard bekerja kembali

#### SSD

SSD SATA berfungsi normal dan TRIM otomatis diaktifkan dengan menggunakan `trimforce.kext`

#### Bluetooth

Berfungsi normal.

```
Memaksakan Mematikan Bluetooth di Prefensi System itu akan membuat bluetooth menjadi tidak terdeteksi 
Solusi untuk masalah tersebut adalah dengan merestart atau sleep and wake
```


#### Trackpad 

Masih memiliki banyak masalah

```
Solusi terbaik saat ini dengan menggunakan ApplePs2SmartTouchpad.kext
```

### [ASUS A455LD](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases/tag/A455LD)

[![OpenCore](https://img.shields.io/badge/OpenCore-v0.8.7-blue?style=flat&logo=okta)](https://github.com/acidanthera/OpenCorePkg)

[![MacOS High Sierra](https://img.shields.io/badge/macOS-10.13.2-yellow.svg)](https://www.apple.com/li/macos/high-sierra/)
[![MacOS Mojave](https://img.shields.io/badge/macOS-10.14.2-brown.svg)](https://www.apple.com/li/macos/mojave/)
[![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-green.svg)](https://www.apple.com/li/macos/catalina/)
[![MacOS Big Sur](https://img.shields.io/badge/macOS-11.6.7-red.svg)](https://www.apple.com/macos/big-sur/)
[![MacOS Monterey](https://img.shields.io/badge/macOS-12.5-violet.svg)](https://www.apple.com/macos/monterey/)

<img align="right" src="https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/blob/main/Image/Untitled-4.png" width="30%">

| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |2.70 GHz Intel Core i5-4210U  |										      
|**GPU**		       |Intel HD 4400				     		 										       |
|**DGPU**		       |Nvidia GT 820M			     		 										       |
|**RAM**         |4 GB DDR3               		   |
|**SDD**         |SSD SATA III  		                |
|**Layar**       |14 Inch HD LED	1366x768	 		               |										      
|**Wi-Fi/BT**    |Built In 	  			     		                |	     
|**Bluetooth**   |Built In 			     		                         | 	  
|**Ethernet**    |Realtek RTL8111				 		                    |										      
|**Audio** 		   |Sonic Master Audio					 		                 |
|**Input**       |PS2 Keyboard & Asus PS2 Touchpad |

## Apa yang berhasil

#### CPU

Manajemen daya XCPM didukung secara native. HWP juga diaktifkan sepenuhnya.

Cek lagi dengan menggunakan aplikasi intel power gadget

#### Baterai

Tampilan daya berfungsi normal.

#### Wifi

Model nirkabel OEM adalah `Atheros ar9565`. Sarankan untuk menggantinya dengan wifi yang didukung).

> Wifi atheros hanya bekerja di MacOS mojave sampai dengan Bigsur saja.

> Fitur airplay di macOS bigsur dan diatasnya tidak berfungsi lagi

#### USB

Berfungsi normal.

#### Ethernet

Berfungsi normal.

#### Layar

Model Integrated Graphics adalah `Intel HD Graphics 4400`
VRAM telah diatur ke 3072 MB.

MacOS saat ini tidak mendukung teknologi nvidia \
Menggunakan `SSDT-DDGPU` untuk menonaktifkannya supaya menghemat daya baterai

HDMI terpasang dengan `Intel HD Graphics 4400` dan berfungsi normal.

#### Audio

Didorong oleh AppleALC dengan `layout-id: 28`. Semuanya bekerja normal.

#### Keyboard

Berfungsi normal kecuali tombol <kbd>Insert</kbd> <kbd>pause break</kbd>

Saat keyboard berhenti bekerja (not respond), solusinya adalah dengan `sleep wake` dan `restart` agar keyboard bekerja kembali

#### SSD

SSD SATA berfungsi normal dan TRIM otomatis diaktifkan dengan menggunakan `trimforce.kext`

#### Bluetooth

Berfungsi normal.

```
Memaksakan Mematikan Bluetooth di Prefensi System itu akan membuat bluetooth menjadi tidak terdeteksi 
Solusi untuk masalah tersebut adalah dengan merestart atau sleep and wake
```


#### Trackpad 

Masih memiliki banyak masalah

```
Solusi terbaik saat ini dengan menggunakan ApplePs2SmartTouchpad.kext
```

## INSTALASI


## Mulailah dengan bios.

<details>
  <summary><strong> Menyiapkan dengan Bios</strong></summary>
 
   Catatan: Beberapa opsi ini mungkin tidak ada di Bios Anda. Jika Anda tidak menemukan beberapa bios, tinggalkan dan jangan khawatir.

   **Cara Memasuki Bios:**\
Tekan **F2** 
  
<details>
<summary><strong>Aktifkan:</strong></summary>
 
*  *Intel* Virtualization → Enabled
*  *VT-d* → Enabled
*  *Graphics Configuration* → DVMT Pre-Allocation → 64M / default 32M tetapi perlu tambalan 
*  *USB Configuration* → XHCI Pre-Boot Mode → Enabled / Smart Auto jika menggunakan perangkat EHCI
*  *SATA Mode* → AHCI
  </details>
 
 
<details>
  <summary><strong>Nonaktifkan:</strong></summary>
 
*  *Security* → Secure Boot → Disabled
*  *Boot* → Launch CSM → Disabled untuk Resolusi Boot OC

</details>

Setelah mengatur pengaturan ini di bios, simpan dan keluar.
</details>

**Ini adalah rangkuman sederhana dan cepat dari pembuatan USB pemasangan online.**

### Penginstal macOS Bigsur dengan Pengguna Windows dan Mac:
<details>
  <summary><strong>Process 1. MacOS BigSur Online Installer dari Windows, linux dan macOS:</strong></summary>
 
   - **`Untuk pengguna Windows`**
 
      1. Download [rufus](https://rufus.ie/en/) untuk memformat sdcard ke fat32.
      2. Pilih flash drive atau Sdcard yang Anda inginkan untuk menginstal penginstal di bawah opsi perangkat
      3. Buka rufus dan Pilih `non-bootable` sebagai `pemilihan boot` (WAJIB)
      4. Pilih `FAT-32` atau `Large FAT-32` sebagai skema partisi. Tekan mulai (dengan melakukan ini format sdcard sehingga Anda akan kehilangan semua data di sdcard).
      5. Jika di windows, Buka partisi usb di file explorer dan hapus semua file yang dibuat oleh rufus secara manual.

   - **`Untuk pengguna mac`**

          1. Luncurkan `Utilitas Disk`
          2. `Pilih Tampilan` > `Tampilkan semua perangkat` di kiri atas
          3. Pilih flash drive Anda (root perangkat usb) dan format sebagai `MS-DOS (FAT)` atau `FAT-32`.
          4. ubah `guid patition table`-> `Master Boot Record Partiton`.
          5. tekan mulai (dengan melakukan ini format sdcard sehingga Anda akan kehilangan semua data di sdcard).
       
   - **`Untuk pengguna Linux`**
  
   1. Instal `gparted` dan format usb ke `Fat32` dan `MBR` ATAU `MASTER BOOT RECORD PARTITION.
   2. SELESAI.
  
6. Lalu ......................
7. Sekarang, Instal Python dari toko Microsoft atau Unduh secara manual untuk pengguna MAC, linux dan Windows di sini -> [python](https://www.python.org/downloads/) (Pastikan Anda memilih tambahkan python x.x ke jalur ke variabel lingkungan untuk pengguna windows.)
8. Unduh dan ekstrak [Paket OpenCore](https://github.com/acidanthera/OpenCorePkg/releases) (Versi release).
9. Pilih folder "macrecovery" di folder "opencorepkg" di `/Utilities/macrecovery/` .
10. Salin jalur folder "macrecovery" di pengelola file atau pencari.
11. Jalankan command prompt atau Terminal dan ketik `cd` dan tekan bilah spasi dan rekatkan jalur folder macrecovery.
12.Jika Anda tidak dapat menjalankan perintah ini, tambahkan `python` atau `python3` ke awal kode ini.
   - Untuk BigSur -Jalankan perintah: `macrecovery.py -b Mac-42FD25EABCABB274 -m 000000000000000000 download`
   - Untuk Monterey -Jalankan perintah: `macrecovery.py -b Mac-E43C1C25D4880AD6 -m 000000000000000000 download`

13. Ini akan mengunduh beberapa file di folder macrecovery tetapi kita hanya perlu "BaseSystem.dmg" dan "BaseSystem.chunklist" (membutuhkan sekitar 600mb hingga 800mb internet) untuk Mengunduh penginstal Macos.
14. Buat folder di USB atau flashdisk atau flash drive bernama `com.apple.recovery.boot`.
15. Paste kedua file tersebut di folder `com.apple.recovery.boot` di partisi flash drive atau sdcard atau flashdisk anda.
16. Unduh EFI terbaru yang dibuat [di sini](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases)
17. Salin folder bernama `EFI` dan tempel di partisi USB Anda.

**Catatan: Jika Anda perlu mengedit Config.plist, jangan Clover configurator karena opencore. Gunakan konfigurator OpenCore , gunakan PlistEdit pro, PropperTree, atau Xcode.**

** Anda hanya akan mendapatkan gangguan tampilan saat menginstal macOS melalui USB atau flash drive apa pun. Tapi Anda tidak akan mendapatkan setidaknya satu kesalahan setelah menginstal macos atau menggunakan MacOS sebagai driver harian.**

`Catatan: Pastikan untuk menerapkan pengaturan bios yang benar sebelum melanjutkan (disediakan di atas)`

  18. Nyalakan kembali laptop Anda dan tekan tombol <kbd> F2 </kbd> terus menerus hingga Anda masuk ke pengaturan bios.
`Catatan: Pastikan untuk menerapkan pengaturan bios yang benar sebelum melanjutkan (disediakan di atas)`
19. Pilih flash drive Anda sebagai opsi boot sementara di menu boot.
20. Sekarang di menu OpenCore pilih nama partisi USB Anda
21. Baik! Sekarang instal dan atur macOS Big Sur seperti biasa (Proses ini membutuhkan internet 14gb untuk mengunduh Macos bigsur lengkap).
22. sistem reboot untuk sekali atau dua kali, ketika reboot pilih usb setiap kali sampai Anda melihat nama Partisi Macos Anda di menu boot.
23. Setelah mem-boot ke OS, Anda perlu mengunduh konfigurator opencore dan memasang drive sistem, Kemudian Tempelkan efi ke efi yang terpasang dari USB atau drive. lalu reboot dan hapus usb.

  </details>
  <details>
   <summary><strong>Process 2. MacOS BigSur Offline Installer dari Windows dan macOS:</strong></summary>
 
- 1.Cari dan Unduh Olarila BigSur atau Monterey .raw dari [Di Sini](https://www.olarila.com/topic/6278-hackintosh-and-macintosh-olarila-vanilla-images-macos/)versi terbaru dari bigsur adalah 11.xxxx dan untuk Monterey adalah 12.xxxx
- 2.Unduh etsa dari [di sini](https://www.balena.io/etcher/)
- 3.Membuat Usb bootable (Flash the Sdcard) menggunakan Etcher dan olarila bigsur.
- 4.pasang efi dari Sdcard atau drive yang dapat di-boot.
- Untuk pengguna mac gunakan Opencore Configurator.app official [di sini](https://mackie100projects.altervista.org/download-opencore-configurator/)
- 5.Hapus folder EFI default yang ada di bootable usb
- 6.dan tempelkan Efi ke USB. Unduh Efi [di sini](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases)

**Catatan: Jika Anda perlu mengedit Config.plist, jangan Clover configurator karena opencore. Gunakan konfigurator OpenCore , gunakan PlistEdit pro, PropperTree, atau Xcode.**

** Anda hanya akan mendapatkan gangguan tampilan saat menginstal macOS melalui USB atau flash drive apa pun. Tapi Anda tidak akan mendapatkan setidaknya satu kesalahan setelah menginstal macos atau menggunakan MacOS sebagai driver harian.**

- 7.Restart laptop Anda dan tekan tombol `Delete` terus menerus hingga Anda masuk ke pengaturan bios.
- 8.Pilih kartu sd atau flash drive Anda sebagai opsi boot sementara di menu boot.
- 9. Sekarang di menu OpenCore pilih nama partisi USB Anda
- instal. Nikmati!!!!

</details>

<details>
 
<summary><strong>Setelah boot ke Macos Recovery</strong></summary>
 

** Anda mungkin mendapatkan gangguan tampilan hanya saat menginstal macOS melalui USB atau flash drive apa pun. Tapi Anda tidak akan mendapatkan setidaknya SATU glitch setelah menginstal macos atau Menggunakan MacOS sebagai driver harian.**

         - 1. buka `Disk Utiliy` -> Pilih `View` yang ada di kiri atas -> pilih `Show all devices` -> Pilih root dari `SSD drive storage` yang ingin Anda instal MacOS (root SSD drive) perangkat) -> Klik `Hapus` -> `Namai` drive Anda sesuka Anda, Lebih disukai untuk menamai sebagai `Macintosh` ATAU `Macintosh HD` -> ubah `Format` menjadi `APFS` -> `Scheme` menjadi `Guid Patition Peta` -> Klik `Hapus` .
         - 2. Klik `done` dan tutup jendela `disk utility`.
         - 3. Pilih `Install MacOS <macos_version_here>` & klik `continue` -> pilih `SSD drive name` yang telah Anda ganti namanya sebelumnya di Disk Utility dan klik `continue` .
         - 4. Pemasang membutuhkan waktu 1-3 jam untuk menginstal untuk proses online & offline.

#### Catatan : Jangan matikan layar, sampai instalasi selesai atau sampai reboot. Jika layar mati dalam proses instalasi, reboot dan Anda perlu melakukan proses instalasi yang sama.
 

- Setelah mem-boot ke OS, di `setup` Anda akan melihat `File-Vault` harus dinonaktifkan atau dimatikan. Setelah penyiapan, Anda hanya perlu melakukan sedikit pekerjaan, baca post-install-0

</details>

<hr>

## Layout Partisi:
```
╭─[~/Downloads/EFI]─[Hackpro]
╰─[:)] % diskutil list
/dev/disk0 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *1.0 TB     disk0
   1:                        EFI EFI                     209.7 MB   disk0s1
   2:                  Apple_HFS Hackintosh               118.6 GB   disk0s3
   3:                 Apple_Boot Recovery HD             650.0 MB   disk0s4
   4:       Microsoft Basic Data DATA                    697.9 GB   disk0s7

/dev/disk1 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *120.0 GB   disk1
   1:         Microsoft Reserved                         16.8 MB    disk1s1
   2:       Microsoft Basic Data                         120.0 GB   disk1s2
```

# Post Install
Setelah Anda memverifikasi bahwa mesin Anda melakukan booting dengan benar tanpa masalah seperti yang dijelaskan di bagian "Apa Yang Berhasil", lanjutkan untuk melakukan hal berikut
  
Berdasarkan [Panduan Pasca-Instal OpenCore Dortania](https://dortania.github.io/OpenCore-Post-Install/).

<details><summary><strong>0.Boot os tanpa usb atau drive apa pun</strong></summary>
 
Setelah mem-boot ke OS, Anda tidak dapat mem-boot tanpa usb, karena EFI ada di USB. Jadi, Anda perlu mengunduh konfigurator opencore [tautan](https://mackie100projects.altervista.org/opencore-configurator/) -> buka `opencore-configurator` berikan izin di `system prefereneces` -> `security` -> `open anyway`. buka `opencore-configurator` lagi -> pasang `EFI` dan rekatkan `EFI<folder>` ke `EFI partition`.
  - Lepas USB dan reboot. `RESET-NVRAM` sekali dalam menu boot opencore dan reboot..Selesai...

 
</details>

<details><summary><strong>1.Nonaktifkan teks layar hitam saat booting</strong></summary>

(Menonaktifkan mode Verbose) Pengguna hackintosh baru menggunakan ini. Untuk menonaktifkannya, Di Config.plist, navigasikan ke 'NVRAM' -> buka Add `7C436110-AB2A-4BBB-A880-FE41995C9F82` -> `boot-args` -> hapus argumen `-v`. Simpan dan reboot.
  </details>

<details><summary><strong>2.Nonaktifkan ShowPicker</strong></summary>
 
Jangan gunakan ini jika Anda menggunakan dual boot. Di Config.plist, Anda dapat menonaktifkan layar boot picker sehingga Anda langsung boot ke logo Apple dengan mengatur di bawah `Misc` -> `Boot` -> `ShowPicker` False (NO)
Catatan: Anda masih dapat melihat boot picker dengan ShowPicker disetel ke no/false dengan mengirim spam ke <kbd>alt</kbd> + <kbd>Esc</kbd> sebelum logo apel ditampilkan saat boot.
</details>
  
  <details><summary><strong>3.Aktifkan FileVault</strong></summary>
   
  [FileVault](https://support.apple.com/en-us/HT204837) digunakan untuk mengenkripsi disk mulai di Hackintosh Anda. Mengaktifkannya sepenuhnya opsional, tetapi mungkin ide yang bagus untuk kesadaran keamanan. Sebelum mengaktifkan fitur ini, Anda harus memastikan bahwa OpenCore telah dikonfigurasi dengan benar untuk berinteraksi dengan drive terenkripsi. Ikuti Panduan Pasca-Instal OpenCore untuk [menyiapkan file config.plist Anda untuk digunakan dengan FileVault](https://dortania.github.io/OpenCore-Post-Install/universal/security/filevault.html).

Perubahan (opsional) berikut telah dibuat:

* `Misc > Boot > PollAppleHotKeys` → `True`
* `Misc > Keamanan > AuthRestart` → `True`

Anda sekarang dapat mengaktifkan FileVault di Keamanan & Privasi di Preferensi Sistem seperti di Mac asli. Setelah proses enkripsi selesai, kata sandi akun Anda akan diminta untuk mendekripsi disk pengaktifan setiap kali Hackintosh Anda dijalankan.

Catatan: Anda juga harus melakukan perubahan ini pada konfigurasi OpenCore drive USB Anda sehingga dapat mem-boot sistem Anda dengan benar jika partisi EFI `Macintosh SSD` menjadi kacau. Jika Anda tidak memperbarui konfigurasi, bootloader OpenCore mungkin tidak dapat menangani drive terenkripsi FileVault dengan benar
    
  </details>

<details><summary><strong>4.Bersihkan Memperbarui EFI Anda dengan rilis EFI baru</strong></summary>

Untuk memperbarui EFI Anda dengan EFI Rilis baru. Langkah langkah:-

1) Unduh EFI Rilis baru dari [di sini](https://github.com/JaemanPratama/Hackintosh-EFI-Library-Asus-A455L-X455L-Model/releases)

2) Ambil cadangan file SMBios atau windows 
 fboot ke folder lain, jika diperlukan. (jika Anda ingin mencadangkan SMBIOS, salin `nomor seri sistem`, `UUID sistem`, `MLB`, `ROM`, `Nama produk sistem`.)

3) Sekarang tambahkan SMBIOS tersebut atau tempatkan file Windows EFI sebagaimana mestinya di EFI lama ke EFI baru, jika Anda telah membuat cadangan sebelumnya.

4) Pasang partisi EFI, Hapus EFI LAMA.

5) Salin dan tempel EFI baru ke partisi EFI.

6) tekan reboot, Ingatlah untuk hanya melakukan Reset NVRAM satu kali.

7) Selesai, Anda telah melakukan Pembaruan EFI yang bersih.

</details>

<details><summary><strong>5. Tambahkan Properti Perangkat untuk Serial number, MLB, ROM, System-UUID.</strong></summary>
 
Gunakan SMBios `MacBookAir9,1`. Direkomendasikan : opencore configurator, Buka `PlatformInfo >SMBios`Centang "Add to the section to config file" di `SMBIOS` dan `DATAHUB -GENERIC- PLATFORMNVRAM` dan lanjutkan Menambahkan SMBIOS Anda.
Ikuti [panduan Opencore](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial) ini untuk mengatur nomor seri dan info yang menyertai untuk mendapatkan iServices.
 
  Trik untuk Mendapatkan detail Prosesor yang tepat di Informasi Sistem - Saat Anda menambahkan smbios, Edit `processor type` -> `0` atau hapus di dalam `processor-type` .
  </details>
 
<details><summary><strong>6. Perbaiki Imessage dan Facetime.</strong></summary>
 
Jika Anda baru mengenal akun apple atau jika Anda menggunakan akun apple untuk pertama kalinya di hackintosh, Anda perlu menggunakan akun apple selama satu bulan dan menggunakan icloud. Padahal imessage atau factime tidak jalan..
Masalahnya adalah "Gunakan" selama sebulan atau lebih dan secara otomatis setelah beberapa hari, secara ajaib facetime dan imessages bekerja ... Tada ...
  </details>
 
  <details><summary><strong>7. Install Windows di Pre-installed MacOS (Dual-Boot).</strong></summary>
 
  - Proses ini sangat sederhana untuk dual boot dan dapat menanyakan keraguan dan masalah di sini.
 
  1. Ambil Usb atau sd-card, sambungkan ke pc & Luncurkan `Disk Utility` -> Pilih `View` > `Show all devices` di kiri atas.
  2. Pilih perangkat flash Anda (root perangkat usb Anda) dan format sebagai `MS-DOS (FAT)` atau `FAT-32`. Ubah `guid patition table` -> `Master Boot Record Partiton`. Tekan mulai (dengan melakukan ini format sdcard sehingga Anda akan kehilangan semua data di sdcard).
  3. Salin EFI yang Anda gunakan sekarang ke perangkat `USB`.
  4. Selanjutnya, untuk mempartisi drive Anda, -> Luncurkan `Disk Utility` -> Pilih `View` > `Show all devices` di kiri atas -> Pilih `MacOS-drive` Anda sebagai root -> Klik `Partition` - > klik `tambahkan partisi` jika Anda melihat munculan -> `Namai` partisi Anda. -> Ubah jenis `Format` menjadi `ExFat` atau `Ms-dos` -> Sesuaikan `Ukuran partisi` sesuka Anda. klik `Terapkan`. Proses ini memakan waktu minimal 15 menit.
  5. Ambil USB Lain, Sekarang Jadikan bootable dari versi windows yang diperlukan oleh rufus atau lainnya.
  6. Boot ke USB dari bios. Jalankan Penginstal windows sebagai Asusual. Tapi ingat untuk menginstal di Partisi windows Anda di `tempat menginstal` di disk windows.
  7. Saat Anda boot ke windows, instal semua Pembaruan dan Anda juga dapat memulai ulang saat pembaruan memerlukan reboot. (Lupakan tentang macOS untuk saat ini). Setelah menginstal semua pembaruan, Colokkan `EFI usb` atau sdcard (yang sebelumnya Anda salin folder EFI dan Microsoft) dan reboot ke usb dari bios untuk boot ke MacOS.
  8. Saat Anda mem-boot ke MacOS, <ins>Pasang folder EFI</ins>, dan Ganti EFI default (drive efi) dengan usb atau sdcard EFI Anda. Lepas EFI dan reboot.
  9. Coba periksa menu boot dengan Reboot ke macOS & Windows. (Anda dapat melihat "MacOS" & "Windows" di menu boot)..
  10. Sekarang Anda dapat dengan mudah mendapatkan Windows & MacOS di menu boot.
 
  </details>
  
<details><summary><strong>8.Instal Utilitas Boot Camp.</strong></summary>
  
  Untuk kembali ke macOS dari Windows tanpa memerlukan input pengguna selama boot, [Perangkat Lunak Dukungan Windows](https://support.apple.com/en-us/HT204923) Apple harus diinstal. Panduan Pasca-Instal OpenCore mencakup [petunjuk penggunaan alat pihak ketiga untuk mengunduh driver ini](https://dortania.github.io/OpenCore-Post-Install/multiboot/bootcamp.html). Namun, mereka juga dapat diunduh langsung di macOS menggunakan Boot Camp Assistant.

1. Luncurkan Boot Camp Assistant dan pilih item menu `Action > Download Windows Support Software`

2. Salin file yang diunduh ke drive USB yang kompatibel dengan Windows dan reboot ke Windows

3. Hapus semua driver Boot Camp yang tidak diperlukan:
    * Semua folder di `$WinPEDriver$` (simpan folder induk)
    * Semua folder di `BootCamp/Drivers/` **kecuali** `Apple/`
    * Semua folder/file di `BootCamp/Drivers/Apple/` **kecuali** `BootCamp.msi`
   
    <br/>
   
    ![File Kamp Pelatihan yang Tersisa](https://user-images.githubusercontent.com/867617/111693344-e3534a80-8806-11eb-8442-510c9500b299.png)

4. Jalankan `BootCamp/Setup.exe` untuk menginstal perangkat lunak Boot Camp.

5. Sekarang Anda dapat menggunakan Panel Kontrol Boot Camp di bilah tugas untuk memulai ulang langsung ke macOS tanpa memerlukan input pengguna lebih lanjut, seperti pada Mac asli yang menjalankan Boot Camp.

![Panel Kontrol dan Asisten Boot Camp](https://user-images.githubusercontent.com/867617/111683749-44c1ec00-87fc-11eb-8932-c747264443bc.png)
  
  </details>


<details><summary><strong>9.Pemetaan port USB.</strong></summary>

menggunakan [Hackintool](https://github.com/headkaze/Hackintool) atau [USBMap](https://github.com/corpnewt/USBMap)
</details>

<details><summary><strong>10.Perbaikan audio.</strong></summary>

- https://hackintosher.com/guides/get-hackintosh-audio-working/

| Device-Preset         | AppleALC ID | Audio Output | Output Switch | Microphone | Feature    |
| --------------------- | ----------- | ------------ | ------------- | ---------- | ---------- |
| Asus A455LD,  | alcid=3     | ✓            | ✓             | ✓          | Line-In          |
| Asus A455LF   | alcid=21    | ✓            | ✓             | ✓          | Line-In          |
| Asus X455LA, X455LJ  | alcid=28    | ✓            | ✓             | ✓          | Line-In          |


</details>

 
<hr>

Beritahu saya, Jika ada kesalahan / kesalahan ejaan dalam Instalasi atau di mana ...

## Alat yang digunakan : Opencore Configurator, Opencore EFI Bootloader, MaciASL, Hackintool, IORegistryExplorer
- https://mackie100projects.altervista.org/download-opencore-configurator/
- https://github.com/acidanthera/OpenCorePkg/releases
- https://github.com/acidanthera/MaciASL
- https://github.com/headkaze/Hackintool
- https://karabiner-elements.pqrs.org
- https://software.intel.com/content/www/us/en/develop/articles/intel-power-gadget.html

## Kexts penting untuk diperbarui untuk setiap versi macOS
- https://github.com/acidanthera/WhateverGreen
- https://github.com/acidanthera/Lilu
- https://github.com/acidanthera/AppleALC

## ACPI-Patching Tools

- [Piker-Alpha/ssdtPRGen](https://github.com/Piker-Alpha/ssdtPRGen.sh)
- [corpnewt/SSDTTime](https://github.com/corpnewt/SSDTTime)
- [acidanthera/MaciASL](https://github.com/acidanthera/MaciASL)

---

### Tautan Berguna

## ACPI

- [Menambal DSDT/SSDT untuk kontrol lampu latar LAPTOP](https://www.tonymacx86.com/threads/guide-patching-dsdt-ssdt-for-laptop-backlight-control.152659/)
- [Perbaiki Tombol Pintas Keyboard / Tombol Fungsional](https://www.insanelymac.com/forum/topic/330440-beginners-guide-fix-keyboard-hot-keys-functional-keys/)
- [RehabMan/OS-X-ACPI-Debug](https://github.com/RehabMan/OS-X-ACPI-Debug)

## PCI

- [OpenCore tanpa akselerasi keyboard/touchpad/gpu](https://www.olarila.com/topic/6730-opencore-no-keyboardtouchpadgpu-accelleration/?tab=comments#comment-86076)
- [Cara menambahkan properti perangkat untuk OpenCore](https://www.youtube.com/watch?v=hD0kpsQHIIc)

## Tidur

- [Apa perbedaan antara hibernatemode=0 dan hibernatemode=3](https://www.tonymacx86.com/threads/what-is-different-between-hibernatemode-0-and-hibernatemode-3.164030/)
- [Cara Memilih Mode Tidur Mac](https://mackeeper.com/blog/post/366-do-you-know-what-sleep-mode-is-the-best-for-your-mac/)

## Manajemen daya

- [Apa yang dilakukan -xcpm?](https://www.reddit.com/r/hackintosh/comments/85e8hn/what_does_xcpm_do/)
- [X86PlatformPlugin Customization und Anpassung – Perfektes Speedstepping](https://www.hackintosh-forum.de/forum/thread/48025-cpufriend-guide-hwp-speedstep-x86platformplugin-vs-acpi-smc-platformplugin/)

## Keamanan

- [OpenCore Post-Install: Apple Secure Boot](https://dortania.github.io/OpenCore-Post-Install/universal/security/applesecureboot.html#what-is-apple-secure-boot)
- [Melindungi data di beberapa lapisan](https://developer.apple.com/news/?id=3xpv8r2m)
- [Volume snapshot? com.apple.os.update-xxxxxx di Disk Utility](https://discussions.apple.com/thread/252032330)
- [Perubahan APFS di Big Sur: cara Time Machine mencadangkan ke APFS, dan lainnya](https://eclecticlight.co/2020/06/29/apfs-changes-in-big-sur-how-time-machine-backs-up-to-apfs-and-more/)
- [Volume Sistem Bertanda Tangan Big Sur: perlindungan keamanan tambahan](https://eclecticlight.co/2020/06/25/big-surs-signed-system-volume-added-security-protection/)
- [Apakah volume sistem Big Sur disegel?](https://eclecticlight.co/2020/11/30/is-big-surs-system-volume-sealed/)

## Kesalahan

- [Kode Error Filevault](https://support.addigy.com/support/solutions/articles/8000056056-filevault-error-codes)
- [Perbaiki Mac Anda yang macet saat dienkripsi dengan FileVault](https://www.macissues.com/2014/12/16/fix-your-mac-stuck-on-encrypting-with-filevault/)
- [FileVault Stuck saat Enkripsi Dijeda](https://forums.macrumors.com/threads/filevault-stuck-on-paused-encryption.1952148/)
- [FileVault Stuck on Pause](https://apple.stackexchange.com/questions/160161/filevault-stuck-on-pause)

## Tombol FN

- [Kecerahan Keyboard FN ASUS UX32VD macOS 11.1](https://github.com/hieplpvip/AsusSMC/issues/93)
- [Perbaiki Tombol Pintas Keyboard / Tombol Fungsional](https://www.insanelymac.com/forum/topic/330440-beginners-guide-fix-keyboard-hot-keys-functional-keys/)
- [PANDUAN: Cara Memperbaiki Hotkey Kecerahan di DSDT](https://www.insanelymac.com/forum/topic/305030-guide-how-to-fix-brightness-hotkeys-in-dsdt/)
- [Menambal DSDT/SSDT untuk kontrol lampu latar LAPTOP](https://www.tonymacx86.com/threads/guide-patching-dsdt-ssdt-for-laptop-backlight-control.152659/)

## Pembaca Kartu

- [Coba RealtekCardReader(+Friend).kext](https://github.com/rafaelmaeuer/Asus-UX32VD-Hackintosh/issues/36)
- [Masalah dengan RTS5139](https://github.com/0xFireWolf/RealtekCardReader/issues/21)
- [Bagaimana cara membuang log yang dihasilkan oleh driver?](https://github.com/0xFireWolf/RealtekCardReader/blob/main/Docs/FAQ.md#how-do-i-dump-the-log-produced-by-the-driver)

**Linux**

- [Jalankan Ubuntu 20.04 dari USB Stick](https://linuxhint.com/run_ubuntu_usb_stick/)
- [OpenCore Multiboot - Dualbooting dengan Linux](https://dortania.github.io/OpenCore-Multiboot/oc/linux.html#dualbooting-with-linux)

## Apa yang ada di dalam folder EFI?
```
├── EFI
│   ├── BOOT
│   │   └── BOOTx64.efi
│   └── OC
│       ├── ACPI
│       │   ├── SSDT-AC0.aml.aml
│       │   ├── SSDT-ALS0.aml
│       │   ├── SSDT-BATT.aml
│       │   ├── SSDT-EC.aml
│       │   ├── SSDT-FN.aml
│       │   ├── SSDT-GPRW.aml
│       │   ├── SSDT-HPET.aml
│       │   ├── SSDT-MEM2.aml
│       │   ├── SSDT-PNLF.aml
│       │   ├── SSDT-PRGEN.aml
│       │   ├── SSDT-PWRB.aml
│       │   └── SSDT-SBUS-MCHC.aml
│       ├── config.plist
│       ├── Drivers
│       │   ├── HfsPlus.efi
│       │   ├── OpenCanopy.efi
│       │   ├── AudioDxe.efi
│       │   ├── ResetNvram.efi
│       │   ├── ToggleSipEntry.efi
│       │   └── OpenRuntime.efi
│       ├── Kexts
│       │   ├── AirPortAtheros40.kext
│       │   ├── ApplePS2SmartTouchPad.kext
│       │   ├── AsusFnKeys.kext
│       │   ├── AppleALC.kext
│       │   ├── Ath3kBT.kext
│       │   ├── Lilu.kext
│       │   ├── CPUFriend.kext
│       │   ├── DisableTurboBoost.kext
│       │   ├── VirtualSMC.kext
│       │   ├── ECEnabler.kext
│       │   ├── FeatureUnlock.kext
│       │   ├── HibernationFixup.kext
│       │   ├── RestrictEvents.kext
│       │   ├── SerialMouse.kext
│       │   ├── ThermalSolution.kext
│       │   ├── TrimForce.kext
│       │   ├── USBToolBox.kext
│       │   ├── VoltageShift.kext
│       │   └── WhateverGreen.kext
│       ├── OpenCore.efi
│       └── Resources
│           ├── Font
│           ├── Image
│           └── Label

```

## Contact me
[![Telegram](https://img.shields.io/badge/Chat_on-Telegram-blue.svg)](https://t.me/Abbas098op)


