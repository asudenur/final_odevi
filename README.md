# TODO List Uygulaması (Flutter + Firebase)

Bu proje, Final Mobil Programlama Dersi kapsamında Flutter ve Firebase kullanılarak geliştirilmiş bir TODO listesi uygulamasıdır. Kullanıcılar görev ekleyebilir, tamamlanan görevleri işaretleyebilir ve tüm veriler Firestore veritabanında **gerçek zamanlı** olarak güncellenir.

## 🔧 Kullanılan Teknolojiler

- Flutter
- Firebase Firestore
- DatePicker
- DropdownButton (varsayılan Flutter ikonları)
- BottomSheet Modal
- Checkbox

## 📱 Özellikler

- **Gerçek zamanlı güncelleme:** Firestore üzerinde yapılan tüm değişiklikler anlık olarak kullanıcı arayüzünde yansıtılır.
- **Bottom Modal** kullanarak yeni görev ekleme
- Görev oluşturulurken kullanıcıdan şu bilgiler alınır:
  - **İkon:** Sabit bir listedeki 10 Flutter varsayılan ikonundan seçim yapılır (DropdownButton ile)
  - **Başlık**
  - **Alt Başlık (İçerik bilgisi)**
  - **Zaman bilgisi** (DatePicker ile seçilir)
- **Veriler Firestore’a kaydedilir.**
- Kullanıcı sadece belirlenen 10 ikondan seçim yapabilir.
- Firestore’dan veri çekilirken sadece bu ikonlar dikkate alınır.
- Her görev için bir **Checkbox** bulunur:
  - Checkbox işaretlendiğinde görev başlığı **üstü çizili** hale gelir ve veritabanı güncellenir.
  - Checkbox kaldırıldığında başlık normale döner ve veritabanı yeniden güncellenir.

## 📝 Kurulum ve Kullanım

1. Firebase hesabı oluşturun ve bir Firestore projesi açın.
2. Flutter projenizi bu Firebase projesine bağlayın.
3. Gerekli bağımlılıkları yükleyin:
   ```bash
   flutter pub get
