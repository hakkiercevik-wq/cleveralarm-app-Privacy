# Gizlilik Politikası

**Son Güncelleme: 1 Mart 2026**

## CleverAlarm Uygulaması

### Genel Bakış

CleverAlarm uygulaması, gizliliğinize önem verir. Uygulamanın temel alarm ve görev (matematik, hafıza, sıra, adım vb.) özellikleri büyük ölçüde çevrimdışı çalışır. Uygulama **kendi sunucularımıza** kişisel verilerinizi göndermez.

Bu uygulama bazı özellikler için üçüncü taraf servisler (ör. Google AdMob, Google Play satın alma/güncelleme/yorum) kullanabilir. Bu servisler kendi gizlilik politikaları kapsamında **teknik veriler** işleyebilir (aşağıda).

### Veri Toplama ve Yerel Saklama

Uygulama bir kullanıcı hesabı oluşturmaz.

Uygulamanın kullandığı ve **cihazınızda yerel olarak** saklanan veriler (uygulamanın çalışması için gereken ayarlar) şunlardır:

- ⏰ Alarm ayarlarınız (saat, günler, etiket)
- 🔔 Ses tercihleri (seçilen zil sesi/sistem alarm sesi, ses seviyesi)
- 🧮 Matematik soru ayarları (soru sayısı, zorluk seviyesi)
- 🧠 Hafıza (Memory) görevi ayarları (örn. eş/kart sayısı)
- 🔁 Sıra Takibi (Sequence) görevi ayarları (örn. tur sayısı, sıra uzunluğu)
- 🚶 Adım görevi ayarları (örn. hedef adım sayısı)
- 🎨 Görünüm tercihi (karanlık/aydınlık tema)
- ✅ Alarm aktif/pasif durumları
- 🛒 “Reklamları kaldır” satın alma durum bilgisi (satın alındı/geri yüklendi)
- 🖼️ Alarm ekranı duvar kağıdı tercihi (seçilen duvar kağıdının dosya yolu veya uygulama içi hazır görsel seçimi)

Bu bilgilerin tamamı yalnızca cihazınızda (örn. SharedPreferences ve uygulama içi yerel dosyalar) saklanır.

**Duvar kağıdı (alarm ekranı arka planı):** Uygulama, isterseniz cihazınızdan bir görsel seçmenize ve kırpmanıza (crop) izin verir. Seçtiğiniz görsel, yalnızca uygulamanın çalışabilmesi için uygulamanın kendi yerel depolama alanına kopyalanabilir ve bu kopyanın yolu cihazınızda saklanır. Görsel uygulama tarafından internete yüklenmez ve uygulamanın kendi sunucularına gönderilmez.

Notlar:
- Fotoğraf/galeri erişimi, sistemin dosya seçicisi üzerinden ve yalnızca sizin seçtiğiniz dosya ile sınırlıdır.
- Uygulamayı kaldırdığınızda uygulama depolama alanındaki bu görseller de silinir.

**Adım verileri (Steps/Adım görevi):** Uygulama, cihaz sensörlerinden gelen adım bilgisini yalnızca alarm kapatma görevi için kullanır. Adım verisi uygulama içinde işlenir ve uygulamanın kendi sunucularına gönderilmez.

**Zil sesi / sistem alarm sesleri:**
- **Özel zil sesi** seçerseniz, yalnızca sizin seçtiğiniz ses dosyası kullanılabilir ve gerekli olduğunda uygulamanın yerel depolama alanına kopyalanabilir.
- **Sistem alarm sesleri** listesini görüntülediğinizde, Android’in sistem zil sesi listesindeki alarm seslerine ait başlık/URI gibi bilgiler uygulama içinde gösterilir.

Bu ses dosyaları uygulama tarafından internete yüklenmez.

### İnternet Bağlantısı

⚠️ Bu uygulama aşağıdaki durumlarda internet bağlantısı kullanabilir:

- Reklamların yüklenmesi (Google AdMob)
- Satın alma ve satın alma geri yükleme işlemleri (Google Play Billing)
- Uygulama içi güncelleme kontrolü (Google Play In-App Update)
- Uygulama içi değerlendirme/yorum isteme (Google Play In-App Review)
- Uygulama içindeki “Gizlilik Politikası” sayfasının GitHub üzerinden görüntülenmesi (WebView)

⚠️ “Gizlilik Politikası” sayfası GitHub üzerinde barındırılan bir dokümanı uygulama içinde (WebView) görüntüler. Bu sayfayı açtığınızda barındırma/altyapı sağlayıcıları (örn. GitHub) standart web sunucu günlükleri kapsamında bazı teknik verileri (örn. IP adresi, cihaz bilgisi, istek zamanı) işleyebilir.

✅ Alarm ayarlarınız internet gerektirmez ve çevrimdışı çalışır.

✅ Uygulama, kendi sunucularına kişisel veri göndermez.

### Üçüncü Taraf Hizmetler

Bu uygulama aşağıdaki üçüncü taraf servisleri kullanabilir:

- ✅ **Google AdMob (google_mobile_ads)**: Uygulama içi reklamları göstermek için kullanılır.
  - Reklam gösterimleri/tıklamaları ile ilgili ölçümler yapılabilir
  - Cihaz türü, işletim sistemi, IP adresi, yaklaşık konum (IP’den türetilebilir) gibi teknik bilgiler işlenebilir
  - Kişiselleştirilmiş reklamlar için reklam kimliği (Advertising ID) kullanılabilir (cihaz ayarlarından sınırlandırılabilir)
  - Google gizlilik politikası: https://policies.google.com/privacy

- ✅ **Google Play Billing (in_app_purchase)**: “Reklamları Kaldır” satın alımını yapmak ve satın alımı geri yüklemek için kullanılır.
  - Satın alma işlemleri Google Play üzerinden yürütülür
  - Satın alma durumuna dair basit bir durum bilgisi cihazınızda yerel olarak saklanabilir
  - Google gizlilik politikası: https://policies.google.com/privacy

- ✅ **Google Play In-App Update (in_app_update)**: Android’de uygulama güncellemelerini kontrol etmek/sunmak için kullanılır.
  - Bu işlem Google Play servisleri üzerinden yürütülür
  - Google gizlilik politikası: https://policies.google.com/privacy

- ✅ **Google Play In-App Review (in_app_review)**: Uygulama içi değerlendirme/yorum istemek için kullanılır.
  - Bu işlem Google Play servisleri üzerinden yürütülür
  - Google gizlilik politikası: https://policies.google.com/privacy

Diğer hizmetler (uygulamanın kendi içinde):
- ✅ **WebView (webview_flutter)**: Gizlilik politikası sayfasını uygulama içinde göstermek için
- ✅ **URL açma (url_launcher)**: tarayıcı/e-posta gibi uygulamaları açmak için
- ✅ **Paylaşım (share_plus)**: cihazın sistem paylaşım ekranını açmak için

Diğer hizmetler **KULLANILMAZ**:

- ❌ Analitik servisleri (Google Analytics, Firebase Analytics vb.)
- ❌ Çökme raporu servisleri (Crashlytics vb.)
- ❌ Sosyal medya entegrasyonları
- ❌ Kullanıcı takip araçları

### İzinler

Uygulama işlevlerine göre aşağıdaki Android izinlerini kullanır (bazıları Android sürümüne göre değişebilir):

1. **RECEIVE_BOOT_COMPLETED**: Cihaz yeniden başlatıldığında alarmları tekrar kurabilmek için
2. **WAKE_LOCK**: Alarm zamanı geldiğinde cihazı uyandırabilmek için
3. **VIBRATE**: Alarm titreşimini çalıştırabilmek için
4. **USE_FULL_SCREEN_INTENT**: Alarm çalarken tam ekran alarm arayüzünü gösterebilmek için
5. **POST_NOTIFICATIONS**: Alarm bildirimlerini gösterebilmek için
6. **ACTIVITY_RECOGNITION**: “Adım” görevi seçildiğinde adım sayısını okuyabilmek için
7. **FOREGROUND_SERVICE / FOREGROUND_SERVICE_MEDIA_PLAYBACK**: Alarm sesi/çalma sırasında arka planda güvenilir çalışabilmek için
8. **USE_EXACT_ALARM / SCHEDULE_EXACT_ALARM**: Alarmları tam zamanında kurabilmek için
9. **INTERNET / ACCESS_NETWORK_STATE**: Reklamlar, satın alma işlemleri, güncelleme/yorum akışları ve gizlilik politikası sayfasını görüntülemek için
10. **MODIFY_AUDIO_SETTINGS**: Alarm sesi/oynatım ayarlarını yönetebilmek için
11. **SYSTEM_ALERT_WINDOW**: Bazı cihazlarda alarm arayüzünü diğer uygulamaların üstünde gösterebilmek için (sistem ayarlarından yönetilebilir)

Dosya/medya erişimi:
- Özel zil sesi veya duvar kağıdı seçimi gibi durumlarda **sistem dosya seçici** kullanılır; uygulama yalnızca sizin seçtiğiniz dosyaya erişir.

### Kontrol ve Seçimler

- Kişiselleştirilmiş reklamları Android ayarlarından sınırlayabilirsiniz (reklam kimliği/kişiselleştirme ayarları).
- Uygulamanın yerel verilerini temizlemek için Android/iOS’ta “Uygulama verilerini sil” (Clear storage) seçeneğini kullanabilirsiniz.

### Veri Güvenliği

Uygulama verileri cihazınızda yerel olarak saklanır. Veri güvenliği cihazınızın güvenlik ayarlarına bağlıdır. Uygulamayı kaldırdığınızda uygulama depolama alanındaki veriler otomatik olarak silinir.

### Çocukların Gizliliği

Uygulama kendi sunucularına kişisel veri göndermez. Ancak uygulamada reklam gösterimi (Google AdMob) bulunabilir ve Google, reklam sunumu sırasında kendi politikalarına göre bazı teknik verileri işleyebilir. Daha fazla bilgi için Google gizlilik politikasını inceleyebilirsiniz: https://policies.google.com/privacy

### Değişiklikler

Bu gizlilik politikası gerektiğinde güncellenebilir. Değişiklik durumunda güncelleme tarihi bu sayfada belirtilir.

### İletişim

Gizlilik politikası hakkında sorularınız varsa bizimle iletişime geçebilirsiniz.

Destek e-postası: cleveralarmdestek@gmail.com

---

**Özetle:**
- ✅ Kendi sunucularımıza kişisel veri gönderilmez
- ✅ Alarm/görev ayarları cihazınızda yerel kalır
- ✅ Duvar kağıdı ve seçtiğiniz ses dosyaları internete yüklenmez
- ⚠️ Reklamlar için Google AdMob kullanılır
- ⚠️ Satın alma/güncelleme/yorum akışları Google Play servisleriyle çalışır

**Gönül rahatlığıyla kullanabilirsiniz!**
