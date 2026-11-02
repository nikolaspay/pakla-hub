# Pakla Hub 4.29.0

- Yeni Neko App bölümü: logo, yerel tanıtım fragmanı ve varsayılan tarayıcıda web sitesi bağlantısı.
- Neko fragmanı otomatik başlamaz; sayfa kapatıldığında oynatıcı serbest bırakılır.
- Yenilenen Pakla Clean: dosya bazında seçim, simetrik kartlar, inceleme/onay akışı ve azaltılmış hareket desteği.
- Tepside çalışma ve açık kayıt/sohbeti koruyan X davranışı devam eder.

## Doğrulama

Neko WebView2 görünümü ve yerel video 480/1240 pikselde; temizleme seçimleri ve korumaları; temel uygulama/tepsi yaşam döngüsü; kurulum çıkarma ve kapanma; RSA imzası, SHA-256, bozuk paket reddi, güncelleme geri alma ve kullanıcı verilerini koruma testleri geçti.

VPN hizmeti sağlanmaz; mevcut Windows VPN profilleri yönetilir. İki gerçek hesapla DM ve gerçek VPN bağlantısı bu yayın çalışmasında denenmedi. Neko'nun dış web hizmeti/hesap akışı test edilmedi. Windows Authenticode sertifikası yapılandırılmadı; uygulama içi güncelleme paketi mevcut RSA anahtarıyla ayrıca imzalıdır.
