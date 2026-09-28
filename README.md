# 🚨 Deprem Tatbikat ve Kapı Kontrol Sistemi

Bu proje, okul ve kurum binalarında deprem anında yaşanabilecek tahliye zorluklarını önlemek amacıyla geliştirilmiş bir otomasyon sistemidir. 

*(Not: Projenin kaynak kodları okul laboratuvarı/eski bilgisayarım ortamında kaldığı için bu depoda projenin mimarisi ve çalışma mantığı sunulmuştur.)*

## 🎯 Projenin Amacı
Deprem sarsıntısı başladığında binadaki kilitli kapıların otomatik olarak açılmasını sağlayarak hızlı ve güvenli bir tahliye ortamı oluşturmak. Tahliye tamamlandıktan sonra ise olası hırsızlık vakalarını engellemek için kapıların uzaktan kumanda ile tekrar kilitlenebilmesini sağlamak.

## 🛠️ Kullanılan Teknolojiler ve Donanımlar
* **Mikrodenetleyici:** Arduino Uno
* **Sensörler:** Darbe/Titreşim Sensörü (Depremi algılamak için)
* **Aktüatörler:** Servo Motorlar / Selenoid Kilitler (Kapı mekanizmaları için)
* **Haberleşme:** RF veya IR Kumanda Modülü (Uzaktan kontrol için)

## ⚙️ Sistem Nasıl Çalışıyor?
1. **Algılama:** Titreşim sensörü, belirlenen şiddetin üzerinde bir sarsıntı algıladığında Arduino'ya sinyal gönderir.
2. **Tahliye Modu:** Arduino, kapılardaki kilit mekanizmalarına (motorlara) tetik göndererek tüm kapıları eşzamanlı olarak açar.
3. **Güvenlik Modu:** Acil durum sona erdiğinde, yetkili kişi uzaktan kumanda yardımıyla sisteme komut gönderir ve kapılar tekrar kilitli konuma geçer.
