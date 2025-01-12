# Coctohug - Bir web tarayıcısından düzinelerce chia blockchain çatal madenciliğini yönetin!
- Düzinelerce dil desteğiyle güzel yerelleştirme: [English](./wiki_en.md), [العربية](./wiki_ar.md), [Bulgarian](./wiki_bg.md), [Catalan](./wiki_ca.md), [Deutsch](./wiki_de.md), [Español](./wiki_es.md), [زبان فارسی](./wiki_fa.md), [Français](./wiki_fr.md), [Galego](./wiki_gl.md), [Indonesian](./wiki_id.md), [Italiano](./wiki_it.md), [日本語](./wiki_ja.md), [한국어](./wiki_ko.md), [Português do Brasil](./wiki_pt.md), [limba română](./wiki_ro.md), [Русский](./wiki_ru.md), [Serbian](./wiki_sr.md), [Thai](./wiki_th.md), [Tagalog (Filipino)](./wiki_tl.md), [Türkçe](./wiki_tr.md), [Українська](./wiki_uk.md), [Vietnamese](./wiki_vi.md), [简体中文](./wiki_zh-CN.md), [繁體中文](./wiki_zh-TW.md)

Kullanımı Kolay Kurulum [Hızlı başlangıç](https://www.coctohug.xyz/)

*Bizimle ilgili daha fazla yardım isteyin [Website](https://www.coctohug.xyz/) / [Github](https://github.com/raingggg/coctohug) / [Discussions](https://github.com/raingggg/coctohug/discussions) / [Discord](https://discord.gg/umfKHm7gVM)*.

# Hızlı başlangıç
  - [Linux işletim sisteminde Coctohug&#39;u kurun](#cch-linux)
  - [Windows işletim sisteminde Coctohug&#39;u kurun](#cch-windows)
  - [Mac OS&#39;de Coctohug&#39;u Kurma](#cch-macOS)
  

# Genel Ayarlar
  - [Parola](#cch-password)
  - [Anahtarlar](#cch-keys)
  - [madencilik](#cch-farming)
  - [izleme](#cch-monitoring)
  - [NFT Kurtarma](#cch-nft_recovery)
  - [Bulunan Bloklar / Alınan Paralar](#cch-blocks_found)
  - [Madencilik Uyarıları](#cch-farming_warnings)
  - [Günlük rapor](#cch-daily_report)
  - [Haftalık rapor](#cch-weekly_report)
  - [Düğüm Senkronizasyonu](#cch-node_sync)
  - [Bağlantı Yönetimi](#cch-connections_management)
  - [Cüzdan Yönetimi](#cch-wallets_management)
  - [El Yönetimi](#cch-hands_management)
  - [Para Transferi](#cch-transfer_coins)


# Gelişmiş Ayarlar
  - [Soğuk Cüzdan](#cch-cold_wallet)
  - [Güvenli Parolalı 24 Anımsatıcı Söz](#cch-secure_passphrase)
  - [Blockchain Çatalları](#cch-forks)
  - [biçerdöver](#cch-harvester)
  - [Güncelleme](#cch-upgrade)

# En İyi Uygulamalar
  - [Yerel dil](#cch-local_language)
  - [Donanım Gereksinimleri](#cch-hardware_requirements)

<p id="cch-linux">&nbsp;</p>

## Linux işletim sisteminde Coctohug&#39;u kurun
- Kurmak <a target='_blank' href='https://www.docker.com/products/docker-desktop'>Docker</a> + <a target='_blank' href='https://docs.docker.com/compose/install/'>Docker-Compose</a> 
- siteye git <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a>, ardından gerekli tüm form alanlarını girin ve oluşturulan sıkıştırılmış docker-compose dosyalarını indirin
- İndirilen klasörleri açın ve çalışma dizininize kopyalayın
- Tüm klasörleri sırayla çalıştırın:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Tarayıcıyı açın ve url ile WebUI&#39;ye erişin <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Not 1: Chia blok zinciri çatalları, düğüm senkronizasyonu ilk kez yapıldığında gerçekten CPU yediğinden, aynı anda 5&#39;ten fazla blok zinciri çatalı başlatmayın.
- Not 2: Her blok zinciri çatalı için yaklaşık 1.8G RAM gereklidir, bu nedenle bilgisayar belleğinize göre bazı blok zincir çatalları seçin
- Not 3: Herhangi bir sorun varsa, tüm klasörleri sırayla yeniden çalıştırmanız gerekebilir:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Not 4: Sistem güvenlik duvarı ayarlarınıza 12630&#39;dan 12700&#39;e kadar izin verilen bağlantı noktaları eklemeniz gerekebilir.



<p id="cch-windows">&nbsp;</p>

## Windows işletim sisteminde Coctohug&#39;u kurun
- İle aynı [Linux işletim sisteminde Coctohug&#39;u kurun](#cch-linux)

<p id="cch-macOS">&nbsp;</p>

## Mac OS&#39;de Coctohug&#39;u Kurma
- İle aynı [Linux işletim sisteminde Coctohug&#39;u kurun](#cch-linux)

<p id="cch-password">&nbsp;</p>

## Parola
- URL ile WebUI&#39;ye ilk kez eriştiğinizde, güvenli ayarlar için bir parola belirlemeniz istenecektir. <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Güvenli ayarlar şunları içerir: Cold Wallet, Coin Transfer, Restart Blockchain Forks, Harvester...

<p id="cch-keys">&nbsp;</p>

## Anahtarlar
- URL ile WebUI&#39;ye ilk kez eriştiğinizde, 24 anımsatıcı kelimeyi girmeniz istenecektir - bu esas olarak çiftçilik amaçlıdır
- Veya tamamen yeni bir anahtar oluşturabilirsiniz - bu esas olarak soğuk cüzdan amaçlıdır

<p id="cch-farming">&nbsp;</p>

## madencilik
- Düğüm senkronizasyonu yapıldığında, çiftçilik otomatik olarak başlamalıdır
- Ardından madencilik durumunu çeşitli yollarla izleyebileceksiniz.

![English](../../images/coctohug-summary-en-min.png)

<p id="cch-monitoring">&nbsp;</p>

## izleme
- Özet sekmesi şunları gösterebilir: Toplam Maden Paraları, Hesap Bakiyesi, Arsa Sayısı, Arsa Boyutu, Netspace Boyutu ve Beklenen Kazanma Süresi
- Özet sekmesindeki her blok zinciri çatal paneli, düzgün çalışıyorsa açık yeşil bir arka plana sahip olacaktır, aksi takdirde açık sarı arka plana sahip olacaktır.
- Detayları diğer sekmeleri kullanarak da inceleyebilirsiniz.

<p id="cch-nft_recovery">&nbsp;</p>

## NFT Kurtarma
- Alınan Paralar sekmesinde bir bağlantı bulunur: <a class="nav-link" target="_blank" href="https://alltheblocks.net/nft-recovery">NFT 7/8 ödüllerinizi talep edin</a>

<p id="cch-blocks_found">&nbsp;</p>

## Bulunan Bloklar / Alınan Paralar
- Bulunan toplam blokları listele
- Alınan toplam paraları listele

![English](../../images/received-coins-min.png)


<p id="cch-farming_warnings">&nbsp;</p>

## Madencilik Uyarıları
- Olası ağ sorununu listeleyin
- Olası işaret noktası sorununu listeleyin
- Olası disk arama sorununu listeleyin
- Olası arsa sayısı azalan sorunu listeleyin

<p id="cch-daily_report">&nbsp;</p>

## Günlük rapor
- Bulunan Blokları / Güne Göre Alınan Paraları Özetle
- Madencilik Uyarılarını güne göre özetleyin

![English](../../images/daily_report-min.png)


<p id="cch-weekly_report">&nbsp;</p>

## Haftalık rapor
- Bulunan Blokları / Haftaya Göre Alınan Paraları Özetle
- Madencilik Uyarılarını Haftaya Göre Özetleyin

<p id="cch-node_sync">&nbsp;</p>

## Düğüm Senkronizasyonu
- Düğüm varsayılan olarak otomatik olarak eşitlenir
- Ayrıntılı durumu incelemek için Bağlantılar veya Blokajlar sekmesine gidebilirsiniz.
- Düğüm senkronizasyonunuzu hızlandırmak için, [https://alltheblocks.net/](https://alltheblocks.net/) düğüm listesi ve veritabanı dosyası sağlar (her blok zincirine tıklayın ve ardından bunları sağ üst bölümde bulabilirsiniz)

<p id="cch-connections_management">&nbsp;</p>

## Bağlantı Yönetimi
- Tüm düğüm bağlantılarını listele
- Bağlantılar sekmesinde bağlantı ekleyebilir/kaldırabilirsiniz

![English](../../images/connections-min.png)


<p id="cch-wallets_management">&nbsp;</p>

## Cüzdan Yönetimi
- Cüzdan durumunu ve hesap bakiyesini listeleyin
- Paraları cüzdan sekmesinden de aktarabilirsiniz.

![English](../../images/wallets-min.png)


<p id="cch-hands_management">&nbsp;</p>

## El Yönetimi
- Bu, her bir blockchain çatal işçisi
- Artık çiftlik yapmayı planlamadığınızda bir elinizi kaldırabilirsiniz.


<p id="cch-transfer_coins">&nbsp;</p>

## Para Transferi
- Cüzdan sekmesine gidin ve madeni paraları aktarmak için güvenli şifrenizi girin

<p id="cch-cold_wallet">&nbsp;</p>

## Soğuk Cüzdan
- Güvenli şifrenizle ayarlar sekmesine gidin
- Soğuk Cüzdan Hesabını Dışa Aktar
  ```
  1. Yeni bir makine hazırlayın (madencilik makinesinden farklı)
  2. Ziyaret https://www.coctohug.xyz ve docker-compose klasörleri oluşturmak için Cüzdan Modu&#39;nu tıklayın
  3. Docker-compose klasörlerini kurun [Linux işletim sisteminde Coctohug&#39;u kurun]
  4. WebUI başlatma ekranında bu sefer yeni bir anahtar oluşturun
  5. Blockchain çatallarının yeniden başlatılması için birkaç dakika bekleyin
  6. Her klasöre gidin ve komut dosyasını yürütün docker-compose stop && docker-compose up -d
  7. Ziyaret http://localhost:12630/, ve soğuk cüzdan adreslerini dışa aktarmak için ayarlar - soğuk cüzdan sekmesine gidin
  8. İndirilen dosyayı Anahtarlar sekmesinde gösterilen bilgilerle karşılaştırarak her adresin manuel olarak doğru olduğunu onaylayın.
  9. Benzer terminal komut dosyasıyla 24 anımsatıcı kelime alın
    docker exec -it coctohug-flora flora keys show --show-mnemonic-seed
    docker exec -it coctohug-covid covid keys show --show-mnemonic-seed
    docker exec -it coctohug-lucky lucky keys show --show-mnemonic-seed
  ```
- Soğuk Cüzdan Hesabını İçe Aktar
  ```
  1. Madencilik makinenizde ayarlar - soğuk cüzdan sekmesini ziyaret edin
  2. Daha önce indirilen soğuk cüzdanı (farklı makinelerde önerilir) json dosyasını içe aktarın
  3. Birkaç dakika bekleyin ve soğuk cüzdan adresinin güncellenip güncellenmediğini görmek için cüzdan sekmesine gidin.
  4. Not 1: İçe aktarmadan önce cüzdan yapılandırmalarınızı yedeklemenizi öneririz.
  5. Not 2: Yalnızca çalışan blok zinciri çatalları, soğuk cüzdanı içe aktarabilir. Lütfen bunu yapmadan önce blok zinciri çatallarının durup durmadığını kontrol edin. Elbette daha sonra yeniden başlatıldıklarında tekrar içe aktarabilirsiniz.
  6. Not 3: Herhangi bir sorun varsa, tüm klasörleri sırayla yeniden çalıştırmanız gerekebilir:
    cd coctohug0 && docker-compose up -d
    cd ../coctohug1 && docker-compose up -d
    cd ../coctohug2 && docker-compose up -d
    cd ../coctohug3 && docker-compose up -d
  ```
![English](../../images/cold_wallet-min.png)



<p id="cch-secure_passphrase">&nbsp;</p>

## Güvenli Parolalı 24 Anımsatıcı Söz
- <a target='_blank' href='https://github.com/raingggg/coctohug-passphrase'>coctohug-passphrase</a> 24 anımsatıcı kelimenizi güvenceye almak için kullanılabilir
- Anahtarlarınızı yalnızca sizin bildiğiniz bir parola ile şifreler
- Yeni blockchain çatalları eklerken şifre ile şifresini çözebilirsiniz.

<p id="cch-forks">&nbsp;</p>

## Blockchain Çatalları
- Coctohug github&#39;ı birkaç günde bir kontrol edin
- Yeni blockchain çatalları çok yakında desteklenecek
  
<p id="cch-harvester">&nbsp;</p>

## biçerdöver
- Ziyaret <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a> ve docker-compose klasörleri oluşturmak için Harvester Mode&#39;a tıklayın
- Ziyaret <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a> ve biçerdöver ile kontrolör arasındaki bağlantıyı kurmasına izin ver&#39;i tıklayın.
- Docker-compose klasörlerini kurun [Linux işletim sisteminde Coctohug&#39;u kurun](#cch-linux)
- Birkaç dakika sonra, hasat makinesini WebUI eller sekmesinde görebileceksiniz.

<p id="cch-upgrade">&nbsp;</p>

## Güncelleme
- Tek satırlık komut dosyası
  ```
  docker-compose stop && docker-compose rm -f && docker-compose pull && docker-compose up -d --force-recreate
  ```
- Ayrıca yukarıdaki komut dosyalarını adım adım çalıştırabilirsiniz.
  ```
  docker-compose stop
  docker-compose rm -f
  docker-compose pull
  docker-compose up -d --force-recreate
  ```
- Uyumsuz db sorunu olması durumunda, docker-compose başlatma komut dosyasını çalıştırmadan önce mevcut veritabanı dosyasını şu şekilde kaldırabilirsiniz:
  ```
  rm ~/.coctohug-web/db/coctohug.sqlite
  ```

<p id="cch-local_language">&nbsp;</p>

## Yerel dil
- WebUI&#39;nin sağ üst köşesinde, en çok beğendiğiniz dili seçin
- Dilerseniz daha sonra başka dillere geçebilirsiniz.
  
  
<p id="cch-hardware_requirements">&nbsp;</p>

## Donanım Gereksinimleri
- Senkronize edildikten sonra, 10. Nesil Intel® Core™ i7 İşlemciler, 50&#39;den fazla blok zinciri çatalı oluşturmak için yeterli olacaktır.
- Ancak ilk düğüm senkronizasyon aşaması için gerçekten CPU yiyor. Bu nedenle, grup başına 5 blok zinciri çatalı kurmanızı ve gruplara göre grup başlatmanızı öneririz.
- Gerekli bellek şuna eşittir: madencilik blok zinciri çatallarının sayısı 1.8G RAM ile çarpılır
- 50&#39;den fazla blockchain çatalı için normal disk iyi olmalıdır



# Github Üzerindeki Açık Kaynak Projelerimiz
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


## Ticari Marka Bildirimi
CHIA NETWORK INC, CHIA™, CHIA BLACKCHAIN™, CHIA PROTOCOL™, CHIALISP™ ve “yaprak Logosu” (Chia&#39;ya atıfta bulunduğunda veya Chia&#39;yı gösterdiğinde yalnızca yaprak logosu dahil), Chia Network, Inc&#39;in ticari markaları veya tescilli ticari markalarıdır. ., bir Delaware şirketi. *Bu Coctohug projesi ile ana Chia Network projesi arasında herhangi bir bağlantı yoktur.*