# ping_reboot
Script yang dipakai untuk reboot otomatis openwrt ketika tidak ada koneksi internet, bisa untuk xl protek diskonek per 1GB 

## Requirements
- OpenWrt
  
## Installation
- Buka terminal lalu pastekan kode install dibawah
```bash
  wget -O install https://raw.githubusercontent.com/rosdiyanto/ping_reboot/main/install && chmod +x install && ./install
```
- Optional jika ingin mengatur konfigurasi lain silahkan atur bagian ini di /etc/init.d/ping_reboot.
```bash
  # untuk setting ip/domain yang akan di ping
  IP_ADDRESS="google.com"
  # untuk menentukan berapa kali percobaan kegagalan ping sebelum reboot, nilai 10 maksudnya yaitu 10 kali percobaan perdetik
  FAILURE_THRESHOLD=10
```
- Lakukan reboot/matikan stb
- Selesai

## Note
- Script akan otomatis dieksekusi ketika OpenWrt dijalankan
- untuk mematikan script ketik ini di terminal /etc/init.d/ping_reboot disable
