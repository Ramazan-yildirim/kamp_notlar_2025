# Frameworkler

## Genel Tanım
Framework, yazılım geliştirmeyi kolaylaştıran, belirli kurallar ve hazır bileşenler sunan yapılardır. Kod tekrarını azaltır, düzenli bir mimari sağlar.

### Backend Frameworkleri
#### Laravel (PHP)
- PHP için en popüler web framework’üdür.
- MVC (Model-View-Controller) mimarisini kullanır.
- **Migration:** Veritabanı tablolarını yönetmek için kullanılır.
- **Model:** Tabloların temsilcisidir, veritabanı işlemlerini kolaylaştırır.
- **Controller:** İş mantığını yönetir, model ve view arasında köprü kurar.
- **Blade Template Engine:** Görsel arayüz (view) kısmında kullanılır.
- **php artisan** → Laravel’in komut satırı aracıdır.
    - `php artisan make:migration create_users_table`→ Yeni tablo migration’ı oluşturur.
    - `php artisan route:list` → Tüm route’ları listeler.

#### Node.js (JavaScript runtime)
- JavaScript’i tarayıcı dışında çalıştırmaya yarar.
- 2012’den sonra yaygınlaştı.
- Sunucu tarafında yüksek performans sağlar.
- **npm (Node Package Manager):** Node için paket yöneticisi.
- **nvm (Node Version Manager):** Node sürümlerini yönetir.

### Frontend Frameworkleri
#### Vue.js
- Kullanıcı arayüzü geliştirmek için hafif ve esnek bir framework.
- Component tabanlıdır.
- Temel dosyalar: `App.vue`, `main.js`.
- **CLI ile başlatma:**
    - `npm create vue@latest`→ Yeni Vue projesi oluşturur.
    - `npm run dev` → Projeyi geliştirici modunda çalıştırır.
- **Vue Router:** Sayfa yönlendirmeleri için.
- **Pinia:** State management (veri yönetimi) için.

#### Quasar (Vue tabanlı)
- Vue üzerine inşa edilmiş gelişmiş bir framework.
- Hem web hem de mobil uygulama geliştirmeye uygundur.
- **CLI ile kurulum:**
    - `npm i -g @quasar/cli`
    - `pm init quasar@latest`
- Hazır component kütüphanesi sunar (Button, Dialog, Notify vb.).
- **quasar.config.js** → Proje ayarlarının yapıldığı dosya.

#### Alpine.js
- Vue.js’nin daha hafif ve basit bir alternatifi.
- Küçük etkileşimler eklemek için idealdir.

### Yazılım Prensipleri (Frameworklerle İlgili)
- **SOLID Prensipleri:**Temiz ve sürdürülebilir kod yazmayı sağlar.
- **DRY (Don’t Repeat Yourself):** Kod tekrarından kaçınılmalı.
- **SOC (Separation of Concerns):** Her modülün kendi görevine odaklanması gerekir.

### Diğer Araçlar
- **Composer (PHP):** PHP paket yöneticisi.
- **XAMPP / Laragon:** Geliştirme ortamları (Apache, PHP, MySQL içerir).
- **Docker:** Uygulamaları izole edilmiş ortamlarda çalıştırır.