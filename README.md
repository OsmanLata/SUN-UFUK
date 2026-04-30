# SUNİ-UFUK
OSMAN, ÖMER, ÖZGÜR adlı kullanıcıların ortaya koydukları çalışma

Proje Süreci ve Yapay Zeka İş Bölümü
Bu projede üç kişilik bir ekip olarak Google Gemini 3.1 Pro'dan yoğun şekilde faydalandık. 

Yapay Zekanın Görevi: Projeyi sıfırdan adım adım yapay zekaya soru sorarak, analiz ve deneme yöntemleriyle; en basit yön tuşlarıyla lineer çalışan bir suni ufuktan, daha kompleks lineer tepki vermeyen ve ekstradan altimetre, varyometre, directional gyro gibi ekstradan birçok özelliği bulunan bir suni ufuk tasarımı elde etmeyi başardık.

Eski Kuralları Bozma: Yeni özellikler eklerken eski kuralları unuttu. Örneğin, havacılık kuralı olan "sola yatışta ufkun sağa devrilmesi" mantığını sık sık standart bir oyun gibi (sola basınca ufkun sola yatması) algılayarak bozdu. Bunu komutlarla sürekli hatırlatmak zorunda kaldık.

Görsel İkazları Silme: Kodu güncellerken, GPWS sistemi için daha önce eklediğimiz "TERRAIN" ikazı gibi çalışan kısımları dikkatsizlik sonucu koddan sildi.

Yazım (Sentaks) Hataları: Harf büyüklüğü hataları (YESIL yerine YESil yazmak) veya eksik parantezler yüzünden kod çöktü. Kodu satır satır okumak yerine, terminaldeki hata çıktılarını kopyalayıp yine yapay zekaya vererek kendi hatasını (debug) çözmesini sağladık.

Kapasite Aşımı: Kod 500 satıra ulaşıp maskelemeler ve uyarı sistemleri eklendiğinde standart model tıkandı ve cevapları yarıda kesti. Bu sorunu aşmak için, daha yavaş ama derin analiz yapabilen "Düşünme (Reasoning) Modu"na geçerek projenin tamamlanmasını sağladık.

Sonuç
Yapay zeka bu projede harika işler çıkarmış olsada sürekli denetlenip yönlendirilmeye ihtiyacı var. Basit işleri bizim, ağır hesaplamaları yapay zekanın yaptığı ve hatalarını yine kendisine çözdürdüğümüz bu stratejiyle projeyi başarıyla tamamladık.

