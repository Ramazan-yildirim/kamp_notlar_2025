# API ve HTTP

## Genel Tanım
API (Application Programming Interface) yazılımlar arasında iletişim kurmayı sağlayan arayüzdür. HTTP (Hypertext Transfer Protocol) ise istemci (client) ile sunucu (server) arasındaki veri iletişimini sağlar. Modern web geliştirmede genellikle REST API ve JSON formatı kullanılır.

### HTTP Metodları (CRUD ile ilişkili)
- **GET** → Veriyi almak için kullanılır (Read).
- **POST** → Yeni veri göndermek için kullanılır (Create).
- **PUT** → Var olan veriyi tamamen günceller (Update).
- **PATCH** → Var olan veriyi kısmen günceller.
- **DELETE** → Veriyi siler (Delete).

Bu metodlar CRUD işlemleri ile örtüşür:
- Create → POST
- Read → GET
- Update → PUT / PATCH
- Delete → DELETE

### Veri Formatları
- **JSON (JavaScript Object Notation):**
    - Hafif, insan tarafından okunabilir veri formatı.
    - { "ad": "Ali", "yas": 25 } şeklinde yazılır.
    - REST API’lerde en yaygın kullanılan veri formatıdır.
- **XML:** JSON öncesinde kullanılan veri formatı.
- **CSV:** Tablo şeklinde basit veri formatı.

### REST (Representational State Transfer)
- **REST API:** HTTP metodlarını kullanarak istemci-sunucu iletişimi sağlayan standart.
- **Stateless:** Her istek bağımsızdır, önceki istekten bilgi taşımaz.
- **Resource (Kaynak):** API’de genellikle URL ile temsil edilir.
    - Örnek: https://site.com/api/users

### API Test ve Araçları
- **Postman** → API isteklerini test etmek için popüler araç.
- **Insomnia** → Hafif bir API test aracı.
- **Swagger (OpenAPI):** API’leri dokümante etmeye ve test etmeye yarar.

### HTTP Durum Kodları
- **200 OK** → İstek başarılı.
- **201 Created** → Yeni kaynak oluşturuldu.
- **400 Bad Request** → Hatalı istek.
- **401 Unauthorized** → Yetkisiz erişim.
- **403 Forbidden** → Erişim reddedildi.
- **404 Not Found** → Kaynak bulunamadı.
- **500 Internal Server Error** → Sunucu hatası.

### İleri Konular
- **REST vs. SOAP:** REST daha hafif ve JSON tabanlıdır, SOAP ise XML kullanır.
- **GraphQL:** Alternatif bir API yaklaşımı, istemci ihtiyacı kadar veri çeker.
- **WebSocket:** Gerçek zamanlı iletişim sağlar (örn. canlı sohbet, oyunlar).
- **JWT (JSON Web Token):** API güvenliği için kullanılan kimlik doğrulama yöntemi.