# SUNİ-UFUK
OSMAN, ÖMER, ÖZGÜR adlı kullanıcıların ortaya koydukları çalışma

Proje Süreci ve Yapay Zeka İş Bölümü
Bu projede üç kişilik bir ekip olarak Google Gemini 3.1 Pro'dan yoğun şekilde faydalandık. 

Ekibimizin Görevi: Renk ayarları, güç dağıtımları ve yön tuşları gibi temel arayüz tasarımını ve basit mantık işlemlerini biz üstlendik.

Yapay Zekanın Görevi: Projenin "beyni" olarak; B737 MAX 8 aerodinamiği, PID kontrol mantığı ve Suni Ufuk (ADI) trigonometrisi gibi karmaşık matematiksel hesaplamaları yapay zekaya kodlattık. Daha sonra bu iki yapıyı entegre ettik.

Eski Kuralları Bozma: Yeni özellikler eklerken eski kuralları unuttu. Örneğin, havacılık kuralı olan "sola yatışta ufkun sağa devrilmesi" mantığını sık sık standart bir oyun gibi (sola basınca ufkun sola yatması) algılayarak bozdu. Bunu komutlarla sürekli hatırlatmak zorunda kaldık.

Görsel İkazları Silme: Kodu güncellerken, GPWS sistemi için daha önce eklediğimiz "TERRAIN" ikazı gibi çalışan kısımları dikkatsizlik sonucu koddan sildi.

Yazım (Sentaks) Hataları: Harf büyüklüğü hataları (YESIL yerine YESil yazmak) veya eksik parantezler yüzünden kod çöktü. Kodu satır satır okumak yerine, terminaldeki hata çıktılarını kopyalayıp yine yapay zekaya vererek kendi hatasını (debug) çözmesini sağladık.

Kapasite Aşımı: Kod 500 satıra ulaşıp maskelemeler ve uyarı sistemleri eklendiğinde standart model tıkandı ve cevapları yarıda kesti. Bu sorunu aşmak için, daha yavaş ama derin analiz yapabilen "Düşünme (Reasoning) Modu"na geçerek projenin tamamlanmasını sağladık.

Sonuç
Yapay zeka bu projede harika işler çıkarmış olsada sürekli denetlenip yönlendirilmeye ihtiyacı var. Basit işleri bizim, ağır hesaplamaları yapay zekanın yaptığı ve hatalarını yine kendisine çözdürdüğümüz bu stratejiyle projeyi başarıyla tamamladık.

