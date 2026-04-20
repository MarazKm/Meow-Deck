**🐾 Meow Deck v2.0: Advanced Macro Console**

OLED Integrated, Dual-Encoder Control, and Dynamic Centering Engine
Meow Deck, sıradan bir makro klavyenin ötesinde; görsel geri bildirim, hassas döner kontrolörler ve optimize edilmiş bir kullanıcı arayüzü sunan gelişmiş bir kontrol istasyonudur. Bu proje, maliyet etkinliği ve yüksek performansı birleştiren "Maker" ruhuyla geliştirilmiştir.

**🏗️ Teknik Mimari ve Donanım**

**Kontrol ve Girdi Katmanı**

 - **Key Matrix (2x5):** Toplam 10 mekanik tuş, matris yapısı sayesinde minimum pin kullanımıyla maksimum tepkisellik sunar.

 - **Dual Rotary Encoders:** Ses kontrolü ve sayfa/menü geçişleri için iki adet enkoder entegre edilmiştir. Sinyal yönleri yazılımsal olarak kalibre edilmiştir.

 - **Physical Reset System:** Geliştirme sürecini kolaylaştırmak için RST ve GND arasına fiziksel bir donanım reset butonu eklenmiştir.

**Görsel Arayüz (OLED Engine)**
   
 - **Dynamic Centering:** ikonCiz fonksiyonu, metin ve görselleri ekran genişliğine (128px) göre matematiksel olarak otomatik hizalar.

 - **Custom Graphics:** 32x32 ve 48x48 piksel boyutlarında, PROGMEM üzerinde saklanan özel ikon seti (Kalp, Mikrofon Durumu, Sablon).

🔌 Pin Bağlantı Haritası (Technical Mapping)
 
   **Modül,Pinler,Fonksiyon**

- **OLED Display**,"SDA (2), SCL (3)",I2C Communication

- **Key Matrix**,"R: 4,5 / C: 6, A0, A1, A2, A3",10-Key Input

- **Encoder 1 (Ses)**,"7, 8 (Sinyal), 14 (Buton)",Master Volume Control

- **Encoder 2 (Nav)**,"10, 9 (Sinyal), 15 (Buton)",Page / Layer Navigation

- **Reset Switch**,"RST, GND",Hardware Debugging

**🎨 Tasarım ve Gövde (Enclosure)**

- Proje, "Accessibility and Sustainability" (Erişilebilirlik ve Sürdürülebilirlik) prensibiyle tasarlanmıştır:

**Kasa**: El yapımı veya geri dönüştürülmüş malzemelerden (DIY) üretilmeye uygun modüler yapı.

**Ergonomi**: Kullanıcının tercihine göre optimize edilebilir 35∘ eğimli yerleşim.

**💻 Yazılım Özellikleri**

- **HID-Project:** Multimedya ve sistem kısayolları için genişletilmiş klavye desteği.

- **Adafruit_SSD1306:** Optimize edilmiş grafik renderlama.

- **Kısayol Setleri:** Discord (Mic/Cam Mute), Windows yönetimi ve özelleştirilmiş makrolar.
