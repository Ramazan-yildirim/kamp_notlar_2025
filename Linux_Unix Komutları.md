# Linux / Unix Komutları

### Genel Tanım
Linux, açık kaynaklı bir işletim sistemidir. Yazılım geliştirmede sıkça tercih edilir çünkü güçlü bir terminal (komut satırı) desteği vardır. Terminal üzerinden dosya işlemleri, yazılım yükleme ve sistem yönetimi yapılır.

### Paket Yöneticileri
- **yum:** Red Hat tabanlı (CentOS, Fedora gibi) Linux sistemlerinde yazılım paketlerini kurmaya, güncellemeye ve kaldırmaya yarayan bir paket yöneticisidir.
- **pacman:** Arch Linux ve türevi dağıtımların, sistemi güncel tutmak ve yazılım paketlerini yönetmek için kullandığı komut satırı tabanlı bir paket yöneticisidir.
- **apt:** Debian tabanlı (Ubuntu, Mint gibi) Linux sistemlerinde yazılım kurma, güncelleme ve bağımlılıkları yönetme işlemlerini kolaylaştıran gelişmiş bir paket yönetim aracıdır.

### Paket Yönetimi Komutları
- `sudo apt update` → Paket listelerini günceller.
- `sudo apt upgrade -y` → Mevcut paketleri günceller.
    - `-y` eki, kurulum sırasında sorulan "Evet/Hayır" sorularını otomatik olarak "Evet" olarak yanıtlar.
- `sudo apt install <paket>` → Yeni bir paket yükler.
- `sudo apt remove <paket>` → Paketi kaldırır.
- `sudo apt purge <paket>` → Paketi ve yapılandırma dosyalarını tamamen kaldırır.
- `yum install <paket>` → Red Hat tabanlı sistemlerde paket yüklemek için kullanılır.
- `pacman -S <paket>` → Arch Linux tabanlı sistemlerde paket yüklemek için kullanılır.

### Dosya ve Dizin Yönetimi
- `pwd` → Çalışılan dizinin tam yolunu gösterir.
- `ls` → Bulunduğun dizindeki dosya ve klasörleri listeler.
- `ll` → Dosyaları ayrıntılı listeleme (izinler, boyut, tarih).
- `cd <dizin>` → Belirtilen dizine geçiş yapar.
- `cd ..` → Bir üst dizine çıkar.
- `mkdir <isim>` → Yeni klasör oluşturur.
- `rmdir <isim>` → Boş klasörü siler.
- `rm <dosya>` → Dosya siler.
- `rm -rf <dizin>` → Dizini içindekilerle birlikte siler.
- `cat <dosya adı>` → Bir dosyanın içeriğini terminal ekranında okumanızı sağlar.

### Dosya İşlemleri
- `sudo` → Komutu yönetici (root) yetkisiyle çalıştırır.
- `chmod <izinler> <dosya>` → Dosya izinlerini değiştirir.
- `chown <kullanıcı>:<grup> <dosya>` → Dosya sahipliğini değiştirir.
- `whoami` → Kullanıcı adını gösterir.

### Sistem ve Servis İşlemleri
- `systemctl start <servis>` → Servisi başlatır.
- `systemctl stop <servis>` → Servisi durdurur.
- `systemctl status <servis>` → Servisin durumunu gösterir.
- `ps aux` → Çalışan süreçleri listeler.
- `kill <pid>` → Belirtilen süreç ID’sini (PID) sonlandırır.
- `top` → Anlık sistem süreçlerini ve kaynak kullanımını gösterir.

### İleri Komutlar
- `grep <aranan> <dosya>` → Dosya içinde arama yapar.
- `find <dizin> -name <dosya>` → Belirtilen dosyayı dizinlerde arar.
- `tar -czvf <arsiv.tar.gz> <dizin>` → Dosya/dizin arşivler.
- `unzip <dosya.zip>` → ZIP dosyasını açar.
- `df -h` → Disk kullanımını gösterir.
- `free -m` → Bellek kullanımını gösterir.
- `ifconfig` veya `ip addr` → Ağ bilgilerini listeler.