
# Ağ ve İnternet Kavramları

## Genel Kavramlar

### 🔹 Yazılım ve Web Geliştirme

- **Tema (Theme):** Bir web sitesinin görsel tasarımını belirleyen yapı.
- **Plugin / Eklenti:** Sisteme yeni özellikler ekleyen yazılım parçaları.
- **Şablon (Template):** Önceden hazırlanmış taslak yapılar.
- **Syntax (Sözdizimi):** Programlama dillerinin yazım kuralları.
- **Slide (Slayt):** Sunumlarda kullanılan sayfa yapısı.
- **SPA (Single Page Application):** Tek sayfa uygulaması, içerik dinamik olarak güncellenir.
- **SOC (Separation of Concerns):** Kodun görevlerine göre ayrıştırılması.
- **DRY (Don’t Repeat Yourself):** Kod tekrarından kaçınma prensibi.
- **SOLID:** Nesne yönelimli programlamada sürdürülebilirliği artıran prensipler.

### 🔹 Veri ve Kodlama

- **Encoding (Karakter Kodlama):** Verilerin doğru görüntülenmesi için kullanılan standartlar.
- **UTF-8:** En yaygın kodlama.
- **UTF-8 MB4:** Emoji gibi özel karakterleri destekler.
- **CSV:** Verilerin virgülle ayrıldığı dosya formatı.
- **Null:** Değerin olmadığını veya bilinmediğini belirtir.
- **Raw / Detail / Summary:** Verilerin ham, detaylı ve özet gösterimleri.

---

## 🌐 Ağ ve İnternet Kavramları

### 🔹 Temel Kavramlar

- **DNS (Domain Name System):** Alan adlarını IP adreslerine çevirir.
- **IP (Internet Protocol):** Cihazların ağdaki kimlik adresi.
- **IPv4:** 32-bit adresleme (örn. 192.168.1.1).
- **IPv6:** 128-bit adresleme (örn. 2001:0db8::1).
- **Router (Yönlendirici):** Ağ trafiğini cihazlar arasında yönlendirir.
- **Port:** Uygulamaların iletişim için kullandığı numaralandırılmış kapılar. (22 (SSH), 80 (HTTP), 443 (HTTPS), 3306 (MySQL))
- **TLD (Top-Level Domain):** Alan adlarının uzantıları (.com, .org, .tr).
- **ICANN:** Alan adlarını ve IP adreslerini yöneten uluslararası kuruluş.
- **TTL (Time To Live):** DNS kayıtlarının önbellekte saklanma süresi.

---

### 🔹 İnternet Erişim Akışı

Bir tarayıcıya `www.ornek.com` yazıldığında:

1. **Tarayıcı önbelleği (cache):** Daha önce kaydedilmiş DNS kaydı kontrol edilir.
2. **Hosts dosyası:** Bilgisayarda özel yönlendirme tanımı varsa burada aranır.
3. **Yerel DNS önbelleği:** İşletim sisteminin tuttuğu DNS kayıtları kontrol edilir.
4. **Router DNS:** Modem/router’un DNS önbelleği sorgulanır.
5. **ISS DNS:** İnternet sağlayıcının DNS sunucularına istek gönderilir.
6. **Root DNS:** En üst düzey sunucular, .com gibi uzantının hangi TLD sunucusunda olduğunu döner.
7. **TLD DNS:** İlgili alan adı için yetkili DNS sunucusunu gösterir.
8. **Authoritative DNS:** Son olarak alan adının kesin IP adresini döner.
9. **TCP/HTTPS Bağlantısı:** Tarayıcı IP’ye bağlanır, güvenli bağlantı gerekiyorsa SSL/TLS handshake yapılır.
10. **HTTP(S) İsteği:** Tarayıcı siteyi yükler ve içerikleri (HTML, CSS, JS, resimler) talep eder.

**📌 Özet:** Tarayıcı → Cache → Router → ISS DNS → Root DNS → TLD → Authoritative DNS → IP → Site

---

### 🔹 Ek Ağ Kavramları

- **CDN (Content Delivery Network):** İçeriği dünya genelinde dağıtarak hız ve güvenlik sağlar (örn. Cloudflare).
- **NAT (Network Address Translation):** Yerel ağ cihazlarını tek bir genel IP üzerinden internete çıkarır.
- **Ping:** Bir sunucuya erişilebilirliği test eder.
- **Traceroute:** Bir paketin hedefine giderken geçtiği tüm ağ noktalarını gösterir.
