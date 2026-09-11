# MENTORIA — DIŞ GÖRÜŞ İŞLEME VE KARAR AYRIMI v0.1

**Kayıt:** K-756 · **Tarih:** 11.09.2026 · **Durum:** DIŞ GÖRÜŞ ALINDI / yerel ön doğrulama yapıldı / uygulama YOK.
**Kaynak:** Ürün sahibinin bu oturumda ilettiği dış değerlendirme metni. Aşağıdaki öneri tabloları bu metnin kayıt-ID'leri korunmuş işleme özetidir; dış görüşün kelimesi kelimesine ham transkripti değildir. Ajan teyitleri dış değerlendirmeci görüşünden ayrıca ayrılmıştır.
**Değerlendirilen paket:** v0.1 MENTORIA-LEX / MENTORIA-SED briefi; Protokol v1.2 + Sözlük v1.6. Brief, inceleme tabanı olarak bu tur değiştirilmedi.

## 1. Alınan sonuç ve sınır

- Dış değerlendirmeci iki ürünün kapsamını ayrı kabul etmiş: **LEXIVA MENTORIA v2.11.2** için KORU ağırlıklı/sınırlı REVİZE; **SEDUVA MENTORIA v1.5.5** için KORU + daha yoğun REVİZE/kaynak doğrulaması.
- LEX: resmî sonuç aktarımı + özgün telemetri + uzman yorumu. SED: dış ölçek/puan/kılavuz kesmesi + ürün kaydı/hesaplaması + uzman yorumu/rapor kararı. Ortak ilkeler mümkündür; veri modeli ve ekran dili tekleştirilmez.
- Kapsam kabulü, her görünür durumun incelendiğini veya hesaplamaların doğrulandığını göstermez. Brief regex-aday havuzu taşır; bu inceleme tüm ürün için YEŞİL kabul testi değildir.
- Dış metnin sonundaki “DIŞ GÖRÜŞ İÇİN HAZIR” ifadesi ileri bir gönderim emri değil, iletilmiş görüşün kendi kapanış ifadesidir. Yerel durum artık **DIŞ GÖRÜŞ ALINDI / UYGULAMA KARARI BEKLİYOR**.
- YAZ/GİZLE/KORU/REVİZE dış önerilerdir. GİZLE dahil hiçbir öneri uygulanmadı; yeni sözlük/protokol/ürün sürümü oluşturulmadı.
- Dış metin teknik kaynak kontrolü yaptığını bildiriyor; iletilen yanıtta URL, sayfa ve sürüm künyeleri bulunmuyor. Pearson/SDQ/diğer araçlar için bunlar bu tur bağımsız doğrulanmış kabul edilmedi. Vanderbilt'in önceki K-754 kanıtları kendi kapsam ve sürüm sınırıyla saklıdır; tekrar inceleme açılmadı.

## 2. Yerel olarak doğrulanan kanon açıkları

### KANON-M7 — gerçek metin uyuşmazlığı; iki kullanım

- Protokol v1.2 **satır 81 / §6 M-7**: `Burada puan yok. Nasıl yaptığını birlikte göreceğiz.`; eski `Seni dününden iyi tanıyorsun` ifadesinin kaldırıldığı yazılı.
- Sözlük v1.6 **satır 112 / §3-H Dürüst-not**: eski tam cümle hâlâ var.
- Sözlük v1.6 **satır 117 / Yolculuk Yıldızı açıklaması**: aynı eski cümle ikinci kez var.

**Hüküm:** Sözlükte iki aktif kullanım Protokol M-7 ile uyuşmuyor. Önerilen en küçük düzeltme, iki alıntının da mevcut Protokol cümlesine hizalanmasıdır; yeni ifade veya yeni dil sistemi icat edilmez. **Bu tur uygulanmadı.** Bunun çocuk ürünlerine geri sızdığı veya çocuk yüzeyi yeniden bozulduğu sonucu çıkarılmadı; tespit belge katmanındadır.

### KANON-NAV — K-709 kararı ile sözlük §3-D eski ad kaydı

- Sözlük v1.6 **satır 86 / §3-D**: `Guidance Navigator (Mentoria)`.
- Strateji Karar Defteri **K-709**: sahibin onaylı adı **Klinik Rehber**; yanlış ajan adı `Vaka Yönlendirici` geri alınmış.
- İki ürünün `src/components/Kabuk.tsx` menülerinde `navigator` = **Klinik Rehber**.

**Hüküm:** Mevcut ürünü geri adlandırmak yok. Öneri, sözlükte ilgili kaydı K-709 ile hizalayan küçük bir düzeltme/şerh için ayrı sahip kararıdır. §3-D'nin tamamını topluca yeniden adlandırmak kapsam dışıdır.

**Önemli ayrım:** `Uzman Masası` açılış ekranı, `Klinik Rehber` ise ayrı `navigator` alt ekranıdır. Protokol §1 ile bu iki ekranın ayrı ad taşıması kendi başına çelişki DEĞİLDİR. LEX'in ayrı Kurum menüsü ve SED'in kurum ekranını Uzman Masası olarak sunması K-709 bağlamıyla okunur.

## 3. Dış görüşün kayda alınırken düzeltilmesi gereken atıf/bağlam noktaları

1. **LEX-117 yanlış terimle özetlenmiş.** Briefte gerçek ifade `... Oİ/GT hesaplanır.`; dış görüşte `FSI/TB hesaplanır` diye yazılmış. LEX-117 üzerinden FSI/TB gizleme işlemi çıkarılamaz. Bununla birlikte LEX havuzunda **LEX-176/177** FSI/TB/G_growth kayıtları var; yerel `NavigatorPaneli.tsx` içinde Oİ/GT ile FSI/TB'nin birlikte bulunması ayrı, konumlu tutarlılık adayıdır.
2. **“Tanım yok” ile “pakette yeterli dayanak görünmüyor” aynı şey değil.** SED `src/data/navigator.ts:3–5` FSI/TB/G_growth tanımlarını ve PRD/K-537 bağını; LEX eş dosya `:3–5` Oİ/GT/G_growth tanımlarını içeriyor. Strateji Defteri K-537, TB ve G_growth ad kararını kaydediyor. Bunlar hesabın bilimsel/işlevsel doğrulaması DEĞİLDİR; fakat yeniden metrik tanımı icat etmeden önce mevcut dayanak okunmalıdır.
3. **Norm Şeması yalnız SED'de değil.** Aynı başlık LEX havuzunda **LEX-186**, SED'de **SED-212**; her iki `components/izleme/IzlemePaneli.tsx:102` içinde var. İki ürün için ayrı aday kaydı gerekir; otomatik ortak düzeltme yapılmaz. Eşik/kılavuz kategorisi ile istatistik normu aynı şey sayılmaz.
4. **SED-577 mevcut çekinceyi de içeriyor:** `✅ Üçgen tamam — yorum yapılabilir (tek başına yeterli değil, trend gerekir).` Dış görüşteki kısa alıntı çekinceyi dışarıda bırakıyor. “Yorum yapılabilir” ifadesi hâlâ incelenebilir; “hiç sınır yok” diye sınıflanamaz. LEX-544 aynı ifadeyi taşıyor.
5. **LEX-451 parçalı çıkarımdır.** Gerçek havuz satırı `olarak raporlanır — klinik etki DEĞİL ...` diye başlıyor; etkililik ifadesinin tam cümlesi `components/rapor/RaporAtolyesi.tsx:110` bağlamında mevcut. Parçayı bağımsız ürün cümlesi olarak yeniden yazmak yok.
6. Bazı dış görüş alıntıları İngilizce özetlenmiş (ör. LEX-120/206/207/502). Briefte bunların Türkçe metinleri bulunuyor; İngilizce özet, üründe İngilizce UI hatası kanıtı sayılmaz.
7. Aralıkla verilen atıflar tek bir kavramın tüm örnekleri değildir. Örneğin SED-216–225 içindeki her kayıt indeks adı değildir. Her ürün konumunda özgün metin ve alıcı rolü tek tek okunmalı; aralık bir toplu değiştir komutu değildir.

## 4. Ayrı iş sınıfları ve işlem sınırı

| Sınıf | İçerik | Şimdiki işlem |
|---|---|---|
| Kanon tutarlılığı | KANON-M7, KANON-NAV | Doğrulanmış açık kayıt; ayrı minimum-düzeltme önerisi, uygulama onayı yok |
| LEX editoryal | Etkililik ifadesi, clinic, batarya puanlaması, öneri/yorum sahibi | Kaynak konumu + tam önce/sonra/adet + dayanak tablosu hazırlanmalı; henüz dönüşüm listesi onaylanmadı |
| SED editoryal | Kılavuz açıklaması/uzman yorumu, değerlendirir, öneri güçlenir, teknik/koçluk rolü, norm/eşik başlığı | Aynı yöntem; LEX'e otomatik taşıma yok |
| Hesaplama/kaynak | SDQ, metrikler, eşik şeması, yüzdeler, T-skoru, FSIQ/g, diğer dış araçlar, entegrasyon beyanları | Doğrulama adayı; kaynak/kod bağımlılığı. Metin rötuşuyla kapanmaz; bu tur yeni teknik inceleme açılmadı |
| Vanderbilt | Adlandırma + mevcut C-M1/V-1…V-5 | **Mevcut VANDERBILT-DUZELTME kuyruğuyla ilişkilendirildi**; mükerrer iş yok, sıraya öne alınmadı |
| KORU önerileri | Teknik terimler, TASLAK, insan onayı, test uygulamaz, birey-içi trend, telif | Mevcut metni bozma; dış KORU önerisi ilgili işlevin bağımsız test edildiği anlamına gelmez |
| SCHOLARIA / SUPPORTA | İki ürün için ayrı paketler ve ham kaynak/rol/ekran/rapor/ölçüm bağlamları | Materyal gereksinimi kaydedildi; MENTORIA'dan nihai dil kararı devredilmez; paket üretimi bu tur açılmadı |

**Önerilen sonraki adım:** Önce iki kanon açığı ile iki ürünün editoryal adaylarını, birbirine karıştırmadan, kaynaklı **ÖNCE → SONRA → ADET → DAYANAK** kararcığına çevirmek. Sahip onayından önce kod/sözlük/protokol yazımı yok. Hesaplama işleri ayrı kalır. Minimum düzeltme sonrası mevcut ürün sürümleri korunur; yeni mühür yine ayrı onay gerektirir.

## 5. Dış görüş öneri kayıtları — iki ayrı ürün

Bu tablolar dış görüşün karar satırlarını muhafaza eder; “Yerel sınıf” ajan yönlendirmesidir. Her aralıkta tüm brief ID'lerinin varlığı kontrol edildi. Tam örnek metinler Ek A'da brief ID'leriyle bulunur. Sayılar benzersiz hata veya tüm UI taraması sayısı değildir; yalnız dış görüşün gruplanmış öneri satırı sayılarıdır.

### MENTORIA-LEX — 32 öneri satırı

| Brief referansı | Dış görüş önerisi | Gerekçe özeti | Yerel sınıf |
|---|---|---|---|
| LEX-015 | REVİZE | Etkililik iddiası ile izlem/trend ayrımı | EDITORYAL |
| LEX-026 | KORU* | K-709; sözlükte eski ad ayrıca raporlansın | KANON |
| LEX-033 | KORU | Test uygulamaz sınırı | KORU |
| LEX-041 | KORU | Uzman yorumu ve TASLAK | KORU |
| LEX-049 | KORU | Özgün telemetri ve norm/akran karşılaştırması ayrımı | KORU |
| LEX-074 | KORU / kaynak doğrulaması | ASİS dış araç adı | KAYNAK |
| LEX-100 | KORU | Bant/eşik uzman yüzeyinde; kaynak açıklığı | BAGLAM |
| LEX-102 | KORU | Yorum üretmez, trend izler | BAGLAM |
| LEX-108 | KORU | Betimleyici eksen, norm yok | KORU |
| LEX-117 | GİZLE / KANIT GEREKLİ | Dış görüş FSI/TB diye alıntılıyor; gerçek satır Oİ/GT | ATIF-DUZELTME |
| LEX-120 | KORU | Resmî sonuçların aktarımı | KORU |
| LEX-145 | REVİZE | Eğitimsel etkililik ifadesi | EDITORYAL |
| LEX-206 | KORU | 6 haftalık plan ve eğitimsel gelişim raporu | KORU |
| LEX-207 | KORU | Uzman yorumu; dış görüşte özetlenmiş | KORU |
| LEX-231–240 | KORU | Dış araç/resmî sonuç/değişim takibi | BAGLAM |
| LEX-259 | KORU | Kendi zaman serisi | KORU |
| LEX-306 | KORU | Otomatik norm yorumu yok, yorum uzmanda | KORU |
| LEX-319 | KORU / kaynak doğrulaması | PREDYS dış araç adı/sürümü | KAYNAK |
| LEX-320–328 | KORU | Performans/rapor/uzman yorumu; ölçüm bağlamı | BAGLAM |
| LEX-334 | KORU | Nesnel sistem verisi seçimi | KORU |
| LEX-335–337 | KORU | Resmî sonuç + telemetri ayrımı | KORU |
| LEX-369 | KORU / hesaplama doğrulaması | Tepki yüzdesinin pay/payda/gözlem birimi | HESAPLAMA |
| LEX-451 | REVİZE | Etkililik değerlendirmesi; gerçek kayıt cümle parçasıdır | BAGLAM |
| LEX-462 | KORU | Tanı koymaz/ilaç önermez | KORU |
| LEX-464 | KORU | Trenddir, tanı değildir | KORU |
| LEX-467 | REVİZE / kaynak doğrulaması | Puanlamayı batarya yapar; rol/veri sorumluluğu | EDITORYAL+KANIT |
| LEX-478 | REVİZE | Uzman-clinic adlandırması | EDITORYAL |
| LEX-482 | KORU | Çocuk ölçümü değil, uzman notu | KORU |
| LEX-493–498 | KORU / bağlam gerekli | Ölçüm kanıtı/öneri düzeyi | BAGLAM |
| LEX-502 | KORU / kaynak adı doğrulaması | Öğrenme Güçlüğü Tanılama Testi dış araç adı | KAYNAK |
| LEX-531–532 | KORU | Dış araçlar ve eğitimsel değişim | BAGLAM |
| LEX-535–544 | KORU / bağlam doğrulaması | Rapor/üçgen/trend; yorum yeterliliği koşulu | BAGLAM |

### MENTORIA-SED — 54 öneri satırı

| Brief referansı | Dış görüş önerisi | Gerekçe özeti | Yerel sınıf |
|---|---|---|---|
| SED-032 | KORU* | K-709; sözlükte eski ad | KANON |
| SED-033 | REVİZE | Kılavuz bilgisi ile sistem açıklaması ayrımı | EDITORYAL+KANIT |
| SED-039 | KORU | TASLAK ve uzman onayı | KORU |
| SED-042 | KORU | Uzman notu | KORU |
| SED-048 | KORU | Uzman sorumluluğu | KORU |
| SED-075 | KORU / kaynak doğrulaması | ADHD-RS-5 dış araç | KAYNAK |
| SED-105 | KORU / kaynak doğrulaması | BASC-3 dış araç | KAYNAK |
| SED-111 | KORU / kaynak doğrulaması | BRIEF-2 dış araç | KAYNAK |
| SED-124 | YAZ / KANIT GEREKLİ | FSI/TB tanım ve hesaplama bağlantısı | HESAPLAMA |
| SED-127 | KORU | Yetkin uygulayıcı ve dış hesaplama sorumluluğu | KORU |
| SED-137/138 | KORU / kaynak doğrulaması | Conners sürümleri | KAYNAK |
| SED-140–143 | REVİZE | DEHB koçluk/mentörlük rol sınırı | EDITORYAL+KANIT |
| SED-144 | KORU / kaynak doğrulaması | DSM-IV araç adı | KAYNAK |
| SED-149 | KORU | Veri akışı beyanı; teknik doğrulama ayrı | BAGLAM |
| SED-150 | REVİZE | Değerlendirir ifadesinde puan kaydı/yorum ayrımı | EDITORYAL+KANIT |
| SED-162 | KORU | Akran karşılaştırması yok | KORU |
| SED-163 | KORU | Birleşik taslak rapor | KORU |
| SED-184 | REVİZE | Öneri güçlenir: otomatik karar izlenimi | EDITORYAL+KANIT |
| SED-195 | REVİZE | CBT/PCIT atfı ve terapi uygulaması izlenimi | EDITORYAL+KANIT |
| SED-203–204 | YAZ / KANIT GEREKLİ | FSI/TB/G_growth tanım ve hesaplama | HESAPLAMA |
| SED-212 | REVİZE | Norm sözcüğü ve normsuzluk gerilimi | EDITORYAL+KANIT |
| SED-214 | HESAPLAMA + KAYNAK DOĞRULAMASI | Ortalama puan → kategori | HESAPLAMA |
| SED-216–225 | KORU / kaynak doğrulaması | Dış araç indeksleri; aralıktaki her satır aynı tip değil | BAGLAM |
| SED-217 | KORU / REVİZE AD KONTROLÜ | FSIQ ile g ayrımı | KAYNAK |
| SED-251 | KORU | Ölçek seçimi/puan girişi | KORU |
| SED-287 | HESAPLAMA DOĞRULAMASI | Otomatik kategori; şerh algoritmayı doğrulamaz | HESAPLAMA |
| SED-305 | REVİZE / KAYNAK DOĞRULAMASI | Vanderbilt adı, ürün tanı diliyle ayrım | VANDERBILT |
| SED-318 | KORU | Otomatik norm yorumu yok | KORU |
| SED-319 | HESAPLAMA DOĞRULAMASI | Kategori ile norm yorumu ayrımı | HESAPLAMA |
| SED-335–348 | KORU / bağlam kontrolü | Performans/puan/uzman yorumu | BAGLAM |
| SED-342 | KORU | Profesyonel uzman yorumu | KORU |
| SED-347 | KORU | Puan özeti ve yorum sorumluluğu | KORU |
| SED-351 | KORU | Rapor taslağı/uzman onayı | KORU |
| SED-360–363 | HESAPLAMA/KAYNAK DOĞRULAMASI | SDQ form/yaş/sürüm/kesme | HESAPLAMA |
| SED-400 | KORU / kaynak doğrulaması | SNAP dış araç adı | KAYNAK |
| SED-408 | HESAPLAMA DOĞRULAMASI | Tepki yüzdesi formülü | HESAPLAMA |
| SED-409 | KORU / kaynak doğrulaması | T-skorunun ait olduğu araç | KAYNAK |
| SED-422 | KORU | Tarama pozitifliği ≠ tanı | KORU |
| SED-443–447 | HESAPLAMA + KAYNAK DOĞRULAMASI | Vanderbilt belirti/performans koşulları | VANDERBILT |
| SED-450–453 | KORU / kaynak doğrulaması | WISC dış araç adları | KAYNAK |
| SED-454 | KORU / kaynak doğrulaması | WFIRS-P dış araç | KAYNAK |
| SED-459–460 | KORU | Otomatik öneri yok; uzman seçer | KORU |
| SED-473–476 | KORU | BEP yazmaz, kanıt üretir | KORU |
| SED-503 | KORU | Tanı koymaz/ilaç önermez | KORU |
| SED-505 | KORU | Trenddir, tanı değildir | KORU |
| SED-507 | REVİZE / KANIT GEREKLİ | Batarya puanlaması sorumluluğu | EDITORYAL+KANIT |
| SED-518 | KORU / kaynak doğrulaması | WMI araç bağlamı | KAYNAK |
| SED-535 | KORU | Ölçek maddeleri üründe yok | KORU |
| SED-536–537 | KORU | Ölçme kanıtı terimi | BAGLAM |
| SED-540–541 | REVİZE / KANIT GEREKLİ | Önerinin sahibi sistem mi uzman mı | EDITORYAL+KANIT |
| SED-556 | KORU | Lisans uyarısı | KORU |
| SED-564 | REVİZE | Gelişimsel Eşik bağlamı | EDITORYAL+KANIT |
| SED-575 | KORU / kaynak doğrulaması | Süreler ürün kuralı mı bilimsel eşik mi | KAYNAK |
| SED-577 | REVİZE | Üçgen tamam/yorum yapılabilir; mevcut çekince korunarak okunmalı | EDITORYAL+KANIT |

## 6. Ortak ilkelerin kabul kaydı (uygulama değil)

Dış araç adı ürünün kendi iddiası değildir; ölçek puanı/sistem çıktısı/uzman yorumu/otomatik karar ayrı tutulur. Tanı koymaz şerhi çevresindeki iddiaları kendiliğinden doğrulamaz. Norm/kesme kaynağı ve sürümü belirtilmelidir; birey-içi trend akran/norm karşılaştırması değildir. TASLAK rapor uzman onayı gerektirir. Teknik yetişkin dili korunabilir; çocuk M-3 listesi yetişkine körlemesine uygulanmaz. Klinik Rehber mevcut ad olarak korunur; kanon uyumu ayrı ele alınır. Yeni sözlük/protokol/ürün sürümü otomatik üretilmez.

## 7. Sonraki paketlerin talep edilen materyalleri

**SCHOLARIA-LEX ve SCHOLARIA-SED ayrı:** mevcut sürüm; App/kabuk/menü; öğretmen panel/kart bileşenleri; 232/230 havuzun ham kaynak bağlamı; metin–ekran–rol–alıcı eşlemesi; öğretmen rapor örnekleri; gerçek metrik ekranları; varsa dış araç kaynak/sürümü; mevcut dil kararları.

**SUPPORTA-LEX ve SUPPORTA-SED ayrı:** mevcut sürüm; App/kabuk; destek/eğitmen paneli; 289/288 havuzun ham kaynak bağlamı; rol tanımı; öneri/yönlendirme/ölçüm/rapor ekranları; tekniklerin kaynakları; mevcut dil kararları. MENTORIA uzman dili diğer roller için otomatik standart değildir.

## 8. İz ve koruma

- Değerlendirilen brief SHA-256: `6b2fbcd79ea8740eb694cc3f2836951d89745992db9f1048b00a0756f25d8b8d`; brief bu tur değişmedi.
- `VAMOLA-STRATEJIK-HIZALAMA-VE-DIL-PROTOKOLU_v1.2.md` SHA-256: `e9336cc78dcd45ca8eb3914be601003f7efb7cc6502522794affcc03dc2c3455`; bu tur değişmedi.
- `VAMOLA-KANONIK-TERIM-SOZLUGU_v1.6.md` SHA-256: `cce22ec321ace3aacd093b221fb75968aa2862d5b07b3f2816f9ee52a890c9ba`; bu tur değişmedi.
- Ürün sürümleri LEX 2.11.2 / SED 1.5.5; kaynak/HTML/hesaplama değiştirilmedi. Yeni mühür kurulmadı.

## Ek A — Görüşte atıf verilen gerçek brief kayıtları

Aşağıdaki kayıtlar kaynak kod satırı değildir; önceki briefin kimlik alanları açılmış aday havuzundan alınmıştır. Dış görüşteki kısaltmaların/çevirilerin yerine bu metin esas alınır; nihai işlemde ham kaynak konumu ayrıca gerekir.

```text
LEX-015	Değişim “eğitimsel etkililik / öğrenme çıktısı” olarak raporlanır — klinik etki DEĞİL.
LEX-026	Klinik Rehber
LEX-033	Uygulama test UYGULAMAZ ([REF])
LEX-041	([REF]); uzman yorumu esastır, rapor TASLAK mührüyle verilir.
LEX-049	+ uygulama içi özgün telemetriyi sunar. Norm/akran karşılaştırması üretilmez (Z-15).
LEX-074	ASİS (Anadolu-Sak Zekâ Ölçeği)
LEX-100	Bant/eşik yalnız uzman ekranındadır
LEX-102	Bağlam kaydı + pasif gözlem + izlem eşikleri — yorum üretmez, trend izler ([REF]).
LEX-108	Betimleyici eksen; norm karşılaştırması YOK (Z-15)
LEX-117	Bu danışan için Klinik Rehber verisi yok. Bağlam Kaydı + DRC + oturum girdisi birikince Oİ/GT hesaplanır.
LEX-120	Bu modül; resmî sonuçların (RAM raporu, Öğrenme Güçlüğü Tanılama Testi, BEP) vaka dosyasına
LEX-145	Değişim (eğitimsel etkililik)
LEX-176	FSI/TB/G_growth
LEX-177	FSI/TB/G_growth + Bağlam Kaydı özeti + DRC 9/14 — güçlü yön dahil
LEX-186	Gelişimsel Eşik Norm Şeması — eşik bilgisi
LEX-206	Güçlü yönler (D-L7) + 6 haftalık izleme planı + eğitimsel gelişim raporu (7 başlık) — TASLAK
LEX-207	H1-H3 telemetrisi birlikte okunur: hata sınıfı trendi + iskele kullanımı; support fading planı (yorum uzmanda — [REF])
LEX-231	[REF] dili: “oyun-temelli danışma oturumu” — tanı/tedavi iddiası yok, ürün=sahada değer katmanı
LEX-232	[REF] · Ölçüm Dürüstlüğü
LEX-233	[REF] Ölçüm Dürüstlüğü: uygulama test/tarama UYGULAMAZ — resmî sonuçlar içe aktarılır; değişim "eğitimsel etkililik / öğrenme çıktısı" dili
LEX-234	[REF] kilit: gerçek pilot etik kurul sonrası — bu sürüm veri toplamaz.
LEX-235	[REF]: tek gün/tek ortam verisiyle genelleme yasağı — Bağlam Kaydı+okul+seans üçlüsü
LEX-236	[REF]: tek kaynağa dayalı çıkarım yasak — Bağlam Kaydı + gözlem + oturum girdisi üçlüsü.
LEX-237	KVKK Kurum Politikası
LEX-238	KVKK kurum politikası, şube/uzman yönetimi, yetkilendirme matrisi, kurum mührü. Veri girişi yapmaz.
LEX-239	KVKK kurum: yerel-önce, maskeli UID (ÖĞR-xxxx), need-to-know (şube/uzman), veli onamı, 2 yıl saklama
LEX-240	KVKK: yedek şifreli saklanır, 2 yıl saklama, tenant bazlı.
LEX-259	Kesintisiz odak süresi metriği — “12 → 18 dk” ilerleme dili (Z-9) — kendi zaman serisi, akran karşılaştırması yok
LEX-306	Otomatik norm yorumu yapılmaz — puan yorumu uzmanın sorumluluğundadır. Madde/yönerge/norm tablosu sistemde yok.
LEX-319	PREDYS (RAM genel tarama)
LEX-320	Performans +/-
LEX-321	Performans:
LEX-322	Planlandı
LEX-323	Profesyonel Rapor Üretici (MENTORIA-LEX)
LEX-324	Profesyonel Uzman Yorumu
LEX-325	Program
LEX-326	Program — 2021 DEP Modül Hiza (seçmeli)
LEX-327	Puan özeti (serbest metin, norm yorumu uzmanındır)
LEX-328	Puan özeti:
LEX-334	Raporda görünmesini istediğiniz nesnel sistem verilerini seçin.
LEX-335	Resmî Sonuçlar + Telemetri
LEX-336	Resmî Sonuçlar + Telemetri (Katman 1 & 2)
LEX-337	Resmî Sonuçlar + Telemetri panosundan en az 1 hafta özeti girince çizgi burada oluşur. Akranla karşılaştırma yoktur (Z-15).
LEX-369	Sıklık temelli nokta matrisi, tepki yüzdesi = (tepki/gözlem)×100 — gözlemlenebilir+sayılabilir+bağlamlı
LEX-451	olarak raporlanır — klinik etki DEĞİL (LX-10 §6). Rapor TASLAK mührü taşır; uzman notu boş bırakılır ([REF]).
LEX-462	tanı koymaz, ilaç önermez
LEX-464	trenddir, tanı değildir
LEX-467	verir; puanlamayı batarya yapar. Tek ölçümle karar yok — trend gerekir.
LEX-478	Çekirdek hiza: 3.1 ardıl sıra; sesletim bölümü uzman-clinic alanı (demo dışı).
LEX-482	Çocuk-ölçümü DEĞİLDİR: uzmanın kendi seans-sonu notudur ([REF]). Yalnız-yerel ([REF]).
LEX-493	Ölçme Kanıtı
LEX-494	Ölçme kanıtı:
LEX-495	Ön-görüşme (T0) — Tanışma, Güçlü Yönler ve Vaka Başlangıcı
LEX-496	Önceki 14 gün vs son 14 gün — kendi serisi, akran karşılaştırması yok ([REF]/Z-9).
LEX-497	Öneri düzeyi:
LEX-498	Öneri: Rutin Kartı
LEX-502	Öğrenme Güçlüğü Tanılama Testi
LEX-531	— resmî araçlar eğitimli uygulayıcı tarafından dışarıda uygulanır; değişim "eğitimsel etkililik / öğrenme çıktısı" olarak izlenir.
LEX-532	— çocuk-veli ekranında YOK ([REF]/D1). Uyum dönemi (H1-H2) ayrı yorumlanır; tek oturumla genelleme YOK; sistem öneri ÜRETMEZ.
LEX-535	① Telemetri Özeti (Katman 1 — LEXIVA özgün)
LEX-536	① İzlem Süresi + Oturum Sürekliliği
LEX-537	② Mevcut Düzey (eksen bazlı özet — bantlar yalnız bu raporda, uzmana)
LEX-538	② Resmî Sonuçlar (Katman 2 — içe aktarım; uygulama test UYGULAMAZ)
LEX-539	③ Güçlü Yönler (D-L7 üçlüsü)
LEX-540	④ Destek Alanları + Hata Sınıfı Dağılımı
LEX-541	⑤ Veli İşaretlemeleri (M-4 akıcılık)
LEX-542	⑥ BEP Kanıt Özeti Bağlantısı
LEX-543	⑦ Uzman Notu (yorum uzmanda — sistem öneri üretmez)
LEX-544	✅ Üçgen tamam — yorum yapılabilir (tek başına yeterli değil, trend gerekir).
SED-032	Klinik Rehber
SED-033	Kılavuz Yorumu
SED-039	TASLAK — [REF] · Uzman onayı olmadan geçerli belge değildir
SED-042	Uzman Notu (boş — uzman doldurur [REF]):
SED-048	([REF]); uzman yorumu esastır, rapor TASLAK mührüyle verilir.
SED-075	ADHD Rating Scale - 5
SED-105	BASC-3
SED-111	Behavior Rating Inventory of Executive Function - Second Edition
SED-124	Bu danışan için Klinik Rehber verisi yok. Bağlam Kaydı + DRC + oturum girdisi birikince FSI/TB hesaplanır.
SED-127	Bu ölçek için yetkin uygulayıcı lisansım/erişimim var ve puanları kılavuzuma göre hesapladım (C-2).
SED-137	Conners 3rd Edition
SED-138	Conners 4th Edition
SED-140	DEHB Koçluk — Odak Ritüeli
SED-141	DEHB Koçluk/Mentörlük
SED-142	DEHB Mentörlük — Planlama ve Organizasyon
SED-143	DEHB odağı: yürütücü işlev çantası, BGM-12 ile karışmaz.
SED-144	DSM-IV’e Dayalı Yıkıcı Davranış Bozuklukları Derecelendirme Ölçeği
SED-149	Danışan kodu maskelidir (KVKK). Veli onamıyla PERSONA (çocuk/veli ürünü)/SCHOLARIA (öğretmen ürünü) verisi buraya akar (need-to-know).
SED-150	Danışan takibi, batarya puan girişi, rapor TASLAK üretir; lisanslı ölçekte beyan + C-2 doğrulanmışsa değerlendirir.
SED-162	Değerlendirme Ölçekleri’nden en az 1 kayıt girince çizgi burada oluşur. Akranla karşılaştırma yoktur.
SED-163	Değerlendirme Ölçekleri’nden kayıt ekleyin; sonra burada birleşik rapor üretebilirsiniz.
SED-184	Ebeveyn / öğretmen / danışman — her biri 0-3. Uyum yüksekse öneri güçlenir; düşükse kaynak/ortam gözden geçirilir (Z-12).
SED-195	Etkinliksiz ödev yok · Uyum ödüllendirilir (CBT/PCIT) · ≤10 dk
SED-203	FSI/TB/G_growth
SED-204	FSI/TB/G_growth + Bağlam Kaydı özeti + DRC 9/14 — güçlü yön dahil
SED-212	Gelişimsel Eşik Norm Şeması — eşik bilgisi
SED-214	Gelişimsel Eşik Şeması: ort. puan → kategori, tek ölçümle karar yok, trend gerekir
SED-216	Genel Yetenek (GAI) - ek
SED-217	Genel Zeka (FSIQ - g)
SED-218	Genelle
SED-219	Genelleme
SED-220	Genelleme ve kural
SED-221	Gerek
SED-222	Girdi (etkinlik-bağlı)
SED-223	Global Executive Composite (GEC)
SED-224	Global Index
SED-225	Görsel-Mekansal (VSI)
SED-251	Henüz ölçüm yok — yukarıdan bir ölçek seçip puan girin.
SED-287	Kılavuz kesmesine göre otomatik kategori; tanı yerine geçmez. Ölçek formu MENTORIA-SED’da bulunmaz.
SED-305	NICHQ Vanderbilt ADHD Tanı Ölçeği
SED-318	Otomatik norm yorumu yapılmaz — puan yorumu uzmanın sorumluluğundadır. Madde/yönerge/norm tablosu sistemde yok.
SED-319	Otomatik sınıflandırma kılavuz kesmesine göredir; tanı yerine geçmez.
SED-335	Performans (işlevsellik)
SED-336	Performans +/-
SED-337	Performans:
SED-338	Plan/Organize
SED-339	Planla
SED-340	Planlandı
SED-341	Profesyonel Rapor Üretici (MENTORIA-SED)
SED-342	Profesyonel Uzman Yorumu
SED-343	Program
SED-344	Program — 12 Modüllük Sarmal (seçmeli)
SED-345	Prososyal (Güçlü Yön)
SED-346	Psikomotor / Dikkat-Odak
SED-347	Puan özeti (serbest metin, norm yorumu uzmanındır)
SED-348	Puan özeti:
SED-351	Randevu tek başına belge değildir; rapor taslaktır ve uzman onayı gerekir. Gözlemlenebilir dil kullanılır.
SED-360	SDQ Hiperaktivite ebeveyn kılavuzuna göre Klinik (7-10) düzey olarak tanımlanmaktadır.
SED-361	SDQ Hiperaktivite ebeveyn kılavuzuna göre Normal (0-5) düzey olarak tanımlanmaktadır.
SED-362	SDQ Hiperaktivite ebeveyn kılavuzuna göre Sınır (6) düzey olarak tanımlanmaktadır.
SED-363	SDQ Hiperaktivite öğretmen kılavuzuna göre Sınır (6) düzey olarak tanımlanmaktadır. Sınıf içi hiperaktivite artmış, izleme önerilir.
SED-400	Swanson, Nolan ve Pelham Derecelendirme Ölçeği
SED-408	Sıklık temelli nokta matrisi, tepki yüzdesi = (tepki/gözlem)×100 — gözlemlenebilir+sayılabilir+bağlamlı
SED-409	T-skoru — yaş/cinsiyet normlu, tek T ile etiket yok
SED-422	Tarama pozitifliği — tanı değil, yönlendirme
SED-443	Vanderbilt DE öğretmen kılavuzuna göre Negatif tarama (0-5) olarak tanımlanmaktadır. Sınıf içi dikkat belirtileri eşik altında.
SED-444	Vanderbilt Hiperaktivite ebeveyn kılavuzuna göre Negatif tarama (0-5) olarak tanımlanmaktadır.
SED-445	Vanderbilt Hiperaktivite ebeveyn kılavuzuna göre Pozitif tarama (≥6 belirti 2-3 + ≥1 performans) olarak tanımlanmaktadır.
SED-446	Vanderbilt Hiperaktivite öğretmen kılavuzuna göre Negatif tarama (0-5) olarak tanımlanmaktadır.
SED-447	Vanderbilt Hiperaktivite öğretmen kılavuzuna göre Pozitif tarama (≥6 belirti 2-3 + ≥1 performans) olarak tanımlanmaktadır.
SED-450	WISC-IV-TR (2013 normlu)
SED-451	WISC-V (Wechsler)
SED-452	WISC-V/CBCL/CAS/d2 dışarıda uygulanır, yalnız özet girilir
SED-453	Wechsler Intelligence Scale for Children - Fifth Edition (ve WISC-IV/R TR uyarlamaları)
SED-454	Weiss Functional Impairment Rating Scale - Parent
SED-459	Yasak kutu: tanı/tedavi/yüzde dili/akran karşılaştırması yok — sistem otomatik öneri üretmez, uzman seçer.
SED-460	Yasak kutu: tanı/tedavi/yüzde dili/akran karşılaştırması yok — sistem otomatik öneri üretmez.
SED-473	Z-12 destek üçgeni (çocuk–ebeveyn–öğretmen) tamam mı? Z-17 BEP’in kanıt sütunları — MENTORIA-SED BEP yazmaz, yalnız kanıt üretir.
SED-474	Z-12 — üçgen tamam mı?
SED-475	Z-12: çocuk–ebeveyn–öğretmen üç köşe, her köşe en az 1 kayıt içermeli · Z-17: BEP’in
SED-476	Z-17 — BEP Kanıt Paketi (8 sütun)
SED-503	tanı koymaz, ilaç önermez
SED-505	trenddir, tanı değildir
SED-507	verir; puanlamayı batarya yapar. Tek ölçümle karar yok — trend gerekir.
SED-518	Çalışma Belleği (WMI)
SED-535	Ölçek maddeleri MENTORIA-SED’da yoktur
SED-536	Ölçme Kanıtı
SED-537	Ölçme kanıtı:
SED-540	Öneri düzeyi:
SED-541	Öneri: Rutin Kartı
SED-556	Ücretli ölçeklerde (Conners 3, BRIEF-2, ADHD-RS-5) formu MENTORIA-SED dışından lisanslı olarak temin etmediyseniz puan girmeyiniz.
SED-564	İzleme: Günlük Bağlam Kaydı (günlük 3 soru, 0-3) + öğretmen gözlem pasif (okumaz/puanlamaz) + Gelişimsel Eşik Şeması ([REF])
SED-575	≥6 hafta izlem, haftada-1 oturum 40 dk, ≥14 gün Bağlam Kaydı seri
SED-577	✅ Üçgen tamam — yorum yapılabilir (tek başına yeterli değil, trend gerekir).
```
