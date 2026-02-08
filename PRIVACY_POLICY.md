# Gizlilik Politikası

**Son Güncelleme: 9 Şubat 2026**

## CleverAlarm Uygulaması

### Genel Bakış

CleverAlarm uygulaması, gizliliğinize önem verir. Uygulama temel alarm ve matematik özelliklerinde çevrimdışı çalışır ve kişisel verilerinizi kendi sunucularımıza göndermeyiz.

### Veri Toplama

Uygulamanın kendisi bir kullanıcı hesabı oluşturmaz ve kendi sunucularımıza kişisel verilerinizi göndermeyiz.

Ancak uygulama, **reklam** ve **satın alma** özellikleri için Google hizmetlerini kullandığından, bu üçüncü taraflar kendi gizlilik politikalarına göre bazı teknik verileri işleyebilir (aşağıda detaylı).

Uygulamanın kullandığı ve **cihazınızda yerel olarak** saklanan veriler şunlardır:

- ⏰ Alarm ayarlarınız (saat, günler, etiket)
- 🔔 Ses tercihleri (zil sesi seçimi, ses seviyesi)
- 🧮 Matematik soru ayarları (soru sayısı, zorluk seviyesi)
- 🧠 Hafıza (Memory) görevi ayarları (örn. eş/kart sayısı)
- 🔁 Sıra Takibi (Sequence) görevi ayarları (örn. tur sayısı, sıra uzunluğu)
- 🚶 Adım görevi ayarları (ör. hedef adım sayısı)
- 🎨 Görünüm tercihi (karanlık/aydınlık tema)
- ✅ Alarm aktif/pasif durumları
- 🛒 “Reklamları kaldır” satın alma durum bilgisi (satın alındı/geri yüklendi)
- 🖼️ Alarm ekranı duvar kağıdı tercihi (seçilen duvar kağıdının dosya yolu veya uygulama içi hazır görsel seçimi)

Bu bilgilerin tamamı yalnızca cihazınızda SharedPreferences kullanılarak saklanır ve cihazınızdan çıkmaz.

**Duvar kağıdı (alarm ekranı arka planı):** Uygulama, isterseniz cihazınızdan bir görsel seçmenize ve kırpmanıza (crop) izin verir. Seçtiğiniz görsel, yalnızca uygulamanın çalışabilmesi için uygulamanın kendi yerel depolama alanına kopyalanabilir ve bu kopyanın yolu cihazınızda saklanır. Görselin kendisi uygulama tarafından internete yüklenmez ve uygulamanın kendi sunucularına gönderilmez.

Notlar:
- Fotoğraf/galeri erişimi, sistemin dosya seçicisi üzerinden ve yalnızca sizin seçtiğiniz dosya ile sınırlıdır.
- Uygulamayı kaldırdığınızda uygulama depolama alanındaki bu görseller de silinir.

**Adım verileri (Steps/Adım görevi):** Uygulama, adım sayacı/ivmeölçer gibi cihaz sensörlerinden gelen adım bilgisini yalnızca alarm kapatma görevi için kullanır. Adım sayısı uygulama içinde işlenir ve uygulamanın kendi sunucularına gönderilmez.

**Özel zil sesi:** İsterseniz cihazınızdan bir ses dosyası seçebilirsiniz. Uygulama, seçtiğiniz dosyanın yolunu/kimliğini yerel olarak kaydedebilir ve alarm çalarken o dosyayı kullanabilir. Bu dosya içeriği uygulama tarafından internete yüklenmez.

### İnternet Bağlantısı

⚠️ Bu uygulama reklamlar ve satın alma doğrulaması için internet bağlantısı kullanır.

⚠️ Uygulama içindeki “Gizlilik Politikası” sayfası, GitHub üzerinde barındırılan bir dokümanı uygulama içinde görüntüler. Bu sayfayı açtığınızda GitHub/Google gibi altyapı sağlayıcıları standart web sunucu günlükleri kapsamında bazı teknik verileri (örn. IP adresi, cihaz bilgisi, istek zamanı) işleyebilir.

✅ Alarm ayarlarınız internet gerektirmez ve çevrimdışı çalışır.

✅ Uygulamanın kendi sunucularına kişisel veri göndermez.

### Üçüncü Taraf Hizmetler

Bu uygulama aşağıdaki Google servislerini kullanabilir:

- ✅ **Google AdMob**: Uygulama içi reklamları göstermek için kullanılır.
  - Reklam gösterimleri/tıklamaları ile ilgili ölçümler yapılabilir
  - Cihaz türü, işletim sistemi, IP adresi, yaklaşık konum (IP’den türetilebilir) gibi teknik bilgiler işlenebilir
  - Kişiselleştirilmiş reklamlar için reklam kimliği (Advertising ID) kullanılabilir (cihaz ayarlarından sınırlandırılabilir)
  - Google'un gizlilik politikası: https://policies.google.com/privacy

- ✅ **Google Play Billing (Satın Alma)**: “Reklamları Kaldır” satın alımını yapmak ve satın alımı geri yüklemek için kullanılır.
  - Satın alma işlemleri Google Play üzerinden yürütülür
  - Satın alma durumunun (satın alındı/geri yüklendi) cihazda saklanması için yerel kayıt tutulur
  - Google'un gizlilik politikası: https://policies.google.com/privacy

Diğer hizmetler **KULLANILMAZ**:

- ❌ Analitik servisleri (Google Analytics, Firebase, vb.)
- ❌ Çökme raporu servisleri
- ❌ Sosyal medya entegrasyonları
- ❌ Kullanıcı takip araçları

### İzinler

Uygulama şu izinleri kullanır:

1. **Bildirim İzni**: Alarm zamanı geldiğinde sizi uyarmak için
2. **Tam Ekran Alarm İzni**: Alarm çaldığında matematik ekranını otomatik açmak için
3. **Alarm/Zamanlayıcı İzni**: Belirlediğiniz saatlerde alarm kurmak için
4. **İnternet İzni**: Reklamları yüklemek için

Opsiyonel/özelliğe bağlı izinler:

5. **Hareket/Fiziksel Aktivite (Adım sayma) İzni**: “Adım” kapatma görevi seçildiğinde adım sayısını okuyabilmek için (Android: ACTIVITY_RECOGNITION, iOS: Motion & Fitness)
6. **Dosya Seçme/Medya Erişimi**: Özel zil sesi seçmek istediğinizde sistem dosya seçicisini açmak için (dosya seçimi tamamen sizin kontrolünüzdedir)

**Hafıza (Memory)** ve **Sıra Takibi (Sequence)** görevleri ek bir cihaz izni gerektirmez; yalnızca uygulama içinde çalışır.

Not: Satın alma özelliği kullanıldığında Google Play altyapısı ile iletişim kurulabilir.

Bu izinler yalnızca uygulamanın temel işlevselliği için kullanılır. Alarm ayarlarınız gibi kişisel verileriniz hiçbir zaman internete gönderilmez.

### Veri Güvenliği

Tüm verileriniz cihazınızda yerel olarak saklandığı için, veri güvenliği tamamen cihazınızın güvenlik ayarlarına bağlıdır. Uygulamayı kaldırdığınızda tüm veriler otomatik olarak silinir.

### Çocukların Gizliliği

Bu uygulama her yaştan kullanıcı tarafından kullanılabilir. Uygulama kendi sunucularına kişisel veri göndermez.

Ancak uygulamada reklam gösterimi (Google AdMob) bulunabilir. Google, reklam sunumu sırasında kendi politikalarına göre bazı teknik verileri işleyebilir. Çocukların gizliliği hakkında daha fazla bilgi için Google gizlilik politikasını inceleyebilirsiniz: https://policies.google.com/privacy

### Değişiklikler

Bu gizlilik politikası gerektiğinde güncellenebilir. Herhangi bir değişiklik durumunda, güncelleme tarihi bu sayfada belirtilecektir.

### İletişim

Gizlilik politikası hakkında sorularınız varsa, lütfen uygulama geliştirici ile iletişime geçin.

Destek e-postası: cleveralarmdestek@gmail.com

---

**Özetle:**
- ✅ Alarm ayarlarınız tamamen çevrimdışı çalışır
- ✅ Uygulamanın kendi sunucularına kişisel veriler gönderilmez
- ✅ Duvar kağıdı (alarm ekranı arka planı) seçiminiz cihazınızda saklanır ve internete yüklenmez
- ⚠️ Reklamlar için Google AdMob kullanılır
- ⚠️ Reklamları kaldırma satın alımı için Google Play Billing kullanılabilir
- ✅ Tüm alarm verileriniz sadece cihazınızda
- ✅ Adım görevi verileri cihazda işlenir
- ✅ Gizliliğinizi korumaya odaklanır

**Gönül rahatlığıyla kullanabilirsiniz!** 🔒
