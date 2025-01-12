# Coctohug - Kelola lusinan penambangan garpu chia blockchain dari browser web!
- Lokalisasi yang bagus dengan dukungan puluhan bahasa: [English](./wiki_en.md), [العربية](./wiki_ar.md), [Bulgarian](./wiki_bg.md), [Catalan](./wiki_ca.md), [Deutsch](./wiki_de.md), [Español](./wiki_es.md), [زبان فارسی](./wiki_fa.md), [Français](./wiki_fr.md), [Galego](./wiki_gl.md), [Indonesian](./wiki_id.md), [Italiano](./wiki_it.md), [日本語](./wiki_ja.md), [한국어](./wiki_ko.md), [Português do Brasil](./wiki_pt.md), [limba română](./wiki_ro.md), [Русский](./wiki_ru.md), [Serbian](./wiki_sr.md), [Thai](./wiki_th.md), [Tagalog (Filipino)](./wiki_tl.md), [Türkçe](./wiki_tr.md), [Українська](./wiki_uk.md), [Vietnamese](./wiki_vi.md), [简体中文](./wiki_zh-CN.md), [繁體中文](./wiki_zh-TW.md)

Pengaturan Mudah menggunakan [Mulai cepat](https://www.coctohug.xyz/)

*Cari bantuan lebih lanjut di kami [Website](https://www.coctohug.xyz/) / [Github](https://github.com/raingggg/coctohug) / [Discussions](https://github.com/raingggg/coctohug/discussions) / [Discord](https://discord.gg/umfKHm7gVM)*.

# Mulai cepat
  - [Setup Coctohug di OS Linux](#cch-linux)
  - [Siapkan Coctohug di OS Windows](#cch-windows)
  - [Siapkan Coctohug di Mac OS](#cch-macOS)
  

# Pengaturan umum
  - [Kata sandi](#cch-password)
  - [Kunci](#cch-keys)
  - [Pertambangan](#cch-farming)
  - [Pemantauan](#cch-monitoring)
  - [Pemulihan NFT](#cch-nft_recovery)
  - [Blok Ditemukan / Koin Diterima](#cch-blocks_found)
  - [Peringatan Penambangan](#cch-farming_warnings)
  - [Laporan harian](#cch-daily_report)
  - [Laporan mingguan](#cch-weekly_report)
  - [Sinkronisasi Node](#cch-node_sync)
  - [Manajemen Koneksi](#cch-connections_management)
  - [Manajemen Dompet](#cch-wallets_management)
  - [Manajemen Tangan](#cch-hands_management)
  - [Transfer Koin](#cch-transfer_coins)


# Pengaturan lanjutan
  - [Dompet Dingin](#cch-cold_wallet)
  - [Amankan 24 Kata Mnemonik dengan Frasa Sandi](#cch-secure_passphrase)
  - [Garpu Blockchain](#cch-forks)
  - [Mesin penuai](#cch-harvester)
  - [Meningkatkan](#cch-upgrade)

# Praktik terbaik
  - [Bahasa daerah](#cch-local_language)
  - [Persyaratan Perangkat Keras](#cch-hardware_requirements)

<p id="cch-linux">&nbsp;</p>

## Setup Coctohug di OS Linux
- Mempersiapkan <a target='_blank' href='https://www.docker.com/products/docker-desktop'>Docker</a> + <a target='_blank' href='https://docs.docker.com/compose/install/'>Docker-Compose</a> 
- Pergi ke situs <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a>, lalu masukkan semua bidang formulir yang diperlukan dan unduh file komposisi buruh pelabuhan zip yang dihasilkan
- Buka zip folder yang diunduh dan salin ke direktori kerja Anda
- Jalankan semua folder berdasarkan pesanan:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Buka browser dan akses WebUI dengan url <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Catatan 1: Jangan memulai lebih dari 5 garpu blockchain secara bersamaan, karena garpu blockchain chia benar-benar memakan CPU saat sinkronisasi node untuk pertama kalinya
- Catatan 2: Sekitar 1,8G RAM diperlukan untuk setiap garpu blockchain, jadi pilihlah beberapa garpu blockchain berdasarkan memori komputer Anda
- Catatan 3: Jika ada masalah, Anda mungkin perlu menjalankan ulang semua folder berdasarkan pesanan:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Catatan 4: Anda mungkin perlu menambahkan port yang diizinkan dari 12630 hingga 12700 pada pengaturan firewall sistem Anda



<p id="cch-windows">&nbsp;</p>

## Siapkan Coctohug di OS Windows
- Sama dengan [Setup Coctohug di OS Linux](#cch-linux)

<p id="cch-macOS">&nbsp;</p>

## Siapkan Coctohug di Mac OS
- Sama dengan [Setup Coctohug di OS Linux](#cch-linux)

<p id="cch-password">&nbsp;</p>

## Kata sandi
- Anda akan diminta untuk mengatur kata sandi untuk pengaturan aman, ketika Anda pertama kali mengakses WebUI dengan url <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Pengaturan aman meliputi: Dompet Dingin, Transfer Koin, Mulai Ulang Fork Blockchain, Pemanen...

<p id="cch-keys">&nbsp;</p>

## Kunci
- Anda akan diminta untuk memasukkan 24 kata mnemonic, ketika Anda pertama kali mengakses WebUI dengan url - ini terutama untuk tujuan pertanian
- Atau Anda dapat membuat satu kunci yang benar-benar baru - ini terutama untuk tujuan dompet dingin

<p id="cch-farming">&nbsp;</p>

## Pertambangan
- Setelah sinkronisasi simpul selesai, pertanian akan dimulai secara otomatis
- Maka Anda akan dapat memantau status penambangan dengan berbagai cara

![English](../../images/coctohug-summary-en-min.png)

<p id="cch-monitoring">&nbsp;</p>

## Pemantauan
- Tab Ringkasan dapat menunjukkan: Total Koin yang Ditambang, Saldo Akun, Jumlah Plot, Ukuran Plot, Ukuran Netspace, dan Waktu yang Diharapkan untuk Menang
- setiap panel garpu blockchain di tab Ringkasan akan memiliki latar belakang hijau muda jika berfungsi dengan baik, jika tidak maka akan menjadi latar belakang kuning muda
- Anda juga dapat memeriksa detail menggunakan tab lain

<p id="cch-nft_recovery">&nbsp;</p>

## Pemulihan NFT
- Tab Koin yang Diterima memiliki tautan: <a class="nav-link" target="_blank" href="https://alltheblocks.net/nft-recovery">Klaim hadiah NFT 7/8 Anda</a>

<p id="cch-blocks_found">&nbsp;</p>

## Blok Ditemukan / Koin Diterima
- Daftar total blok yang ditemukan
- Daftar total koin yang diterima

![English](../../images/received-coins-min.png)


<p id="cch-farming_warnings">&nbsp;</p>

## Peringatan Penambangan
- Buat daftar kemungkinan masalah jaringan
- Buat daftar kemungkinan masalah signpoint
- Buat daftar kemungkinan masalah pencarian disk
- Buat daftar kemungkinan masalah penurunan jumlah plot

<p id="cch-daily_report">&nbsp;</p>

## Laporan harian
- Ringkaskan Blok yang Ditemukan / Koin yang Diterima berdasarkan hari
- Rangkum Peringatan Penambangan menurut hari

![English](../../images/daily_report-min.png)


<p id="cch-weekly_report">&nbsp;</p>

## Laporan mingguan
- Ringkaskan Blok yang Ditemukan / Koin yang Diterima berdasarkan minggu
- Ringkas Peringatan Penambangan berdasarkan minggu

<p id="cch-node_sync">&nbsp;</p>

## Sinkronisasi Node
- Node akan disinkronkan secara otomatis secara default
- Anda dapat membuka tab Connections atau Blockchains untuk memeriksa status detailnya
- Untuk mempercepat sinkronisasi simpul Anda, [https://alltheblocks.net/](https://alltheblocks.net/) menyediakan daftar node dan file database (klik setiap blockchain dan kemudian Anda dapat menemukannya di bagian kanan atas)

<p id="cch-connections_management">&nbsp;</p>

## Manajemen Koneksi
- Daftar semua koneksi simpul
- Anda dapat menambah/menghapus koneksi di tab Koneksi

![English](../../images/connections-min.png)


<p id="cch-wallets_management">&nbsp;</p>

## Manajemen Dompet
- Daftar status dompet dan saldo akun
- Anda juga dapat mentransfer koin di tab dompet

![English](../../images/wallets-min.png)


<p id="cch-hands_management">&nbsp;</p>

## Manajemen Tangan
- Ini adalah setiap pekerja garpu blockchain
- Anda dapat menghapus satu tangan ketika Anda tidak berencana untuk bertani lagi


<p id="cch-transfer_coins">&nbsp;</p>

## Transfer Koin
- Buka tab dompet dan masukkan kata sandi aman Anda untuk mentransfer koin

<p id="cch-cold_wallet">&nbsp;</p>

## Dompet Dingin
- Buka tab pengaturan dengan kata sandi aman Anda
- Ekspor Akun Cold Wallet
  ```
  1. Siapkan mesin baru (berbeda dengan mesin pertambangan)
  2. Mengunjungi https://www.coctohug.xyz dan klik Mode Dompet untuk membuat folder penyusun buruh pelabuhan
  3. Siapkan folder komposisi buruh pelabuhan [Setup Coctohug di OS Linux]
  4. Pada layar peluncuran WebUI, buat kunci baru kali ini
  5. Tunggu beberapa menit untuk memulai ulang garpu blockchain
  6. Buka setiap folder dan jalankan skrip docker-compose stop && docker-compose up -d
  7. Mengunjungi http://localhost:12630/, dan buka pengaturan - tab dompet dingin untuk mengekspor alamat dompet dingin
  8. Konfirmasikan setiap alamat sudah benar secara manual dengan membandingkan file yang diunduh dengan informasi yang ditampilkan pada tab Tombol
  9. Dapatkan 24 kata mnemonik dengan skrip terminal serupa
    docker exec -it coctohug-flora flora keys show --show-mnemonic-seed
    docker exec -it coctohug-covid covid keys show --show-mnemonic-seed
    docker exec -it coctohug-lucky lucky keys show --show-mnemonic-seed
  ```
- Impor Akun Cold Wallet
  ```
  1. Di mesin penambangan Anda, kunjungi pengaturan - tab dompet dingin
  2. Impor file json dompet dingin yang diunduh sebelumnya (disarankan pada mesin yang berbeda)
  3. Tunggu beberapa menit, dan buka tab dompet untuk melihat apakah alamat dompet dingin diperbarui atau tidak
  4. Catatan 1: kami sarankan untuk membuat cadangan konfigurasi dompet Anda sebelum mengimpor
  5. Catatan 2: Hanya garpu blockchain yang berfungsi yang dapat mengimpor dompet dingin. Silakan periksa apakah ada garpu blockchain yang dihentikan atau tidak sebelum melakukan ini. Tentunya Anda juga dapat mengimpor lagi nanti ketika mereka dimulai kembali
  6. Catatan 3: Jika ada masalah, Anda mungkin perlu menjalankan ulang semua folder berdasarkan pesanan:
    cd coctohug0 && docker-compose up -d
    cd ../coctohug1 && docker-compose up -d
    cd ../coctohug2 && docker-compose up -d
    cd ../coctohug3 && docker-compose up -d
  ```
![English](../../images/cold_wallet-min.png)



<p id="cch-secure_passphrase">&nbsp;</p>

## Amankan 24 Kata Mnemonik dengan Frasa Sandi
- <a target='_blank' href='https://github.com/raingggg/coctohug-passphrase'>coctohug-passphrase</a> dapat digunakan untuk mengamankan 24 kata mnemonik Anda
- Ini mengenkripsi kunci Anda dengan kata sandi hanya Anda yang tahu
- Anda dapat mendekripsinya dengan kata sandi saat menambahkan garpu blockchain baru

<p id="cch-forks">&nbsp;</p>

## Garpu Blockchain
- Periksa coctohug github setiap beberapa hari
- Garpu blockchain baru akan segera didukung
  
<p id="cch-harvester">&nbsp;</p>

## Mesin penuai
- Mengunjungi <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a> dan klik Harvester Mode untuk membuat folder docker-compose
- Mengunjungi <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a> dan klik Izinkan Harvester untuk membangun hubungan antara pengontrol dan pemanen
- Siapkan folder komposisi buruh pelabuhan [Setup Coctohug di OS Linux](#cch-linux)
- Beberapa menit kemudian, Anda akan dapat melihat pemanen di tab tangan WebUI

<p id="cch-upgrade">&nbsp;</p>

## Meningkatkan
- Skrip satu baris
  ```
  docker-compose stop && docker-compose rm -f && docker-compose pull && docker-compose up -d --force-recreate
  ```
- Anda juga dapat menjalankan skrip di atas langkah demi langkah
  ```
  docker-compose stop
  docker-compose rm -f
  docker-compose pull
  docker-compose up -d --force-recreate
  ```
- Jika ada masalah db yang tidak kompatibel, Anda dapat menghapus file database yang ada sebelum menjalankan skrip awal penulisan docker dengan:
  ```
  rm ~/.coctohug-web/db/coctohug.sqlite
  ```

<p id="cch-local_language">&nbsp;</p>

## Bahasa daerah
- Di kanan atas WebUI, pilih bahasa apa pun yang paling Anda sukai
- Anda dapat beralih ke bahasa lain nanti jika Anda mau
  
  
<p id="cch-hardware_requirements">&nbsp;</p>

## Persyaratan Perangkat Keras
- Setelah disinkronkan, Prosesor Intel® Core™ i7 Generasi ke-10 seharusnya cukup untuk mengolah 50+ garpu blockchain
- Namun untuk tahap sinkronisasi simpul awal, itu benar-benar memakan CPU. Jadi kami sarankan untuk menyiapkan 5 garpu blockchain per grup, dan mulai grup demi grup
- Memori yang dibutuhkan sama dengan: jumlah garpu penambangan blockchain, kalikan 1,8G RAM
- Disk normal seharusnya baik untuk 50+ garpu blockchain



# Proyek Sumber Terbuka kami di Github
[webui](https://github.com/raingggg/coctohug-web-docker)

[cactus](https://github.com/raingggg/coctohug-cactus)

[covid](https://github.com/raingggg/coctohug-covid)

[cryptodoge](https://github.com/raingggg/coctohug-cryptodoge)

[ethgreen](https://github.com/raingggg/coctohug-ethgreen)

[flora](https://github.com/raingggg/coctohug-flora)

[greendoge](https://github.com/raingggg/coctohug-greendoge)

[lucky](https://github.com/raingggg/coctohug-lucky) 

[pipscoin](https://github.com/raingggg/coctohug-pipscoin)

[shibgreen](https://github.com/raingggg/coctohug-shibgreen)

[silicoin](https://github.com/raingggg/coctohug-silicoin)

[skynet](https://github.com/raingggg/coctohug-skynet) 

[staicoin](https://github.com/raingggg/coctohug-staicoin)

[stor](https://github.com/raingggg/coctohug-stor)

[tranzact](https://github.com/raingggg/coctohug-tranzact)

[venidium](https://github.com/raingggg/coctohug-venidium)

[btcgreen](https://github.com/raingggg/coctohug-btcgreen)

[hddcoin](https://github.com/raingggg/coctohug-hddcoin)

[maize](https://github.com/raingggg/coctohug-maize)

[flax](https://github.com/raingggg/coctohug-flax)

[aedge](https://github.com/raingggg/coctohug-aedge)

[apple](https://github.com/raingggg/coctohug-apple)

[wheat](https://github.com/raingggg/coctohug-wheat)

[dogechia](https://github.com/raingggg/coctohug-dogechia)

[tad](https://github.com/raingggg/coctohug-tad)

[taco](https://github.com/raingggg/coctohug-taco)

[socks](https://github.com/raingggg/coctohug-socks)

[mogua](https://github.com/raingggg/coctohug-mogua)

[mint](https://github.com/raingggg/coctohug-mint)

[salvia](https://github.com/raingggg/coctohug-salvia)


## Pemberitahuan Merek Dagang
CHIA NETWORK INC, CHIA™, CHIA BLOCKCHAIN™, CHIA PROTOCOL™, CHIALISP™ dan “Logo daun” (termasuk logo daun saja jika mengacu pada atau menunjukkan Chia), adalah merek dagang atau merek dagang terdaftar dari Chia Network, Inc ., sebuah perusahaan Delaware. *Tidak ada afiliasi antara proyek Coctohug ini dan proyek utama Jaringan Chia.*