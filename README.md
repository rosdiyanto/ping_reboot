# ping_reboot
Script yang dipakai untuk reboot otomatis openwrt ketika tidak ada koneksi internet, bisa untuk xl protek diskonek per 1GB 

## Requirements
- OpenWrt
- 
## Installation
- Copy ping_reboot ke directory /etc/init.d/lokasi_file, gunakan filezila/winscp
- Ketik di terminal chmod +x /etc/init.d/ping_reboot
- Ketik di terminal /etc/init.d/ping_reboot enable
- Untuk mengatur konfigurasi lain silahkan atur bagian ini.
```bash
  # untuk setting ip/domain yang akan di ping
  IP_ADDRESS="google.com"
  # untuk menentukan berapa kali percobaan kegagalan ping sebelum reboot, nilai 10 maksudnya yaitu 10 kali percobaan perdetik
  FAILURE_THRESHOLD=10
```

## Note
- Script akan otomatis dieksekusi ketika OpenWrt dijalankan
