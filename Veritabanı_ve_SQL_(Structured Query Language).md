# Veritabanı ve SQL (Structured Query Language)

### Genel Tanım
Veritabanı, bilgilerin düzenli bir şekilde saklandığı tablolardan oluşur. SQL ise veritabanı yönetimi için kullanılan sorgulama dilidir.

### Temel Kavramlar
- **Veritabanı (Database):** Verilerin tablo şeklinde saklandığı yapı.
- **Tablo (Table):** Satır (row) ve sütunlardan (column) oluşur.
- **Satır (Row):** Her bir kaydı temsil eder.
- **Sütun (Column):** Verinin türünü ve alanını belirler.
- **Primary Key:** Tablo içindeki her kaydı benzersiz yapan sütun.
- **Foreign Key:** Farklı tablolar arasında ilişki kuran sütun.
- **Index:** Verilere hızlı erişim sağlamak için kullanılan yapıdır.
- **Null:** Değerin bilinmediğini ifade eder (boşluk ile farklıdır).

### Veri Tipleri
- **VARCHAR(n):** Değişken uzunlukta metin.
- **DECIMAL(p,s):** Ondalıklı sayılar (tam hassasiyet).
- **FLOAT:** Ondalıklı sayılar (yaklaşık değer).
- **DATETIME:** Tarih ve saat bilgisi.
- **BOOLEAN:** Doğru/yanlış değerleri.

### Temel SQL Komutları
- `SELECT * FROM tablo;` → Tablodaki tüm verileri listeler.
- `SELECT sütun1, sütun2 FROM tablo;` → Belirli sütunları seçer.
- `FROM` → Verilerin alınacağı tabloyu belirtir.
- `WHERE koşul` → Koşula uygun kayıtları getirir.
- `ORDER BY sütun ASC/DESC` → Verileri artan (ASC) veya azalan (DESC) şekilde sıralar.
- `LIMIT n` → Sonuç sayısını sınırlar.
- `IN (değerler)` → Birden fazla değere göre filtreleme yapar.

### CRUD İşlemleri (Create, Read, Update, Delete)
- **CREATE (INSERT):** Yeni veri ekler.
    - `INSERT INTO tablo (sütun1, sütun2) VALUES (değer1, değer2);`
- **READ (SELECT):** Veri okur.
    - `SELECT * FROM tablo;`
- **UPDATE:** Mevcut veriyi günceller.
    - `UPDATE tablo SET sütun1 = değer WHERE id = 1;`
- **DELETE:** Veriyi siler.
    - `DELETE FROM tablo WHERE id = 1;`

### İleri SQL Komutları
- `JOIN` → Tablolar arasında ilişki kurar.
    - `INNER JOIN` → İki tabloda eşleşen kayıtları getirir.
    - `LEFT JOIN` → Sol tablodaki tüm kayıtları, sağda eşleşenlerle getirir.
    - `RIGHT JOIN` → Sağ tablodaki tüm kayıtları, solda eşleşenlerle getirir.
- `GROUP BY` → Kayıtları gruplar.
- `HAVING`→ Gruplar üzerinde filtreleme yapar.
- `ISTINCT` → Tekrarlayan verileri kaldırır.
- `ALTER TABLE` → Tabloya sütun ekler, değiştirir veya siler.
- `DROP TABLE` → Tabloyu tamamen siler.

### Veritabanı Yönetim Sistemleri (RDBMS)
- **MySQL / MariaDB** → Açık kaynaklı, yaygın kullanılan sistemler.
- **PostgreSQL** → Güçlü, açık kaynaklı RDBMS.
- **SQLite** → Küçük ve dosya tabanlı veritabanı.
- **MS SQL Server** → Microsoft tarafından geliştirilmiş sistem.

### Araçlar
- **phpMyAdmin / Adminer** → Web tabanlı MySQL yönetim araçları.
- **PgAdmin** → PostgreSQL yönetim aracı.
- **HeidiSQL** → Birden fazla veritabanı sistemini destekleyen araç.