# setting-mikrotik
1. Koneksi Router

Menghubungkan router Mikrotik ke komputer, dengan cara menghubungkan kabel Ethernet dari port LAN Mikrotik ke port Ethernet pada komputer. 

2. Unduh dan Instal Aplikasi Winbox

Mengunduh dari situs resmi Mikrotik dan instal aplikasi Winbox di komputer.

3. Konfigurasi Awal

Setelah itu buka aplikasi tersebut dan cari Mikrotik yang terhubung ke komputer. Klik pada Mikrotik yang terdeteksi dan klik tombol 'Connect' untuk menghubungkan ke Mikrotik.

4. Setting Konfigurasi IP Address

Konfigurasi IP Address diperlukan untuk mengatur alamat IP pada perangkat Mikrotik. Untuk melakukan ini, buka jendela 'Bridge' pada aplikasi Winbox dan klik tab 'Bridge'. Tekan tombol (+) untuk membuka dialog baru dan masukkan nama jembatan lokal. Klik OK untuk menyimpan pengaturan.
Selanjutnya, klik tab 'Ports' dan klik tombol (+) untuk menambahkan antarmuka Ether2. Pilih 'Lokal' di bagian Bridge dan tekan OK untuk menyimpan pengaturan. Terakhir, buka IP dan klik Addresses. Masukkan alamat IP (misalnya, 192.168.88.1/24) dan pilih 'Local' di bagian 'Interface'. Tekan OK untuk menyimpan pengaturan.

5. Setting Konfigurasi DHCP Server

Konfigurasi DHCP Server diperlukan untuk mengatur alamat IP secara otomatis pada perangkat yang terhubung ke jaringan Mikrotik. Untuk melakukan ini, buka IP pada aplikasi Winbox dan klik 'DHCP Server'. Tekan tombol DHCP Set up untuk membuka jendela baru. Klik 'Local' pada 'DHCP Server Interface' dan klik 'Next' untuk melanjutkan proses konfigurasi.

6. Setting Konfigurasi Jaringan Internet

Pengaturan konfigurasi jaringan internet diperlukan agar perangkat dapat mengakses internet. Buka kategori segmen PPP pada aplikasi Winbox dan klik tab Interfaces. Klik tombol (+) untuk menambahkan 'Klien PPPoE'. Pilih 'Ether 1' di bagian 'Interfce' dan klik OK untuk menyimpan pengaturan.

7. Verifikasi Konektivitas

Setelah semua konfigurasi selesai, verifikasi konektivitas IP dengan melakukan Ping ke Alamat IP yang diketahui server Google. Jika ping berhasil, berarti konfigurasi telah berhasil dan kita dapat mengakses internet dari perangkat Mikrotik.
