# Pakla Hub 4.32.0

## Küçük ana kurulum

Ana EXE yaklaşık 4,2 MiB; kurulum yaklaşık 9,4 MiB. Önceki 4.31.1 ana EXE 34,0 MiB, kurulum 41,0 MiB idi. Karşılaştırma aynı yapılandırmada ölçülen dosya boyutlarıdır; Windows önbelleği, klipler, oyun yedekleri ve indirilen yamalar ayrıca yer kaplar.

Çeviri kütüphanesi/ortak kurulum görünümü, klip kayıt motoru ve Neko tanıtım medyası ayrı `.pakmodule` dosyalarıdır. Katalog ve beklenen SHA-256/boyut değerleri ana uygulamanın içine sabitlenir; ana uygulama mevcut RSA güncelleme güven zinciriyle dağıtılır. Her indirmede boyut/hash ve paket kaydı kontrol edilir. Başarısız/iptal edilmiş indirme geçici dosyasını temizler. Kullanıcı yalnız istediği ek bileşeni indirir, Araç kütüphanesinden kaldırır. Küçük Windows araçları ve Audio'nun küçük ortak ses kitaplıkları yerleşiktir; ayrıca indirilmiş gibi gösterilmez.

## Oyun başına yama

Yama arşivleri ve eski Hades/Borderlands motoru ana kurulumda veya ortak çeviri modülünde yoktur. Kullanıcı oyun seçince yalnız o oyun için gerekli dosyalar boyut/SHA-256 doğrulanarak indirilir ve seçilen oyun klasörüne kurulur. Hades/Borderlands için ortak eski motor da ilk ihtiyaçta indirilir. İndirilen dosyalar doğrulama alanında tutulabilir; oyun klasöründeki özgün dosya yedekleri korunur. Çeviri modülünü kaldırmak oyunlara kurulmuş yamaları kaldırmaz.

Townfall ve Reunion paketleri kullanıcıda bulunmadığından bu ikisi 'Yama paketi yok' durumundadır. Horizon Remastered ve Little Nightmares kurulum güvenlik kapıları korunur. Tüm 12 kartta 'Katalog doğrulandı' yalnız katalog/sürüm/akış kontrolünü ifade eder; oyun içi test veya güvenlik onayı değildir. Açıklamalar bu ayrımı korur.

## Araç kullanım koşulları

İlgili araca ilk girişte amaç, işlemler, veri/üçüncü taraf bağlantıları ve kullanım sınırları gösterilir. 'Okudum ve kabul ediyorum' kutusu seçili gelmez. Reddetmek diğer bölümleri kapatmaz. Onay, bu cihazdaki Pakla hesabı/konuk profiline göre araç ve metin SHA-256'sıyla saklanır; metin değişirse yeniden istenir. Bu ekran genel KVKK açık rızası, pazarlama izni veya bütün Windows yönetici işlemlerine peşin onay değildir. Yasal hakları kaldıran bir sorumsuzluk hükmü eklenmedi. Destek: supportpakla@gmail.com.

Metinler uygulamanın yaptığı işlemleri açıklayan kullanım koşullarıdır; ticari unvan/adres gibi doğrulanmamış bir işletme kimliği uydurulmadı. Gizlilik/aydınlatma yükümlülüklerinin tamamlandığı veya hukuki uygunluk denetimi yapıldığı iddia edilmez.

Başvurulan resmi kaynaklar:
- https://www.kvkk.gov.tr/Icerik/4239/100-Soruda-Kisisel-Verilerin-Korunmasi-Kanunu
- https://tuketici.ticaret.gov.tr/yayinlar/tuketici-bilgi-rehberi/tuketici-sozlesmelerindeki-temel-ilkeler-ve-haksiz-sartlar-hakkinda-bilgilendirme

## Arayüz ve testler

Sohbet filtrelerinde ikonlar kaldırıldı; Tümü/Yeni/Sabit etiketleri %100/%150/%200 DPI'da ortalanır ve kesilmez. Klavye odağı yuvarlak çizilir. Katalog şeridinin yerleşimi korunur; metin ve durum açıklamaları güncellendi.

Derleme, kaynak yedeğinden yeniden derleme, paket imzası/eski istemci geri alma testleri, modül bütünlüğü, açık onay/metin değişimi, filtre eylemleri, 12 kart ve güvenlik/missing-paket durumları, görünüm toparlanması, kurulum yaşam döngüsü ve mevcut uygulama self-test kontrol edilir. Gerçek sürücü kurulumu, canlı DNS aç/kapat ve katalog oyunlarında oyun içi test bu çalışmada yapılmadı.

Derleme: Windows x64, .NET Framework 4.8 ve Python 3 gerekir. `Build.ps1 -PythonPath C:\Python313\python.exe` ile Python yolu seçilebilir. Kaynak yedeğinde bağımlılıklar, imzalı dağıtımın yalnız açık anahtarı ve kaynak/lisans bildirimleri bulunur; düz metin özel imzalama anahtarı eklenmez.
