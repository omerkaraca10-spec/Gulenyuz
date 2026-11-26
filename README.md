# Gülen Yüz – Android proje dosyaları

- Android Studio ile açılacak Kotlin projesidir.
- Android 8.0 (API 26) ve üzerini hedefler; Redmi Note 13 Pro 4G ile uyumludur.
- Google ML Kit yüz algılama modeli uygulamaya paketlenir. Uygulama kurulduktan sonra fotoğraf işleme internet gerektirmez.
- Fotoğraflar ACTION_OPEN_DOCUMENT ile seçilir; uygulama yalnızca seçilen fotoğrafları okur ve sonuçları `Pictures/GulenYuz` klasörüne yazar.
- En fazla 100 fotoğraf tek seferde seçilebilir.

## APK oluşturma

Android Studio'da bu klasörü açın, Gradle senkronizasyonunu tamamlayın ve `Build > Build Bundle(s) / APK(s) > Build APK(s)` seçin. APK genellikle `app/build/outputs/apk/debug/app-debug.apk` altında oluşur.

Not: Bu kaynak paketi bu çalışma ortamında Android SDK/Gradle bulunmadığı için burada APK olarak derlenemedi. İlk Gradle senkronizasyonunda Android Gradle Plugin ve ML Kit bağımlılığı indirilir; sonrasında uygulama cihazda çevrimdışı çalışır.
