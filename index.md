Tessera — Gizlilik Politikası ve Data Safety Taslağı
Durum: Milestone 1 taslağı (7 Kasım 2026). Bu metin hukuki danışmanlık değildir. Reklam, IAP, çökme raporlama veya bulut özellikleri eklenmeden önce yeniden denetlenmeli ve yayın öncesi son sürümle eşleştirilmelidir.

1. Kısa özet (mevcut 0.1.0 prototipi)
Tessera tamamen çevrimdışı çalışan bir bulmaca oyunudur. Mevcut prototip:

kişisel veri toplamaz,
hesap oluşturmaz,
reklam göstermez,
analitik veya çökme raporlama kullanmaz,
kullanıcılar arası sohbet, kullanıcı içeriği veya sosyal özellik içermez,
release yapısında ağ izni kullanmaz.
Oyun ilerlemesi ve ayarlar ilerleyen sürümlerde yalnızca cihazda saklanacaktır (shared_preferences/Hive). Cihazdaki veriler uygulama kaldırıldığında silinir.

Milestone 5'te reklam ve IAP eklendiğinde bu politika güncellenecek; EEA/UK için UMP onay akışı, audienceMode = families için çocuklara yönelik ayarlar ve Google Play Data Safety formu yeniden doldurulacaktır.

2. Gizlilik politikası taslağı (yayın metni için iskelet)
Veri sorumlusu / geliştirici: [ŞİRKET / GELİŞTİRİCİ ADI] İletişim: [DESTEK E-POSTASI] Yürürlük tarihi: [YAYIN TARİHİ]

2.1 Hangi verileri topluyoruz?
Mevcut sürümde hiçbir kişisel veri toplanmaz, sunucuya gönderilmez veya üçüncü taraflarla paylaşılmaz. Oyun tamamen çevrimdışı oynanır.

2.2 Cihazda saklanan veriler
İlerleyen sürümlerde aşağıdaki veriler yalnızca cihazda tutulabilir:

tamamlanan seviyeler ve koleksiyon durumu,
ses, titreşim, renk körü modu ve dil ayarları,
“reklamları kaldır” satın almasının yerel durumu.
Bu veriler reklam veya analitik amacıyla kullanılmaz. Uygulamayı kaldırmak yerel verileri siler.

2.3 Reklamlar (milestone 5 sonrası)
Reklamlar etkinleştirildiğinde Google AdMob kullanılabilir. AdMob; cihaz tanımlayıcıları, IP adresi, yaklaşık konum ve reklam etkileşimleri gibi verileri kendi politikalarına göre işleyebilir. EEA/UK kullanıcılarından UMP onayı alınır. families modunda:

çocuklara yönelik muamele bayrağı etkinleştirilir,
maksimum reklam içeriği derecesi G olur,
kişiselleştirilmiş reklamlar kapatılır.
“Reklamları kaldır” satın alması tek seferliktir ve Google Play tarafından işlenir; kart bilgileri geliştiriciye ulaşmaz.

2.4 Çocukların gizliliği
Oyun her yaş için uygundur; şiddet, kumar benzeri mekanik, loot box, sohbet ve kullanıcı içeriği yoktur. Mevcut sürüm hiçbir veri toplamadığı için çocuklardan bilerek veri toplama söz konusu değildir. Reklamlar etkinleştirildiğinde families modu varsayılan olacak ve Play Families politikalarına uyulacaktır.

2.5 Haklarınız
Mevcut sürümde sunucuda saklanan kişisel veri olmadığından erişim, düzeltme veya silme talebi uygulanacak bir veri kümesi bulunmaz. Yerel verileri temizlemek için uygulamayı kaldırabilir veya işletim sisteminin uygulama verisi temizleme aracını kullanabilirsiniz. Sorular için [DESTEK E-POSTASI].

2.6 Değişiklikler
Politika, yeni bir veri işleyen özellik eklenmeden önce güncellenir ve mağaza sayfasında yayımlanır.

3. Google Play Data Safety formu — mevcut build için taslak
Soru	Taslak yanıt
Uygulama veri topluyor mu?	Hayır
Uygulama veri paylaşıyor mu?	Hayır
Toplanan veri türleri	Yok
Veriler şifreli olarak iletilir mi?	Uygulanamaz (veri toplanmıyor)
Kullanıcı veri silmeyi talep edebilir mi?	Uygulanamaz; yerel veriler uygulama kaldırılınca silinir
Veriler üçüncü taraf reklam/analitik için kullanılıyor mu?	Hayır
Çocuklara yönelik mi?	Evet, tüm yaşlar; families modu hedefi
Önemli: Data Safety formu, kullanılan üçüncü taraf SDK'ların gerçek davranışına göre doldurulmalıdır. AdMob, IAP veya crash reporting eklendiğinde bu tablo geçersizdir; SDK sürümleri ve veri türleri yeniden denetlenmelidir.
