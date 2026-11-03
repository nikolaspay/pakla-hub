# Pakla Hub 4.31.1

- **Pakla DNS:** VPN profil ekranı yerine, Windows 11'in yerleşik şifreli DNS desteğiyle Cloudflare 1.1.1.1 yönetimi. Aç/kapat, IPv4/IPv6, önceki DNS ayarını yedekleme/geri yükleme. DoH tanımlarında şifresiz UDP'ye geri dönüş kapalıdır. WARP kurulumu veya Pakla VPN sunucusu gerektirmez. Windows yönetici onayı ister; kurumsal DNS ilkelerini aşmaz. Windows 10'da bu özellik etkinleşmez.
- **Pakla Audio:** Pakla'nın kendi 10 bantlı stereo ekolayzırı, hazır ayarlar, ön kazanç ve yumuşak geçişler. Bu sürümde yalnız Pakla Müzik'teki MP3/WAV sesini işler; oyun, Spotify ve Windows sistem sesi kapsam dışıdır. FxSound gerekmez.
- **Pakla Driver:** Windows Update sürücü taraması, seçim ve lisans incelemesi sonrası yönetici onaylı kurulum. BIOS/firmware kapsam dışıdır; yeniden başlatma zorlanmaz.
- **Çeviriler:** uygulama içine gömülü Neko Çeviri × Pakla Çeviri kütüphanesi, iki logo, arama, favoriler, oyun sürümü uyarıları ve yerel kurulum kaydıyla Pakla'dan başlatma. Çevirilerin büyük bölümü Neko ekibinden gelir; kaynak/lisans bildirimleri korunur. Kurulum kaydı doğrulanan oyunlarda Pakla'dan başlatma sırasında otomatik intro oynatılır. İptal/hata olursa oyun başlatılmaz.
- **Topluluk ve DM:** keşfet kategorileri, kanalları sabitleme, sabit/yeni/tümü sohbet filtreleri, Türkçe arama ve hesaplara göre saklanan tercihler.
- Araçlarda Pakla isimleri, duyarlı ve dengeli yerleşim; çeviri görünümünün hata sonrası yeniden açılma düzeltmesi. X tepsiye küçültür; Tamamen çık açık işlemleri bekler.

## Sınırlar ve test durumu

DNS ayarları Windows'tan okunup doğrulanır; durum göstergesi bütün uygulamaların DNS yolunu kullandığının kanıtı değildir. IP/konum değiştirmez. Pakla kapansa da Windows ayarı korunur. Şifreli sağlayıcıya erişilemezse DNS çözümlemesi durabilir; Kapat eski ayarları geri yükler. Başka bir uygulama ayarları değiştirmişse Pakla üzerine yazmaz ve yedeği korur.

Çeviri girişindeki 'katalog incelendi' bilgisi gerçek oyun içi uyumluluk veya bütün yamalara güvenlik onayı anlamına gelmez. Horizon Remastered ve Little Nightmares kurulum güvenlik kapıları korunur. Complete Edition, Remastered yamasıyla uyumlu gösterilmez. **Steam/EXE üzerinden açılış kilidi uygulanmamıştır.** Pakla dışından başlatmanın engellendiği iddia edilmez.

Derleme, kendi DSP frekans/stereo testleri, 480/900/1540 piksel araç ve çeviri ekranları, DM filtreleri, test modunda sistem değişikliğini engelleme ve DNS işlemsel testleri geçti. DNS işlemsel testleri Windows komutlarının taklit edildiği yalıtılmış dosyalarda çalıştı: DHCP/statik geri yükleme, mevcut DoH tanımlarını koruma, kısmi hata geri alma, dış değişikliği ezmeme ve destek/ilke kontrolleri. Gerçek Windows DNS ayarları yalnız okundu; canlı yönetici onaylı DNS aç/kapat ve DoH paket trafiği testi henüz yapılmadı. Gerçek sürücü kurulumu, bu katalogdaki oyunlarda oyun içi test ve iki hesaplı canlı sosyal test bu sürüm çalışmasında yapılmadı.

Güncelleme paketi mevcut Pakla RSA yayın anahtarıyla imzalıdır; SHA-256 ve eski istemciyle uygulama/geri alma/veri koruma testleri ayrıca doğrulanır. Windows Authenticode yayıncı sertifikası yapılandırılmamıştır.

[Kurulum](PaklaHub-Kurulum.exe) · [SHA-256](SHA256SUMS.txt)
