# Pakla Hub 4.29.1

- Neko App, arkadaşımızın bağımsız projesi olarak tanıtılır. Pakla ailesi / kendi projemiz ifadeleri başlıktan, kartlardan, alt bilgiden ve hata görünümünden kaldırıldı.
- Neko sayfasında logo ile uyumlu mavi/turkuaz vitrin, renkli özellik kartları, simetrik ikonlar ve hafif hover/gezinme animasyonları.
- Pakla azaltılmış hareket/odak modu ve işletim sistemi hareket tercihinde animasyonlar durur. Gizli sayfada video duraklatılır.

Doğrulama: gerçek uygulama içi WebView2 sayfası ve video 480/1240 pikselde; sayfadan ayrılınca oynatıcının serbest bırakılması; 360/480/780/1180 HTML düzeni; dış site komutu ve azaltılmış hareket; imzalı paketin bütünlüğü, bozuk paket reddi, geri alma ve kullanıcı verilerini koruma kontrolleri geçti.

Neko’nun dış web hizmeti ve hesap akışı bu çalışmada test edilmedi. Windows Authenticode sertifikası yapılandırılmadı; uygulama içi güncelleme paketi mevcut RSA anahtarıyla ayrıca imzalıdır.
