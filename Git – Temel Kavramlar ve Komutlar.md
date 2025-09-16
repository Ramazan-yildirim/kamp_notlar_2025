# Git – Temel Kavramlar ve Komutlar

### Genel Tanım

Git, bir versiyon kontrol sistemidir. Yazılım geliştirme sırasında yapılan değişiklikleri kaydeder, geçmişe dönmeyi sağlar ve ekip çalışmasını kolaylaştırır. Git dağıtık çalışır, yani herkesin kendi bilgisayarında tam depo kopyası vardır.

### Temel Kavramlar
- **Repository (Depo):** Projenin tüm dosyalarının ve geçmişinin tutulduğu alan.
- **Commit:** Yapılan değişikliklerin kaydedilmesi.
- **Branch:** Farklı geliştirme hatları açmak için kullanılır. (ör. main, dev)
- **Merge:** Farklı branch’lerdeki değişiklikleri birleştirme işlemi.
- **Remote:** Uzak sunucuda bulunan depo (GitHub, GitLab gibi).
- **Staging Area (Index):** Commit yapılmadan önce değişikliklerin hazırlandığı alan.

### Temel Komutlar
- `git init` → Yeni bir Git deposu başlatır.
- `git clone <url>` → Var olan bir uzak depoyu bilgisayara kopyalar.
- `git status` → Değişikliklerin durumunu gösterir.
- `git add <dosya>` → Dosyayı commit’e hazırlamak için staging area’ya ekler.
- `git commit -m "mesaj"` → Yapılan değişiklikleri mesaj ile kaydeder.
- `git log` → Yapılan commit geçmişini listeler.
    - `git log --oneline` → Commit geçmişini tek satır halinde gösterir.
- `git diff` → Değişikliklerin ayrıntılarını gösterir.
- `git checkout <branch/commit>` → Farklı bir branch veya commit’e geçiş yapar.
- `git branch` → Branch listesini gösterir.
- `git branch <isim>` → Yeni branch oluşturur.
- `git merge <branch>` → Belirtilen branch’i mevcut branch ile birleştirir.
- `git remote add origin <url>` → Uzak depo ekler.
- `git remote -v` → Uzak depoları listeler.
- `git push origin <branch>` → Yerel branch’teki commitleri uzak depoya gönderir.
- `git pull origin <branch>` → Uzak depodan güncel değişiklikleri alır.
- `git fetch` → Uzak depodan yeni commitleri indirir ama merge etmez.

### İleri Seviye Komutlar
- `git reset` → Değişiklikleri geri alır.
    - `git reset --soft` → Commit’i geri alır ama dosyaları korur.
    - `git reset --hard` → Commit’i ve değişiklikleri tamamen siler.
- `git revert <commit>` → Belirtilen commit’i geri almak için yeni commit oluşturur.
- `git stash` → Henüz commit yapılmamış değişiklikleri geçici olarak saklar.
- `git tag` → Commit’lere etiket eklemek için kullanılır (sürüm numarası gibi).
- `git rebase` → Commit geçmişini yeniden düzenler.
- `git config` → Git'in ayarlarını yapmanızı sağlar.
    - `--global` → bu parametre yapılan ayarların bilgisayarınızdaki tüm Git projeleri için geçerli olmasını sağlar.
    - `git config --global user.name "Ramazan"` → Yaptığınız commit'lerde görünecek olan kullanıcı adınızı ayarlar.
    - `git config --global user.email "abc@gmail.com"` → Yaptığınız commit'lerde görünecek olan e-posta adresinizi ayarlar. 

### Git ile İlgili Araçlar
- **GitHub / GitLab / Bitbucket:** Uzak depo barındırma servisleri.
- **VS Code Git Eklentisi:** Kod editöründen Git işlemlerini kolayca yapmayı sağlar.
- **Sublime Merge / GitKraken:** Görsel arayüzle Git yönetim araçları.
