# Gizlilik Politikası

**Son Güncelleme: 19 Eylül 2026**

## CleverAlarm Uygulaması

### Genel Bakış

CleverAlarm uygulaması, gizliliğinize önem verir. Uygulamanın temel alarm ve görev (matematik, hafıza, sıra, adım vb.) özellikleri büyük ölçüde çevrimdışı çalışır. Uygulama **kendi sunucularımıza** kişisel verilerinizi göndermez.

Bu uygulama bazı özellikler için üçüncü taraf servisler (ör. Google AdMob, Unity Ads aracılığı, Firebase Analytics/Crashlytics/Remote Config, Google Play satın alma/güncelleme/yorum) kullanabilir. Bu servisler kendi gizlilik politikaları kapsamında **teknik veriler** (cihaz veya diğer kimlikler dahil) işleyebilir ve Google / reklam ortaklarıyla paylaşabilir (aşağıda).

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
- 🖼️ Eşya Avı görevi (seçilen nesne listesi)
- 📷 QR / barkod görevi (kayıtlı kod bilgisi)
- 🛡️ Kapanma koruması açık/kapalı tercihi

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

- Reklamların yüklenmesi (Google AdMob ve aracılık ağları, örn. Unity Ads)
- Kullanım ölçümü (Google Analytics for Firebase)
- Çökme/hata raporlama (Firebase Crashlytics)
- Uzaktan yapılandırma (Firebase Remote Config)
- Satın alma ve satın alma geri yükleme işlemleri (Google Play Billing)
- Uygulama içi güncelleme kontrolü (Google Play In-App Update)
- Uygulama içi değerlendirme/yorum isteme (Google Play In-App Review)
- Uygulama içindeki “Gizlilik Politikası” sayfasının GitHub üzerinden görüntülenmesi (WebView)

⚠️ “Gizlilik Politikası” sayfası GitHub üzerinde barındırılan bir dokümanı uygulama içinde (WebView) görüntüler. Bu sayfayı açtığınızda barındırma/altyapı sağlayıcıları (örn. GitHub) standart web sunucu günlükleri kapsamında bazı teknik verileri (örn. IP adresi, cihaz bilgisi, istek zamanı) işleyebilir.

✅ Alarm ayarlarınız internet gerektirmez ve çevrimdışı çalışır.

✅ Uygulama, kendi sunucularına kişisel veri göndermez.

### Üçüncü Taraf Hizmetler

Bu uygulama aşağıdaki üçüncü taraf servisleri kullanabilir:

- ✅ **Google AdMob (google_mobile_ads) ve reklam aracılığı (Unity Ads)**: Uygulama içi reklamları göstermek için kullanılır.
  - Reklam gösterimleri/tıklamaları ile ilgili ölçümler yapılabilir
  - Cihaz türü, işletim sistemi, IP adresi, yaklaşık konum (IP’den türetilebilir) gibi teknik bilgiler işlenebilir
  - Reklam ve ölçüm için **cihaz veya diğer kimlikler** (ör. Android Reklam Kimliği / Advertising ID, uygulama örnek kimliği) toplanabilir ve Google ile reklam ortaklarına **paylaşılabilir**
  - Kişiselleştirilmiş reklamları cihaz ayarlarından sınırlayabilirsiniz; bu durumda reklam yine gösterilebilir ama daha az kişiselleştirilir
  - Google gizlilik politikası: https://policies.google.com/privacy
  - Unity gizlilik politikası: https://unity.com/legal/privacy-policy

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

  
- ✅ **Google Analytics for Firebase**
  Uygulama performansını ölçmek, hangi ekranların kullanıldığını anlamak ve reklamların teknik olarak çalışıp çalışmadığını görmek için kullanılır.

  İsim, e-posta veya telefon toplanmaz. İşlenenler kullanım olayları (ekran, tıklama, oturum) ve reklam istek/gösterim gibi teknik ölçümlerdir. Bu ölçümler **cihaz veya diğer kimlikler** (ör. uygulama örnek kimliği, reklam kimliği) ile ilişkilendirilebilir ve Google’a aktarılabilir.

  Amaç: analiz ve reklam/ölçüm. Verilerinizi satmayız. Google, kendi gizlilik politikasına göre bu teknik verileri işleyebilir.

  - Google gizlilik politikası: https://policies.google.com/privacy

- ✅ **Firebase Crashlytics**: Üretim (release) sürümlerinde çökme ve kritik hataları raporlamak için (debug/test sürümlerinde varsayılan olarak kapalıdır).
  - Kilitlenme günlükleri, cihaz modeli, işletim sistemi sürümü ve uygulama sürümü gibi tanılama bilgileri gönderilebilir
  - Kurulum/cihaz kimliği benzeri teknik kimlikler kullanılabilir
  - Google gizlilik politikası: https://policies.google.com/privacy

- ✅ **Firebase Remote Config**: Uygulama ayarlarını uzaktan güncellemek için (ör. reklam/akış bayrakları). Teknik uygulama kimliği Google’a gidebilir.

Diğer hizmetler (uygulamanın kendi içinde):
- ✅ **WebView (webview_flutter)**: Gizlilik politikası sayfasını uygulama içinde göstermek için
- ✅ **URL açma (url_launcher)**: tarayıcı/e-posta gibi uygulamaları açmak için
- ✅ **Paylaşım (share_plus)**: cihazın sistem paylaşım ekranını açmak için (tanı loglarını destek ekibine göndermek dahil)
- ✅ **Yerel tanı günlüğü**: Sorun giderme için cihazda geçici olarak tutulan teknik log dosyası; yalnızca siz “Tanı loglarını gönder” seçeneğini kullanırsanız paylaşılır

Diğer hizmetler **KULLANILMAZ**:

- ❌ Sosyal medya entegrasyonları
- ❌ Kullanıcı takip araçları (reklam/analitik dışında)

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
9. **INTERNET / ACCESS_NETWORK_STATE**: Reklamlar, analiz, çökme raporu, uzaktan yapılandırma, satın alma, güncelleme/yorum ve gizlilik politikası sayfası için
10. **MODIFY_AUDIO_SETTINGS**: Alarm sesi/oynatım ayarlarını yönetebilmek için
11. **SYSTEM_ALERT_WINDOW**: Bazı cihazlarda alarm arayüzünü diğer uygulamaların üstünde gösterebilmek için (sistem ayarlarından yönetilebilir)
12. **CAMERA**: QR / barkod tarama ve Eşya Avı (nesne tanıma) görevleri için. Kamera görüntüsü bu görevler sırasında cihazda işlenir; uygulamanın kendi sunucusuna yüklenmez
13. **Erişilebilirlik hizmeti (isteğe bağlı)**: Yalnızca “Kapanma koruması” açıksa ve alarm / uyanma görevi / uyanma kontrolü sırasında güç menüsünü kapatmak için. Alarm yokken çalışmaz. Bu hizmet aracılığıyla kişisel veri toplanmaz, saklanmaz veya üçüncü taraflarla paylaşılmaz

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
- ✅ Kendi sunucularımıza kişisel veri (isim, e-posta, alarm içeriği) gönderilmez
- ✅ Alarm/görev ayarları cihazınızda yerel kalır
- ✅ Duvar kağıdı, kamera görüntüsü ve seçtiğiniz ses dosyaları internete yüklenmez
- ⚠️ Reklam, analiz ve çökme raporu için Google (AdMob, Analytics, Crashlytics) ve reklam aracılığı cihaz kimliği işleyebilir ve paylaşabilir
- ⚠️ Satın alma/güncelleme/yorum akışları Google Play servisleriyle çalışır

**Gönül rahatlığıyla kullanabilirsiniz!**
