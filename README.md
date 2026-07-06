<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/e43b9846-9126-4487-8f04-8fe084f4a283" />

⚡ Steam Account Checker & Checker Manager
Steam Account Checker, yüklediğiniz hesap listelerini modern Steam API'lerini kullanarak hızlı, güvenli ve otomatik olarak kontrol eden, gelişmiş bir hesap analiz ve tarama yazılımıdır.

Yazılım, güvenli lisans doğrulama (DRM) altyapısı ve donanım kimliği kilitleme (HWID Lock) özellikleri sayesinde tek bilgisayarda çalışacak şekilde koruma altına alınmıştır.

🚀 Öne Çıkan Özellikler
1. Modern Giriş Altyapısı (IAuthenticationService)
Steam'in en güncel şifreleme ve login akışını kullanır.
Hesapların geçerlilik durumunu doğrular ve Steam Guard (2FA / Mobil / E-posta) korumasına sahip hesapları anında tespit ederek guarded.txt dosyasına ayırır. Guard bulunmayan düz hesapları ise doğrudan içeri alır.
2. Kütüphane ve Aile Koruması Analizcisi
Giriş yapılan hesapların kütüphanesindeki oyunları sorgular. store.steampowered.com API entegrasyonu ile oyunların ID'leri yerine doğrudan isimlerini çözer (örn: Counter-Strike 2, PUBG, Rust).
Hesapta Aile Koruması (Parental PIN) veya Steam Ailesi (Steam Family) olup olmadığını otomatik kontrol eder.
3. Çoklu Thread ve Proxy Desteği
Eş zamanlı taranacak hesap sayısını (Thread) ayarlayabilirsiniz.
HTTP, HTTPS, SOCKS4 ve SOCKS5 proxy türlerini destekler. Proxy listesini uygulama içinden kontrol edip geçersiz olanları tek tıkla temizleyebilirsiniz.
4. Gelişmiş DRM ve Lisans Koruma Sistemi
1 Günlük Deneme Sürümü (Trial): Kullanıcılar uygulamayı test etmek için 1 günlük deneme başlatabilir. Deneme veritabanı Gist üzerinden anlık sorgulanır ve her bilgisayar bu haktan yalnızca 1 kez yararlanabilir.
5. Kullanıcı Dostu Arayüz ve Canlı Terminal
Modern koyu tema tasarımı, işlem sayaçları ve canlı ilerleme çubuğu.
💻 Terminal Sekmesi: Arka planda dönen tüm teknik logları, proxy hatalarını ve giriş denemelerini canlı olarak izleyebileceğiniz entegre bir konsol ekranı.
🗑 Dashboard Temizleyici: Tek tuşla tüm çıktı dosyalarını sıfırlama seçeneği.
🛠️ Nasıl Kullanılır?
Kullanıcılar İçin (Client):
Steam_Checker.exe dosyasını çalıştırın (Uygulama otomatik olarak yönetici yetkisi isteyecektir).
Karşınıza çıkan ekrandan Lisans Anahtarınızı girip doğrulayın veya 🎁 1 Günlük Deneme Sürümü butonuna tıklayarak testi başlatın.
Uygulama açıldığında:
Ayarlar sekmesinden proxy listesini yükleyin ve proxy türünü seçin.
Çoklu Hesap sekmesinden taranacak hesap listesini (kullaniciadi:sifre formatında) yükleyin.
▶ Giriş İşlemini Başlat butonuna basın.
Geçerli hesaplar valid.txt, hatalı hesaplar unvalid.txt ve guard korumalı hesaplar guarded.txt olarak uygulamanın çalıştığı klasöre kaydedilir. Canlı işlem loglarını Terminal sekmesinden izleyebilirsiniz.
Yapımcı / Satıcı İçin (Key Generator):
Lisans anahtarları üretmek için KeyGenerator klasöründeki key_generator.py dosyasını çalıştırın.
Kaç adet anahtar üretmek istediğinizi ve bu anahtarların kaç günlük olacağını (örn: 30 gün) belirleyin.
Üretilen anahtarlar otomatik olarak key.txt dosyasına kaydedilir ve doğrudan Gist veritabanınıza yüklenir. Kullanıcı bu anahtarı ilk kez girdiğinde 30 günlük süresi ve HWID eşleşmesi başlar.
⚠️ Güvenlik Uyarısı
Bu yazılım yalnızca İtemsatış ÜrünPazar mağazası (https://www.itemsatis.com/p/UrunPazar) üzerinden satılmaktadır.


----------------------------------------------------------------------------------------------------------------

⚡ Steam Account Checker & Checker Manager

Steam Account Checker is an advanced account analysis and scanning software that quickly, securely, and automatically checks uploaded account lists using modern Steam APIs.

The software is protected to run on a single computer thanks to its secure license verification (DRM) infrastructure and Hardware ID Lock (HWID Lock) features.

🚀 Key Features

**Modern Login Infrastructure (IAuthenticationService)**  
Uses Steam's latest encryption and login flow. Verifies the validity of accounts and instantly detects accounts protected by Steam Guard (2FA / Mobile / Email), separating them into the `guarded.txt` file. Accounts without Steam Guard protection are processed directly.

**Library and Family Protection Analyzer**  
Queries the games in the logged-in account's library. Through `store.steampowered.com` API integration, it resolves game IDs into their actual names (e.g., Counter-Strike 2, PUBG, Rust). It also automatically checks whether the account has Family View (Parental PIN) or Steam Family enabled.

**Multi-Thread and Proxy Support**  
You can configure the number of accounts to scan simultaneously (Threads). Supports HTTP, HTTPS, SOCKS4, and SOCKS5 proxy types. You can verify your proxy list within the application and remove invalid proxies with a single click.

**Advanced DRM and License Protection System**  
**1-Day Trial Version:** Users can start a 1-day trial to test the application. The trial database is queried in real time via Gist, and each computer can use this trial only once.

**User-Friendly Interface and Live Terminal**  
Modern dark theme design, operation counters, and a live progress bar.

💻 **Terminal Tab:** An integrated console where you can monitor all background technical logs, proxy errors, and login attempts in real time.

🗑 **Dashboard Cleaner:** Reset all output files with a single click.

🛠️ **How to Use**

**For Users (Client):**

Run the `Steam_Checker.exe` file (the application will automatically request administrator privileges).

On the screen that appears, enter and verify your License Key, or click the 🎁 **1-Day Trial Version** button to start the trial.

Once the application is open:

- Load your proxy list from the **Settings** tab and select the proxy type.
- Load the account list to be scanned (in `username:password` format) from the **Multi Account** tab.
- Press the ▶ **Start Login Process** button.

Valid accounts are saved as `valid.txt`, invalid accounts as `unvalid.txt`, and Steam Guard-protected accounts as `guarded.txt` in the application's working directory.

You can monitor live operation logs from the **Terminal** tab.

**For the Developer / Seller (Key Generator):**

Run the `key_generator.py` file in the **KeyGenerator** folder to generate license keys.

Specify how many keys you want to generate and how many days they should remain valid (e.g., 30 days).

The generated keys are automatically saved to the `key.txt` file and uploaded directly to your Gist database.

When a user enters the key for the first time, its validity period (e.g., 30 days) and HWID binding begin.

⚠️ **Security Warning**

This software is sold exclusively through the İtemsatış ÜrünPazar store (https://www.itemsatis.com/p/UrunPazar).
