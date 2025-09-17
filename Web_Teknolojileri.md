# Web Teknolojileri

## Genel Tanım
Web geliştirme, kullanıcıların tarayıcı üzerinden eriştiği uygulamaların ve sitelerin oluşturulmasıdır. Bu süreçte frontend (kullanıcı arayüzü), backend (sunucu tarafı) ve veritabanı katmanları vardır.

### Temel Teknolojiler
#### HTML (Hypertext Markup Language):
- Web sayfalarının iskeletini oluşturur.
- Yapısal elementler (`<head>`, `<body>`, `<title>`, `<h1>`, `<p>` vb.) içerir.
#### CSS (Cascading Style Sheets):
- HTML içeriklerine stil verir.
- Renk, yazı tipi, düzen gibi görsel özellikleri belirler.
- `style` etiketi içinde veya harici `.css` dosyalarında kullanılır.
#### JavaScript (JS):
- Web sayfalarına etkileşim katar.
- DOM üzerinde değişiklik yapabilir.
- `fetch` ile API’lerden veri alabilir.
#### TypeScript (TS):
- JavaScript’in tip güvenliği eklenmiş sürümüdür.
- Büyük projelerde hata riskini azaltır.

### Veri Gönderme ve İletişim
#### JSON (JavaScript Object Notation):
- `{ "ad": "Ahmet", "yas": 25 }` formatında yazılır.
- API’ler ile veri gönderme/çekmede standarttır.
#### REST API:
- JSON formatında veri iletişimi sağlar.
- CRUD işlemlerini HTTP metodları ile gerçekleştirir.
#### AJAX (Asynchronous JavaScript and XML):
- Sayfayı yenilemeden veri almayı/göndermeyi sağlar.
- Günümüzde çoğunlukla fetch ve modern API’ler kullanılır.
#### WebSocket:
- Gerçek zamanlı iletişim sağlar.
- Canlı sohbet, oyunlar, finans uygulamaları için uygundur.

### Uygulama Türleri
#### SPA (Single Page Application):
- Sayfa sadece bir kez yüklenir, içerik dinamik olarak güncellenir.
- Vue, React, Angular gibi frameworklerle geliştirilir.
#### SSR (Server-Side Rendering):
- HTML içerikleri sunucuda hazırlanıp istemciye gönderilir.
- SEO ve hız açısından avantajlıdır.

### Web Sunucuları
- **Apache:** HTML içeriğini dışarıya sunar.
- **Nginx:** Yüksek performanslı, ters proxy destekli web sunucusu.
- **IIS (Internet Information Services):** Microsoft’un web sunucusu.
- **Localhost (127.0.0.1):** Geliştirme ortamında kullanılan yerel adres.
#### Portlar:
- 80 → HTTP
- 443 → HTTPS
- 3306 → MySQL
- 8080 → Geliştirme/test sunucuları

### İleri Konular
#### Markdown (.md):
- Basit işaretleme dili.
- `#` başlık, `*` liste, `---` yatay çizgi.
- Slayt, dokümantasyon, README dosyalarında sık kullanılır.
#### Mermaid.js:
- Markdown içinde diyagram ve şema oluşturmaya yarar.
#### WordPress:
- PHP tabanlı içerik yönetim sistemi (CMS).
- Eklentiler ve temalarla özelleştirilebilir.
- **WooCommerce:** WordPress için e-ticaret eklentisi.
- **ThemeForest:** Hazır WordPress temalarının satıldığı platform.