# Güvenlik ve Hashleme

## Genel Tanım
Yazılım güvenliği, verilerin gizliliğini, bütünlüğünü ve erişilebilirliğini korumayı amaçlar. Bu alanda şifreleme (encryption), kimlik doğrulama (authentication), hashleme ve ağ güvenliği gibi kavramlar ön plandadır.

### Kimlik Doğrulama ve Yetkilendirme
#### JWT (JSON Web Token):
- Kullanıcı oturumlarını yönetmek için kullanılır.
- 3 parçadan oluşur: Header, Payload, Signature.
- Kullanıcının kimliği doğrulandıktan sonra istemciye token verilir ve sonraki isteklerde bu token kullanılır.
- Sunucuda session saklamaya gerek kalmaz, token istemci tarafında tutulur.
#### SSH (Secure Shell):
- Sunucuya güvenli uzaktan bağlantı sağlar.
- **Public Key / Private Key** çifti ile kimlik doğrulama yapılır.
- `ssh-keygen` → Yeni SSH anahtarı oluşturur.
- `cat ~/.ssh/id_rsa.pub` → Public key görüntülenir, GitHub/GitLab gibi platformlara eklenir.

### Hashleme Algoritmaları
#### MD5 (Message Digest 5):
- 32 karakter uzunluğunda hash üretir.
- Günümüzde zayıf sayılır (kırılabilir).
#### SHA (Secure Hash Algorithm):
- SHA-1, SHA-256, SHA-512 gibi türleri vardır.
- MD5’e göre daha güvenlidir.
#### Hash Özellikleri:
- Tek yönlüdür (geri çevrilemez).
- Aynı veri her zaman aynı hash’i üretir.
- Veri değişirse hash tamamen değişir.

### Ağ Güvenliği
- **WireShark:** Ağ trafiğini analiz eden bir araçtır. Paketleri yakalar ve detaylı inceleme imkânı sunar.
- **HTTPS (Hypertext Transfer Protocol Secure):** HTTP’nin TLS/SSL ile şifrelenmiş halidir.
- **Portlar:**
    - 80 → HTTP
    - 443 → HTTPS
    - 3306 → MySQL
    - 22 → SSH

### İleri Güvenlik Kavramları
- **Salt:** Parola hash’lerine eklenen rastgele veri. Aynı parolaların farklı hash değerleri üretmesini sağlar.
- **SSL/TLS Sertifikaları:** Sunucu ile istemci arasında güvenli iletişim sağlar.
- **OAuth:** Kullanıcıların başka bir servis (Google, Facebook vb.) ile kimlik doğrulamasına izin verir.
- **2FA (Two-Factor Authentication):** İki adımlı kimlik doğrulama (örn. SMS + şifre).