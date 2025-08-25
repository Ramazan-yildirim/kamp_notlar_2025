
---

# Git ve Versiyon Kontrolü

Git, yazdığın kodların zaman içindeki değişimlerini kaydeden bir versiyon kontrol sistemidir. Projende yaptığın her değişikliği bir "fotoğraf" gibi kaydeder ve istediğin zaman geçmiş bir versiyona geri dönmeni sağlar.

## Kurulum

* **Windows:** Git SCM web sitesinden indirilebilir. Geliştirme ortamı için Laragon veya VS Code gibi araçlarla entegre çalışır.
* **Linux (Debian/Ubuntu):** Terminal üzerinden aşağıdaki komutla kolayca kurulabilir:

  ```bash
  sudo apt install git -y
  ```

## Temel Kavramlar

* **GitHub:** Git ile oluşturulmuş projelerini depolayabileceğin bulut tabanlı bir servistir. Projelerini başkalarıyla paylaşmanı, takım olarak çalışmanı ve açık kaynaklı projelere katkıda bulunmanı sağlar. Kısacası, GitHub bir Git servisidir.
* **GitLab:** GitHub'ın popüler bir alternatifidir. Özellikle kendi sunucularına kurarak daha güvenli ve özel bir yapı (self-hosted) kurmak isteyen şirketler tarafından tercih edilir.

## Sık Kullanılan Git Komutları

* `git log`: Projedeki tüm "commit" yani kayıt edilmiş değişiklik geçmişini listeler.

  * `git log --oneline`: Commit geçmişini daha okunaklı, tek satırlık bir formatta gösterir.
* `git checkout [dal_adi/commit_hash]`: Projeni belirli bir dala (branch) veya geçmiş bir commit'e geri döndürmeni sağlar.

  * `git checkout main`: Genellikle ana dala (en güncel versiyona) dönmek için kullanılır.
* `git remote add [isim] [url]`: Lokaldeki projenize GitHub gibi bir uzak sunucu adresi eklemenizi sağlar. Genellikle origin ismi kullanılır.
* `git status`: Çalışma alanındaki değişiklikleri ve takip edilen dosyaların durumunu gösterir.
* `git diff`: Yapılan değişiklikleri satır satır karşılaştırarak gösterir.

---

# Temel Linux Komutları

Linux tabanlı sistemlerde (veya Windows'ta WSL ile) terminal, en güçlü yardımcınızdır.

## Paket Yönetimi (Debian/Ubuntu)

* `sudo apt update`: Paket listesini günceller.
* `sudo apt upgrade`: Yüklü paketleri en son sürümlerine yükseltir.
* `sudo apt update && sudo apt upgrade`: İlk komut (update) hatasız çalışırsa, ikinci komutu (upgrade) otomatik olarak çalıştırır.
* `sudo apt remove [paket_adi]`: Bir paketi kaldırır.
* `sudo apt purge [paket_adi]`: Bir paketi konfigürasyon dosyalarıyla birlikte tamamen kaldırır.

**Not:** Diğer dağıtımlarda yum (CentOS/RHEL) veya pacman (Arch Linux) gibi farklı paket yöneticileri kullanılır.

## Dizin ve Dosya Yönetimi

* `pwd`: "Print Working Directory" - o an terminalde hangi klasörün içinde olduğunu gösterir.
* `ls`: Bulunduğun dizindeki dosya ve klasörleri listeler.
* `ll`: `ls -l` komutunun kısaltmasıdır ve dosyaları daha detaylı (izinler, boyut, tarih vb.) bir şekilde listeler.
* `ctrl + l`: Terminal ekranını temizler.
* `cd [klasör]`: Belirtilen klasöre geçiş yapar.
* `mkdir [klasör]`: Yeni klasör oluşturur.
* `rm [dosya]`: Dosya siler.

---

# Web Geliştirme ve Sunucu Kavramları

## Node.js ve npm

* **JavaScript'in Yükselişi:** JavaScript, eskiden sadece web tarayıcılarında çalışan bir dildi. 2009'da Ryan Dahl, JavaScript'i V8 motoruyla terminalde çalıştırmayı başardı ve böylece Node.js doğdu.Node.js, JavaScript’i tarayıcı dışında da çalıştırabilmeni sağlayan bir çalışma ortamıdır. Bu sayede JavaScript ile sunucu taraflı uygulamalar (backend) geliştirmek mümkün hale geldi.
* **Asenkron (Non-Blocking) Yapı:** Node.js'in en önemli özelliklerinden biri asenkron çalışmasıdır. Bir işlem bitmeden diğerine geçebilir. Bu, özellikle aynı anda çok sayıda isteğe cevap vermesi gereken web sunucuları için onu çok verimli kılar.
* **npm (Node Package Manager):** Node.js ile birlikte gelen paket yöneticisidir. Başkalarının yazdığı hazır kod kütüphanelerini (paketleri) projene kolayca dahil etmeni sağlar.

## Web Sunucuları ve Portlar

* **Portlar:** Bilgisayarında çalışan her internet hizmeti, iletişim kurmak için bir "kapı" yani port kullanır.Bir bilgisayarda toplam 65,535 adet port bulunur. İlk 1024 port genellikle standart servisler için rezerve edilmiştir.
* **Apache:** Dünyanın en popüler web sunucularından biridir. Genellikle HTTP istekleri için varsayılan olarak 80 numaralı portu dinler. Tarayıcına `http://127.0.0.1` veya `http://localhost` yazdığında, 80 portu tetiklenir ve Apache sana web sayfasını sunar. PHP ile olan uyumu sayesinde "mükemmel ikili" olarak anılırlar.
* **Nginx:** Apache'ye benzer, yüksek performanslı bir diğer web sunucusudur. Özellikle yüksek trafikli sitelerde tercih edilir.
* **IIS (.NET):** Microsoft'un Windows sunucular için geliştirdiği web sunucusudur. Genellikle .NET uygulamalarını çalıştırmak için kullanılır.
* **Daemon (Servis):** Apache, MySQL gibi programlar arka planda sürekli çalışan uygulamalardır.

## Laragon ve XAMPP

* Bu programlar, bilgisayarında web geliştirme için gerekli olan Apache, MySQL, PHP gibi servisleri tek bir pakette kurup yönetmeni sağlayan araçlardır.
* **Laragon’un avantajı:** Composer gibi modern araçları içerir.
* **İpucu:** Bilgisayarı kapatmadan önce servisleri durdurmak veri kaybını önler.

---

# Veritabanı Temelleri

Veritabanları, verileri organize ve yapısal bir şekilde saklayan sistemlerdir. Veriler genellikle tablolar içinde tutulur.

## MySQL

* Dünyanın en yaygın kullanılan ilişkisel veritabanı yönetim sistemidir (RDBMS).
* Varsayılan olarak 3306 portunda çalışır.
* **Root Kullanıcısı:** MySQL ilk kurulduğunda en yetkili kullanıcı root olarak oluşturulur. Yerel (local) geliştirme ortamlarında genellikle şifresi boş olur veya root olarak ayarlanır.

## MariaDB

* MySQL'in orijinal geliştiricileri tarafından oluşturulmuş, MySQL ile tamamen uyumlu bir alternatiftir.

## Temel Veri Türleri

* `VARCHAR`: Değişken uzunlukta metin verileri için (örn: kullanıcı adı, başlık).
* `DECIMAL`, `FLOAT`: Ondalıklı sayılar için (örn: fiyat, oran).
* `DATETIME`: Tarih ve saat bilgisi için.
* `INT`: Tam sayılar için.
* `BOOLEAN`: Mantıksal değerler (TRUE/FALSE).
* `TEXT`: Çok uzun metinler için (örn: açıklama, içerik).

---

# Faydalı Araçlar ve Kaynaklar

## Markdown (.md)

Markdown, yazılarına başlık, liste, kod bloğu gibi formatlar eklemeni sağlayan basit bir işaretleme dilidir. GitHub'da README.md dosyaları bu formatla yazılır.

**Kullanım Alanları:**

* Yazılım projelerinde README dosyaları hazırlamak.
* Blog yazıları veya dokümantasyon oluşturmak.
* Not alma uygulamalarında (Obsidian, Joplin vb.).
* Diyagram ve tablo hazırlamak.

**Örnekler:**

* **Kod Bloğu:**

  ```bash
  sudo apt update && sudo apt upgrade
  ```
* **Listeleme:**

  * Öğeler
  * Alt öğeler
* **Tablo:**

  | ID | İsim | Yaş |
  | -- | ---- | --- |
  | 1  | Ali  | 25  |

## StackEdit.io

Tarayıcı üzerinden çalışan, yazdığın Markdown metninin anlık önizlemesini gösteren ve farklı formatlarda çıktı almanı sağlayan kullanışlı bir editördür.

## Mermaid

Markdown içerisinde diyagram ve akış şemaları oluşturmanı sağlayan bir kütüphanedir.

## WordPress Kaynakları

* **ThemeForest:** Profesyonel WordPress temaları bulabileceğin bir pazar yeridir.
* **WooCommerce:** WordPress'i bir e-ticaret sitesine dönüştüren popüler eklentidir.

## WakaTime

Kod editörlerinde ne kadar süre harcadığını ve hangi dillerde çalıştığını takip eden bir eklentidir.

---
