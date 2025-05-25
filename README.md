# Görme Engelliler için Ultrasonik Titreşimli Uyarı Sistemi

Bu proje, görme engelli bireylerin önlerindeki engelleri algılamalarına yardımcı olmak amacıyla geliştirilmiştir. HC-SR04 ultrasonik sensör ile çevredeki nesnelerin mesafesi ölçülür ve 50 cm'den daha yakına gelen nesneler için titreşim motoru devreye girer. Nesne yaklaştıkça titreşim aralığı kısalır ve uyarı artar.

## 🛠 Kullanılan Malzemeler
- Arduino Uno
- HC-SR04 Ultrasonik Mesafe Sensörü
- Titreşim Motoru
- NPN Transistör (BC547, 2N2222 vb.)
- 1kΩ Direnç
- 1N4007 Diyot
- Jumper Kablolar
- Breadboard
- 3D Yazıcı ile üretilmiş muhafaza kutusu (isteğe bağlı)

## ⚙️ Devre Şeması

!Devre şeması şıkıştırılmış klasör içinde mevcuttur

## 💾 Arduino Kodu

Kod dosyası: `gorme_engelli.cpp`

Temel işleyiş:
- HC-SR04 sensörü mesafeyi ölçer.
- Mesafe 50 cm'den küçükse titreşim motoru çalışır.
- Mesafe azaldıkça titreşim aralığı kısalır (daha sık titreşim).

## 🔩 Montaj Bilgisi

Devre, 3D yazıcı ile üretilmiş kompakt bir kutu içerisine yerleştirilerek dış etkenlerden korunur. Bu kutu, bir görme engelli bastonunun (değneğin) üzerine sabitlenerek taşınabilir hale getirilmiştir. Böylece sistem hem kullanışlı hem de günlük yaşamda rahatça entegre edilebilir bir hale gelir.

## 🚀 Nasıl Çalıştırılır?
1. Devreyi bağlantı şemasına göre kurun.
2. Arduino IDE ile `gorme_engelli.cpp` dosyasını açın.
3. Kodu Arduino'ya yükleyin.
4. Cihaza 5V güç verin.
5. Motor, engel 50 cm yakına geldiğinde titreşimle uyarı verir.

## 📌 Notlar
- Titreşim motoru transistör ile sürülmelidir. Doğrudan Arduino pinine bağlamak önerilmez.
- Harici güç kaynağı ile daha güçlü titreşim motorları kullanılabilir.
- Kutunun içinde yeterli havalandırma olduğundan emin olun.

## 🧑‍💻 Geliştiren
Bu proje, açık kaynak olarak paylaşıldı. İsteyen herkes geliştirebilir veya üzerine eklemeler yapabilir.
