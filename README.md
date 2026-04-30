# SUNİ-UFUK
OSMAN, ÖMER, ÖZGÜR adlı kullanıcıların ortaya koydukları çalışma

Bu projeyi geliştirirken yazılım çözümlemesini oluşturmak için üç kişilik bir ekip olarak Google Gemini 3.1 Pro yapay zeka modelinden yoğun bir şekilde faydalandık. Ancak bu süreç, "kodu yazdırıp kopyalama" bölümünün ötesinde, iş bölümüne dayalı karmaşık bir yönetim gerektiriyordu.

Kullanılan AI Araçları, Amaçları ve İş Bölümü:
Projede dağıtılan görevleri yapay zeka ile kendi aramızda belirli bir stratejiye göre böldük. Renk paletlerinin (Magenta, Cyan vb.) ayarı, ekrandaki güç dağıtımları ve uçağı kontrol edecek yön tuşlarının (W, A, S, D ve ok tuşları) atanması gibi basit, temel ilerlemeleri kendi içimizde yönettik ve çalıştırdık. Yapay zekayı ise projenin "beyni" diyebileceğimiz karmaşık mühendislik ve matematik kısımlarında kullandık. Bazı uçak modelleri için (B737 MAX 8) aerodinamik sağlayan Vmo/Mmo Crossover (26.000 feet geçişleri) akımları, irtifaya bağlı dinamik Mach programlamaları, PID kontrolcüsü mantığıyla süzülmesi ve Suni Ufuk (ADI) yöntemiyle karmaşık "Gimbal Flip" (90 dereceyi geçince göstergenin ters dönmesi) trigonometrisi gibi zorlu kodları tamamen yapay zekaya yaptırdık. AI'dan aldığımız bu ağır çıktıları, kendi oluşturduğumuz tuş oranları ve renk şemalarıyla entegre ederek projeye uyarladık.

Yapay Zekanın Yetersiz Kaldığı Durumlar ve Sorun Yönetimi:
Yapay zeka, karmaşık algoritmaları kurmada inanılmaz derecede başarılı olsa da, projenin hacmi büyüdükçe çok ciddi "Bağlam Unutkanlığı" (Bağlam Bozulması) sorunları başladı. Yapay zeka ile yaşadığımız en büyük problemler ve yetersizlikleri şu şekilde özetleyebiliriz:

Eski Özellikleri Bozma ve Unutkanlık: Yapay zekadan yeni bir kod bloğu (göstergenin köşesine V/M etiketi) eklemesini istediğimizde, daha önce kusursuz çalışan eski özellikleri bozmaya başladığını fark ettik. Örneğin; havacılık şartlarının gerekliliği olan sola yatış (sol ok tuşu) durumunda ufuk çizgisinin sağa doğru devrilmesi kuralını koda işlemiştik. Ancak AI, her yeni özellik eklemesinde bu kuralı unutup yön tuşlarının mantığını standart bir oyun gibi sıfırlayarak sola basınca ufkun da sola yatmasına sebep oldu. Defalarca "sola basınca ufuk sağa dönecek, bu kuralı bozma" şeklinde müdahale etmek zorunda kaldık.

Görsel İkazların Kaybolması: GPWS (Yer Yakınlık İkaz Sistemi) için ekranın altında yanıp sönen turuncu bir "TERRAIN" yazısı ekletmiştik. Projeye "Pull Up" okunu dahil etmek için AI'dan kodu güncellemesini isterken, bu sefer de Terrain yazısını koddan tamamen sildiğini gördük. İstekler detaylandıkça yapay zekanın tüm özellikleri aynı anda akılda tutma kapasitesi ciddi şekilde düştü.

Sentaks (Sözdizimi) ve Dikkatsizlik Hataları: Yapay zeka zaman zaman parantezleri kapatmayı unuttu veya değişken isimlerinde büyük/küçük harf hataları yaptı (Örneğin tanımlı YESIL değişkeni yerine kodun ortasında dalgınlıkla YESil yazması gibi). Bu tür hatalar Python'un NameError veya SyntaxError verip çökmesine neden oldu. Bu noktada kodu satır satır okuyup hata taramak yerine, farklı bir yöntem izledik: Terminaldeki hatayı kopyalayıp yapay zekaya geri verdik. Yani, kendi yazdığı hatalı kodu yine yapay zekanın kendisine incelettirerek "Bu hatayı bul ve düzelt" komutuyla hata ayıklama (debug) işlemini ona yaptırdık.

Kapasite Aşımı ve Çökme: Proje 500 satıra yaklaştığında, iç içe geçmiş maskelemeler ve hiyerarşik uyarı sistemleri eklendiğinde, standart Pro modelinin işlem kapasitesi tıkandı. Yapay zeka çok fazla kod dizimi isteyince artık cevap veremez hale geldi, yanıtları yarıda kesildi veya tamamen dondu. Projeyi tamamlayabilmek için standart modelden ayrılıp, daha yavaş çalışan ama çok daha derin analiz yapabilen "Düşünen Moda" (Akıl Yürütme/Düşünme Modu) geçmek zorunda kaldık. Bu mod sayesinde kodun tamamı çökmeden çıktı olarak alınabildi.

Sonuç olarak; Yapay zeka bu projede muazzam bir mühendislik motoru görevi görse de, kendi başına bırakılamayacak kadar dikkatsiz bir yapıda olduğunu gösterdi. Üç kişilik ekibimizle basit işleri kendi aramızda halledip, ağır işleri ona devrederek ve yaptığı hataları tekrar kendisine denetleterek projeyi başarılı bir şekilde tamamlayabildik.

