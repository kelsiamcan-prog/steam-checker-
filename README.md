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
