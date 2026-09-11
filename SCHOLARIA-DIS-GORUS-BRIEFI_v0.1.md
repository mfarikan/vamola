# SCHOLARIA — İKİ AYRI ÜRÜN İÇİN DIŞ GÖRÜŞ BRİEFİ v0.1

**Kayıt:** K-760 · **Tarih:** 11.09.2026 · **Durum:** SALT-OKUNUR HAZIRLIK TAMAM / dış görüş bekleniyor.
**Sahip kararı:** “devam” sonrasında ayrı seçim: **SCHOLARIA paketini hazırla**. Ürün/kanon düzeltmesi veya mühür onayı değildir.
**İnceleme tabanı:** v7.65.61 mühürlü kaynak ve mevcut TAM HTML'ler. Bu brief henüz mühür dışı yeni belgedir.

## 0. Dış değerlendiriciye görev

Bu paket bir aile uygulaması değerlendirmesi değildir. **SCHOLARIA-LEX ve SCHOLARIA-SED iki ayrı okul/öğretmen ürünüdür.** Benzer dosyalar/menüler aynı pedagojik anlam, aynı kaynak yeterliği veya ortak düzeltme kararı demek değildir. MENTORIA ve SUPPORTA bu incelemenin hedefi değildir.

**Önce kapsam kabulü:** Her ürün için ayrı `KAPSAM TAMAM` veya `KAPSAM EKSİK — eksik ekran/rol/çıktı/kaynak` yazın. Kapsam kabulü bilimsel, klinik, hukuki doğrulama ya da ürünün her olası durumunun test edildiği anlamına gelmez. Eksik paket varsa onu belirtin; eksikliği “üründe özellik yok” diye otomatik yorumlamayın.

**Sonra satır incelemesi:** Her kayıt için `KORU / REVİZE / GİZLE ADAYI / KAYNAK-İŞLEV DOĞRULAMASI` sınıfını seçin. Şu formatı kullanın:

| Ürün | Kaynak ID / DOM durumu | Exact mevcut ifade | Hedef okur | Karar önerisi | Gerekçe / kaynak | Minimum öneri | İşlev/kaynak bağımlılığı |
|---|---|---|---|---|---|---|---|
| SCHOLARIA-LEX veya SCHOLARIA-SED | SCH-LEX-… / SCH-SED-…; ekran adı | Alıntıyı değiştirmeden | öğretmen/kurum/veli/terminal-önizleme | ayrı karar | varsa URL + baskı/sürüm + sayfa | kesin çözüm değil öneri | metin mi, hesap mı, rol mü? |

- İngilizce açıklamanızı ürünün birebir İngilizce metni gibi alıntılamayın. Parçalı JSX/template kaydı bütün cümle değildir; DOM ve ham kaynak bağlamıyla birleştirin.
- KORU, algoritmanın/kaynağın doğrulandığı anlamına gelmez. Bir başlık/şerh düzeltmesi sahte kesinlik veya eksik işlevi çözmez.
- K-709 onaylı menü adları korunur; alternatif bir ad otomatik kanon olmaz. MENTORIA-LEX'e verilen K-758/D değişim-dili kararı SCHOLARIA'ya otomatik taşınmaz.
- Çocuk yüzeyi M-3 listesi yetişkin panelinde kör 0-hit kuralı değildir. Öğretmen metrikleri kısa açıklamalı; kurum özeti resmî ve kısa; aileye dönük çıktı jargonsuz olmalıdır. Öğrenci terminal önizlemesinin gerçek çocuk yüzeyine dönüşüp dönüşmediği ayrıca değerlendirilir.
- Yeni sözlük/protokol, yeni ürün sürümü, hesaplama/rol düzeltmesi istenmiyor. Dış görüş → sahip kararları → minimum uygulama → test → **ayrı mühür onayı** sırası geçerlidir.

## 1. Kanıt sınırı ve okuma sırası

1. §2/§3'te iki ürünün ayrı kapsamını ve 14'er menüsünü okuyun.
2. Her ürünün DOM ekindeki 25 durum, başlangıç metinlerini ve seçilmiş koşullu çıktıları verir. `textarea` değerleri ayrıca alınmıştır; yalnız body metniyle sınırlı değildir.
3. Metin aday havuzu AST tabanlıdır: LEX474 / SED470 **kaynak kaydı**. Bu sayılar benzersiz görünür cümle veya hata sayısı değildir. Teknik/koşullu parçalar içerir. FrictionMap bağlı olmayan kaynak rezervi diye işaretlidir.
4. Ek C'de her ürünün 23 TS/TSX dosyasının **tam ham metni** bulunur; havuzun kaçırabileceği kısa dizgeler, interpolasyonlar, veri/hesap/rol bağlamı buradan kontrol edilir. CSS ve paket bağımlılıkları metin havuzuna dahil değil. Dinamik kombinasyonların tümü çalıştırılmadı.
5. Ek A mevcut Protokol v1.2 + Sözlük v1.6'nın bu tarihteki tam kopyasıdır; kaynak dosyalar değiştirilmedi. Ek B ilgili karar zinciri ve tarihî ürün-belge sınırını açıklar.

**Uygulanan inceleme:** iki mevcut TAM'da smoke12/12+12/12; DOM25+25 durum, gözlenen konsol/çalışma zamanı hatası0 ve bu akışlarda HTTP/S isteği0. Tarayıcı bağlamları yeni/yalıtılmış; yalnız sentetik not kullanıldı. HTTP/S ağ çıkışı engellenerek izlendi. Ağ isteği görülmemesi bütün güvenlik/KVKK/onam/senkron olasılıklarını doğrulamaz. Build/tsc yeniden yapılmadı; mevcut artefaktlar incelendi. Ürün dosyaları, package/lock, HTML ve kanon SHA'ları değişmedi.

**Tarihî dosyalar:** Eski DEMO/PILOT ve eski README sürüm atıfları güncel TAM diye kullanılmadı; yeniden derlenmedi/silinmedi. Kaynak ile build'in bütünsel üretim eşdeğerliği bu turda yeniden build edilerek kanıtlanmadı; mevcut kanoniklerde seçilmiş DOM akışları doğrulandı.

## 2. SCHOLARIA-LEX — bağımsız kapsam

**Sürüm:**2.10.1 · **Yetişkin bağlamı:** okul/öğretmen; LEXIVA alan uyarlaması (K-700). “Bilişsel Gelişim Laboratuvarı”, sınıf ritmi, katılım, yorgunluk eğimi ve yanıt zamanı eğrisi dili bulunur. Bunlar SED'in GFI/Fslope etiketleriyle aynı yüzey sayılmaz; ad değişimi ölçüm geçerliği kanıtı değildir.

**Gerçek kabuk:** App sabit `rol="B2B Yönetici"` geçirir; menüde öğretmen, öğrenci, veli hedefli içerik olması ayrı giriş/yetkilendirme kanıtı değildir. Veli ekranı öğretmenin hazırladığı paylaşım taslağıdır; aileye doğrudan gönderim doğrulanmadı.

### 2.1 Menü → bileşen → okur → işlev haritası
| Menü | id | Kaynak (src altında) | Okur/aktör | Mevcut kapsam |
|---|---|---|---|---|
| Sınıf Özeti | `pano` | App.tsx | Kurum/öğretmen | Sentetik sınıf kartları; sınıf seçimine geçiş. |
| Sınıf | `sinif` | App.tsx; data/mock.ts; data/seriler.ts | Öğretmen | Sınıf seçici, sentetik gösterge ve çizgiler; ölçüm doğrulaması değil. |
| Öğrenci | `ogrenci` | App.tsx | Yetişkin kabuğunda öğrenci terminal önizlemesi | Görev detay/kilit demosu; ayrı çocuk hesabı/rolü kanıtı değil. |
| Öğretmen | `ogretmen` | components/ogretmen/Cockpit.tsx; components/ders/OneriSablonlari.tsx | Öğretmen | Gösterge, mola yönlendirmesi ve öneri şablonu; gerçek model/analiz/onay işlevi ayrıca sorgulanır. |
| Transfer Gözlem Kartı | `transfer` | components/ogretmen/TransferGozlemKarti.tsx | Öğretmen | Davranış seçimi + serbest not; yerel H-c defteri, Likert değil. |
| Ders & Görev | `ders` | components/ders/GorevAtama.tsx; components/defter/SonucNotu.tsx; data/mufredatYonerge.ts | Öğretmen | MAT/TR kazanım/yönerge, yerel atama ve sonuç notu. Resmî müfredat kaynağı ayrıca doğrulanmalı. |
| Aile Bilgilendirme | `veli` | components/veli/VeliKoprusu.tsx | Üreten: öğretmen; hedef okur: veli | Aile bülteni taslağı + yerel randevu defteri; veli girişi/gönderim sistemi değildir. |
| BEP Hazırlık | `bep` | components/bep/BepHedef.tsx | Öğretmen | Gözlem-hedefi taslağı + probe; resmî BEP değil, editör/onay/taşıma fiilleri kaynakla ayrı incelenir. |
| MEB EBA Entegrasyonu | `eba` | components/eba/EbaPaneli.tsx | Öğretmen/kurum | Yerel H-c tabanlı daily-insight taslağı; mevcut akışta SSO/HTTP aktarımı değil. |
| Gelişim Takibi | `izleme` | components/izleme/IzlemePaneli.tsx; components/takip/GelisimTakibi.tsx | Öğretmen | Öğrenci seçimi ve kendi-serisi; canlı sensör/ölçüm doğruluğu kanıtı değil. |
| Sınıf İçi Ses Yönetimi | `ses` | components/ses/SesPaneli.tsx | Öğretmen | Slider SVG opaklığını değiştirir; mikrofon/filtre donanımı değildir. |
| Rapor | `rapor` | components/rapor/RaporOzeti.tsx; components/portfoy/Portfoy.tsx | Üreten: öğretmen; hedef okur: veli/kurum | Yerel defterlerden salt-okunur not ve metin portfolyosu; yazdırma/ihracat bu önizlemede yok. |
| Ayarlar | `ayarlar` | App.tsx; data/mock.ts | Kurum | Salt-okunur sentetik şube bilgisi; kurum yönetim yetkilendirme altyapısı kanıtı değil. |
| Sistem Kılavuzu ve Terimler | `yardim` | App.tsx; data/kisitlar.ts | Öğretmen/kurum | Kısıtlar, terimler ve açıklamalar; bool sabitleri yasal/teknik uyum sertifikası değildir. |

**Kaynak kökü:** `VAMOLA - Lexiva/LEXIVA_SCHOLARIA/SCHOLARIA_TAM/src` ·23 TS/TSX,17 TSX.

**Kanonik HTML:** `VAMOLA - Lexiva/LEXIVA_SCHOLARIA/SCHOLARIA_TAM/LEXIVA-SCHOLARIA-v2.10.1.html` ·300619 B ·SHA-256 `417c786cdcdd0e0f7e1cffacacbfe1eb806ffea983764781ece52a7cc8d8db4a`.

### 2.2 SCHOLARIA-LEX için özel değerlendirme soruları

- K-700'deki okuma/öğrenme alanı uyarlaması görünür etiket ve görev bağlamında yeterli mi? “Katılım”, “Y-Eğim”, ritim/yanıt zamanı gösterimleri gözlenen/sentetik değer olarak mı okunuyor, öğrenci özelliği veya doğrulanmış ölçüm diye mi?
- Sınıf/öğretmen önerilerinin LEX'e özgü kanıt bağlantısı var mı? T1/L1 analiz iddiası, sabit şablon seçimi ve %78 ifadesi birbirinden ayrılmalı.
- EBA başlığındaki mevcut yetenek çağrışımı, alt paneldeki PLANLI/gönderim yok şerhiyle yeterince sınırlandırılmış mı?
- K-450 kapsam belgesi tarihî faz-A kaydıdır; eski “hedef üretmez” satırını bugünkü hedef-şablonunu silme yetkisi saymayın. K-558 daha sonraki SED şablon kararı, K-683/K-700 aktarım/uyarlama zinciriyle beraber LEX için bağımsız sahip yorumu gerektirir.
- LEX Yardım'daki hızlı-tur metni kaynakta bulunur; SED'de bulunmaması otomatik parite hatası değildir. Bilinçli profil ve tarihî farklar ayrı sınıflanmalı.

## 3. SCHOLARIA-SED — bağımsız kapsam

**Sürüm:**0.2.7 · **Yetişkin bağlamı:** toplu sınıf içi dikkat/yürütücü işlev kalibrasyon sistemi; SED ürün alanı. Kaynakta G_contrast, GFI, Fslope ve d(SDRT)/dt etiketleri bulunur. Öğretmen yüzeyinde olmaları otomatik yasak değil; tanım, türetim, eşik ve yetki iddiası ayrı incelenir. Sinüs tabanlı sentetik seri, gerçek sensör veya doğrulanmış hesap değildir.

**Gerçek kabuk:** App sabit `rol="B2B Yönetici"` geçirir. Öğrenci sekmesi mevcut yetişkin kabuğunun içindeki terminal/kilit önizlemesidir. EBA ve ses işlevleri planlı/simülasyon şerhleriyle okunmalıdır; tarihî PRD'nin hedef mimarisi çalışan ürün işlevi diye sunulmaz.

### 3.1 Menü → bileşen → okur → işlev haritası
| Menü | id | Kaynak (src altında) | Okur/aktör | Mevcut kapsam |
|---|---|---|---|---|
| Sınıf Özeti | `pano` | App.tsx | Kurum/öğretmen | Sentetik sınıf kartları; sınıf seçimine geçiş. |
| Sınıf | `sinif` | App.tsx; data/mock.ts; data/seriler.ts | Öğretmen | Sınıf seçici, sentetik gösterge ve çizgiler; ölçüm doğrulaması değil. |
| Öğrenci | `ogrenci` | App.tsx | Yetişkin kabuğunda öğrenci terminal önizlemesi | Görev detay/kilit demosu; ayrı çocuk hesabı/rolü kanıtı değil. |
| Öğretmen | `ogretmen` | components/ogretmen/Cockpit.tsx; components/ders/OneriSablonlari.tsx | Öğretmen | Gösterge, mola yönlendirmesi ve öneri şablonu; gerçek model/analiz/onay işlevi ayrıca sorgulanır. |
| Transfer Gözlem Kartı | `transfer` | components/ogretmen/TransferGozlemKarti.tsx | Öğretmen | Davranış seçimi + serbest not; yerel H-c defteri, Likert değil. |
| Ders & Görev | `ders` | components/ders/GorevAtama.tsx; components/defter/SonucNotu.tsx; data/mufredatYonerge.ts | Öğretmen | MAT/TR kazanım/yönerge, yerel atama ve sonuç notu. Resmî müfredat kaynağı ayrıca doğrulanmalı. |
| Aile Bilgilendirme | `veli` | components/veli/VeliKoprusu.tsx | Üreten: öğretmen; hedef okur: veli | Aile bülteni taslağı + yerel randevu defteri; veli girişi/gönderim sistemi değildir. |
| BEP Hazırlık | `bep` | components/bep/BepHedef.tsx | Öğretmen | Gözlem-hedefi taslağı + probe; resmî BEP değil, editör/onay/taşıma fiilleri kaynakla ayrı incelenir. |
| MEB EBA Entegrasyonu | `eba` | components/eba/EbaPaneli.tsx | Öğretmen/kurum | Yerel H-c tabanlı daily-insight taslağı; mevcut akışta SSO/HTTP aktarımı değil. |
| Gelişim Takibi | `izleme` | components/izleme/IzlemePaneli.tsx; components/takip/GelisimTakibi.tsx | Öğretmen | Öğrenci seçimi ve kendi-serisi; canlı sensör/ölçüm doğruluğu kanıtı değil. |
| Sınıf İçi Ses Yönetimi | `ses` | components/ses/SesPaneli.tsx | Öğretmen | Slider SVG opaklığını değiştirir; mikrofon/filtre donanımı değildir. |
| Rapor | `rapor` | components/rapor/RaporOzeti.tsx; components/portfoy/Portfoy.tsx | Üreten: öğretmen; hedef okur: veli/kurum | Yerel defterlerden salt-okunur not ve metin portfolyosu; yazdırma/ihracat bu önizlemede yok. |
| Ayarlar | `ayarlar` | App.tsx; data/mock.ts | Kurum | Salt-okunur sentetik şube bilgisi; kurum yönetim yetkilendirme altyapısı kanıtı değil. |
| Sistem Kılavuzu ve Terimler | `yardim` | App.tsx; data/kisitlar.ts | Öğretmen/kurum | Kısıtlar, terimler ve açıklamalar; bool sabitleri yasal/teknik uyum sertifikası değildir. |

**Kaynak kökü:** `VAMOLA - Seduva/SEDUVA_SCHOLARIA/src` ·23 TS/TSX,17 TSX.

**Kanonik HTML:** `VAMOLA - Seduva/SEDUVA_SCHOLARIA/SCHOLARIA-MVP-TAM-v0.2.7.html` ·299792 B ·SHA-256 `36df69c3aa555d425c74a4acd908ae61ea2d4c766bfcdc6ca88a5c50674d36da`.

### 3.2 SCHOLARIA-SED için özel değerlendirme soruları

- Dikkat/yürütücü işlev “kalibrasyonu”, GFI/Fslope, “dürtüsel hataları engeller” ve zorunlu dinlenme çağrışımları; mevcut sentetik/demo davranışla hangi seviyede destekleniyor?
- G_contrast ve d(SDRT)/dt eğrilerinin isimleri ile `seri()` sinüs üreticisi arasındaki fark öğretmene açık mı? Sayı/renk/0.07 eşiği için kaynak ve bağlam istenmeli; bu turda eşik doğrulanmadı/değiştirilmedi.
- BEP hedef şablonu K-558 ile tarihsel olarak izinli. “Öğretmen düzenler” metni ile `readOnly` çıktı ve hazır probe durumlarının fiili anlamı bağımsız incelenmeli; resmî BEP değildir şerhi tek başına düzenleme işlevi sağlamaz.
- SED PRD v1.3'teki donanım/SSO/algı/nedensellik hedefleri ve eski terimler bugünkü ürün beyanından ayrılmalı. PRD'nin Approved ibaresi dış bilimsel kanıt değildir. Tarihî belge bu turda düzeltilmedi.
- Aile notları öğretmen gözlemi aktarımı mı, sistemin öğrenciyi değerlendirmesi gibi mi okunuyor? Serbest öğretmen notunun aynen aktarılması, girdinin dil/mahremiyet açısından doğrulandığı anlamına gelmez.

## 4. Kaynakla belirlenen çapraz inceleme adayları — iki ürüne AYRI karar gerekir

Bu tablo düzeltme listesi veya yeni kanon değildir. Ortak kaynak desenleri bile ürün başına ayrı değerlendirilir.

| Konu | Kanıt / mevcut davranış | Değerlendiriciden istenen ayrım |
|---|---|---|
| Yetki | App sabit B2B Yönetici; Kabuk rol metnini gösterir | Rol etiketi ≠ kimlik doğrulama/rol bazlı erişim. Veli/öğrenci hedefli metni ayrı oturum sanmayın. |
| YZ/istatistik | OneriSablonlari: T1/L1 analiz beyanı; buton `setSecili([0, 2])`; %78 düz dizge | Model çağrısı ve güven aralığı hesabı bu bileşende yok. Metinsel/işlevsel/kaynak sınıflarını ayırın. |
| İnsan onayı | Onayla düğmesinde onClick yok; reddet setReddedildi(true); DOM'da onay sonrası not aynı | Onay/veri izi/gerekçe işlevi ayrı açık; şerhi değiştirmek işlevi tamamlamaz. |
| EBA | App SSO beyanı; EbaPaneli yerel taslak+PLANLI rozeti; gözlenen HTTP0 | Başlık/vaat ile uygulama düzeyini ayırın. Endpoint adı gerçek MEB API doğrulaması değildir. |
| Ses | App “optimal öğrenme ortamı” ifadesi; panel sinüs/SVG ve opaklık değişimi | Ses işleme/algı etkisi/cihaz kurulumu diye yorumlamayın. |
| BEP | Şablon+readOnly textarea; probeEkle 0/1/2 döngüsü; yerel depolama | Şablon kanonu, düzenlenebilirlik, gerçek gözlem girişi ve kurum aktarımı ayrı konular. |
| Müfredat | Kaynak 62 kayıt (MAT25/TR37) ve özgün yönerge iddiası | Resmî kazanım kodu/adı/sürüm ve telif doğrulaması bu turda yapılmadı. “telifiSifir:true” hukuki sonuç değil. |
| Kayıt/çıktı | H-c → RaporOzeti/EBA/Veli/Portfoy; yerel defterler | Not taslağı ≠ basılı rapor/ihracat/gönderim; veri onamı/güvenliği ayrı. |
| Bağlı olmayan kaynak | FrictionMap.tsx App/import zincirine bağlı değil, DOM'da yok | “Öğrenme Sürtünme Haritası”nı canlı ekran diye listelemeyin; dosya rezervi/entegrasyon sorusu. |
| Eski belgeler | README sürümleri paket sürümlerinden geride; KISITLAR.surum=v0.1.0 | Belge/kısıt nesnesi sürümü ile ürün sürümünü karıştırmayın; bu tur değiştirilmedi. |

### 4.1 Exact kayıt adresleri

**SCHOLARIA-LEX:**

- `T1 (Merkez)`: SCH-LEX-0121 (`components/ders/OneriSablonlari.tsx:33`)
- `%78`: SCH-LEX-0125 (`components/ders/OneriSablonlari.tsx:47`)
- `SSO`: SCH-LEX-0040 (`App.tsx:185`); SCH-LEX-0041 (`App.tsx:186`)
- `optimal`: SCH-LEX-0043 (`App.tsx:194`)
- `öğretmen düzenler`: SCH-LEX-0068 (`components/bep/BepHedef.tsx:31`)
- `Gözlem`: SCH-LEX-0064 (`App.tsx:234`); SCH-LEX-0202 (`components/ogretmen/TransferGozlemKarti.tsx:79`); SCH-LEX-0216 (`components/portfoy/Portfoy.tsx:12`); SCH-LEX-0246 (`components/rapor/RaporOzeti.tsx:41`)
- `Friction Map`: SCH-LEX-0160 (`components/izleme/FrictionMap.tsx:36`)
**SCHOLARIA-SED:**

- `T1 (Merkez)`: SCH-SED-0117 (`components/ders/OneriSablonlari.tsx:33`)
- `%78`: SCH-SED-0121 (`components/ders/OneriSablonlari.tsx:47`)
- `SSO`: SCH-SED-0040 (`App.tsx:185`); SCH-SED-0041 (`App.tsx:186`)
- `optimal`: SCH-SED-0043 (`App.tsx:194`)
- `öğretmen düzenler`: SCH-SED-0064 (`components/bep/BepHedef.tsx:31`)
- `Gözlem`: SCH-SED-0198 (`components/ogretmen/TransferGozlemKarti.tsx:79`); SCH-SED-0212 (`components/portfoy/Portfoy.tsx:12`); SCH-SED-0242 (`components/rapor/RaporOzeti.tsx:41`); SCH-SED-0256 (`components/shell/Kabuk.tsx:10`)
- `Friction Map`: SCH-SED-0156 (`components/izleme/FrictionMap.tsx:36`)

## 5. Dış görüş sonrası karar kapısı

1. Sahip briefi paylaşır; bu ajan dışarıya göndermedi.
2. Yanıt iki ürün için ayrı kapsam kabulü ve exact ID'li önerilerle gelir.
3. Kaynak/atıf/kanon kontrolü → ürün-başı önce/sonra/adet/dayanak kararcığı hazırlanır.
4. Sahip seçmeden kaynak/HTML/kanon/hesap/rol değişmez. Klinik/ölçüm/SSO/onam sorunları metin turuyla kapanmaz.
5. Gerekli uygulama seçilirse ürün sürümleri korunarak minimum tur ve test yapılır; mühür ayrıca sorulur.

**Bu turun dışı:** MENTORIA Vanderbilt/SDQ/metrik işleri ayrı kuyruk; SUPPORTA paketi açılmadı; PERSONA B-9/B-10 açılmadı. K-758 MENTORIA kanon hizalamaları mevcut kanona dahil, LEX'e özgü D kararı başka ürüne aktarılmadı.

## Ek A — mevcut kanonun değişmeden alınmış kopyası

Aşağıdaki kanon yerel sahip otoritesini gösterir; ürün algoritmalarının dış bilimsel/hukuki doğrulaması değildir. Belge içindeki eski sürüm atıfları tarihçenin parçasıdır, burada sessizce düzeltilmez.

### VAMOLA-STRATEJIK-HIZALAMA-VE-DIL-PROTOKOLU_v1.2.md

SHA-256 `e9336cc78dcd45ca8eb3914be601003f7efb7cc6502522794affcc03dc2c3455`

~~~~markdown
# VAMOLA (SEDUVA & LEXIVA) STRATEJİK HİZALAMA VE DİL PROTOKOLU

**Güncel sürüm:** v1.2
**Güncel karar/revizyon:** K-720 (10.09.2026)
**Önceki revizyonlar:** v1.1 (K-714/K-715) · v1.0 (K-698, 09.09.2026)
**Durum:** KANON ONAYLI (K-722 · 10.09.2026 — sahibin ask_user onayı: ① Faz-2 v1.1 satır-onayı 187 satır + ② PROTOKOL v1.2 & SÖZLÜK v1.4 kanon onayı) · **FAZ-3 UYGULANDI** (K-723 kod + K-724 dil-regresyon; çocuk yüzeyi 0-hit, smoke 8/8)

**Revizyon geçmişi (özet):**
- v1.2/K-720: §2 terim eşleme tablosu (yasaklı/zorunlu çelişkisi giderildi) · M-8 yönerge/nasıl kapsamı · dil-regresyon 0-hit yüzey tanımı (çocuk yüzeyi; KORU + tasarım sıfatları kapsam dışı).
- v1.2/K-719: Dil-Regresyon Kontrol Listeleri (M-3 + B-liste) · SÖZLÜK 4 satır standardizasyonu.
- v1.2/K-718: 7 küçük düzeltme + Kaptan kural 5 + M-14 veli sınırı.
- v1.2/K-717: pedagojik revizyon (Temel Standart, M-1..M-14, iki-bant, Kaptan 5 kural, editoryal kontrol) + dış görüş K-716 entegrasyonu.
- v1.1/K-714+K-715: §5 Ses Haritası + §6 M-1..M-10 + §7 kahraman ad kararı (Kaptan Fener / Kaptan Nota).
- v1.0/K-698: ilk hizalama protokolü (09.09.2026).

**Amaç:** Lexiva ve Seduva ekosistemlerinin B2B ürün yapılarına bölünmesi ve dış görüşlerden (DBI, UDL, AI Act vb.) alınan akademik geri bildirimlerin tüm sisteme standardize edilerek uygulanması için yazılmış nihai uyum (Alignment) protokolüdür. Bu protokol, workspace içindeki tüm PRD, Spec, README ve Kod dosyaları için "Tek Doğruluk Kaynağı (Single Source of Truth)" olarak kabul edilir.

## 1. ÜRÜN VE ARAYÜZ (MENÜ) İSİMLENDİRME STANDARDI
Lexiva ve Seduva'nın "Monolitik Demo" döneminden kalan tüm eski menü ve ürün isimleri yasaklanmıştır.
*   **PERSONA / Çocuk-Veli:** Ürün adı `PERSONA`'dır. Aile karşılama ekranı `Gelişim Özeti` olarak anılır (Dashboard / Pano yasaktır).
*   **SCHOLARIA / Öğretmen:** Ürün adı `SCHOLARIA`'dır. Karşılama ekranı `Sınıf Özeti` olarak anılır.
*   **SUPPORTA / Eğitmen:** Ürün adı `SUPPORTA`'dır. Karşılama ekranı `Eğitmen Kürsüsü` olarak anılır.
*   **MENTORIA / Uzman:** Ürün adı `MENTORIA`'dır. Karşılama ekranı `Uzman Masası` olarak anılır.

## 2. HUKUKİ VE MEDİKAL SINIRLAR (K-02 GÜNCELLEMESİ — K-720 düzeltmesi)
VAMOLA bir tıbbi cihaz (Medical Device) veya tanı/tedavi yazılımı değildir.
**Terim eşlemesi (eski/yasaklı biçim → kanonik zorunlu biçim):**
| Eski / yasaklı biçim | Kanonik zorunlu biçim |
|---|---|
| Teşhis | YASAK — karşılık YOK (tanı dili ürün dilinde yer almaz) |
| Tedavi | YASAK — karşılık YOK (tedavi dili ürün dilinde yer almaz) |
| eğitimsel destek önerisi (küçük harf, jenerik serbest kullanım) | **Eğitimsel Destek Önerisi** (kanonik terim) |
| gelişimsel hedef (küçük harf, jenerik serbest kullanım) | **Gelişimsel Hedef** (kanonik terim) |
| terapi/terapötik ifade yerine | **Pedagojik Yönlendirme** |
| uyarlama ifadesi yerine | **Eğitimsel Adaptasyon** |

**Kural:** YASAKLI biçim, bir ifadenin küçük-harf/jenerik serbest kullanımıdır; ZORUNLU karşılık o ifadenin yerine geçen kanonik terimdir. Teşhis/Tedavi'nin karşılığı YOKTUR (K-02: ürün tanı/tedavi dili kullanmaz).

## 3. VERİ VE YAPAY ZEKA YÖNETİŞİMİ (AI GOVERNANCE)
Eski veya piyasadaki standart EdTech söylemleri yerine en üst düzey güvenlik ve akademik duruş benimsenecektir.
*   **AI Rolü:** `Human-Accountable AI (İnsan Sorumluluğunda YZ) (İnsan onaylı AI)` yerine, daha kapsayıcı olan **`Human-Accountable AI (İnsan Sorumluluğunda YZ)`** terimi kullanılacaktır. AI tanı koymaz, kanıt (evidence) işler, belirsizliği (uncertainty) bildirir. İnsan uzman bunu override edebilir (geçersiz kılabilir).
*   **Veri Mimarisi:** Düğüm noktaları (Ev, Okul, Merkez, Klinik) arasında `Shared Evidence Protocol (Yetkili Kanıt Protokolü (Shared Evidence Protocol))` veya `Veri Havuzu` kavramları **YASAKLANMIŞTIR**. Doğru tanım: **`Shared Evidence Protocol (Yetkili Kanıt Protokolü)`**. Sistem ham veri değil, kanıtlanmış paket paylaşır.

## 4. 10 KATMANLI BİLİMSEL MİMARİ (SCIENTIFIC ARCHITECTURE)
Herhangi bir belgede sistem mimarisi anlatılırken "Adaptif Öğrenme (Adaptive Learning)" gibi basit tanımlar yerine, **"Adaptif Eğitimsel Destek Ekosistemi"** tanımı ve aşağıdaki 10 katman kullanılacaktır:
1.  **Dynamic Learning Model:** Statik profil atamaz (Örn: Görsel öğrenen demez), anlık duruma göre modeli günceller.
2.  **Evidence Provenance:** Friction (görevi bırakma vs.) bir yorum değil, saf kanıttır.
3.  **Context Layer:** Kanıtın çevresi (ortam, zaman, kişi) kaydedilir.
4.  **Learning Response Map:** Desteklerin neden olduğu reaksiyonların nedensellik iddia edilmeden haritalanması.
5.  **Adaptive Support & Support Fading:** İçerik zorluğu değil, desteğin (ipucu/süre vb.) yoğunluğu ayarlanır ve azaltılır.
6.  **Implementation Fidelity:** Çocuğun başarısızlığı mı yoksa müdahalenin mi eksik uygulandığı ayrıştırılır.
7.  **Transfer Evidence:** Sistemi beceriyi gerçek hayata "transfer eder" diyerek değil, T1-T2-T3 düzeyinde "transfer kanıtını izler" şeklinde tanımlarız.
8.  **Learning Agency:** Öz-düzenleme (mola, yardım isteme) becerisinin izlenmesi.
9.  **Uncertainty Layer:** Sistem karar verirken "Kanıt yetersiz" (Low Confidence) diyebilmelidir.
10. **Evidence Ladder:** E0'dan E7'ye uzanan bilimsel kanıt ölçüm basamakları.

## 5. SES HARİTASI (YENİ v1.1 — K-713/K-714)
Aynı metin havuzu 5 okuyucuya 5 sesle yazılır. 1:1 ayna = aynı KAVRAM, aynı AD (K-709 listesi), farklı SES.

| Okuyucu | Yüzey | Ses |
|---|---|---|
| **Çocuk** (5–10) | Persona çocuk (görevler, Kaptan diyalogları, karşılama, mola) | Kaptan + görev sesi — 3. sınıf okuma düzeyi; 1 satır ≤12 kelime; somut eylem; tek adım; "sen"; kıyas/ceza/leaderboard YOK |
| **Veli** | Persona veli panoları, raporlar | Sıcak, düz, korkutmayan; veri → basit cümle; klinik jargon YOK |
| **Öğretmen** | Scholaria/Supporta öğretmen yüzleri | Net, yarı-resmî; metrik etiketleri kısa açıklama ile |
| **Uzman** | Mentoria, uzman panoları | Profesyonel; jargon serbest; tam tanımlar; istatistik (SD, ms, %) burada yaşar |
| **Kurum** | Kurum panoları, brifingler | Resmî, özet |

**Kural:** Tanımlar ve istatistiksel etiketler UZMAN kartında yaşar; çocuk kartı = başlık + tek yönerge + nasıl + (varsa) Kaptan sonraki-adım satırı — ÖLÇÜM ÇOCUKTA GÖSTERİLMEZ (M-14 · Sözlük v1.4 §3-H).

## 6. ÇOCUK METİN İLKELERİ (v1.2 — M-1..M-14)

### TEMEL STANDART (tek cümle — K-717 sahip)
> **Çocuğa "neyin yanlış olduğunu" veya "hangi bilişsel özelliğe sahip olduğunu" anlatma; çocuğun ŞİMDİ NE YAPACAĞINI ve gerekirse bir sonraki denemede neyi deneyebileceğini söyle.**

- **M-1** Bir ekran bir mesaj; ana kriter = tek mesaj + kısa ve tek anlamlı cümle + mümkünse tek eylem. Kelime sınırı (satır ≤12 · cümle ≤20) YARDIMCI kuraldır.
- **M-2** Çocuk yüzeyinde akademik/klıınik tanım YOK — çocuk ekranı "ne yapacağını" söyler; tanım uzman kartında yaşar.
- **M-3** Çocuk yüzeyinde uzman kavramı değil, çocuğun yapacağı SOMUT EYLEM anlatılır. YASAKLI (açık liste — örnek, kapalı değil): ms · % · SD · formül · katsayı · perseverasyon · inhibisyon · prosodi · otonom sinir · tolerans penceresi · kalibrasyon · batarya · telemetri · paradigma · eksen · "görev performansı" · otomatikleştirmek · tutarlılık · seçicilik · tempo · öz-düzenleme.
- **M-4** Hitap = "sen"; "birey / yürütücü işlev / katılımcı" YOK. Her cümle "sen"le başlamaz — doğal Türkçe esastır.
- **M-5** Kaptan sesi: 1–2 kısa cümle; cesaretlendirici; kıyas/ceza/leaderboard YOK; hata = yumuşak geri bildirim + tekrar daveti. **Kaptan çocuğun duygusunu/kapasitesini VARSAYMAZ; geri bildirim GÖZLENEN eyleme dayanır, sonucu etiketlemez.**
- **M-6** Bir kavram bir ad (tek kaynak: Sözlük v1.4 §3-H/§3-I): *mola* (standart) · çocuk "odak" / uzman "dikkat" · çocuk "oturum" / uzman "seans".
- **M-7** Dürüst-not çocuk dilinde: **"Burada puan yok. Nasıl yaptığını birlikte göreceğiz."** (K-02; "Seni dününden iyi tanıyorsun" KALDIRILDI — doğal değil).
- **M-8** Yönerge = 1 adım 1 eylem (ör. "Mavi düğmeye 12 kez bas"). "Önce… sonra… ardından…" gerektiğinde ayrı adımlara bölünür. **Kapsam (K-720):** YÖNERGE (canlı, yaptırılan talimat) = 1 adım/1 eylem; NASIL/YÖNTEM özeti (kart üstündeki açıklama) gerektiğinde çok adımlı olabilir — ancak UI'da sırayla yaptırılan eylemler her zaman ayrı adım olarak sunulur.
- **M-9** Süre/miktar çocukça: "2 dakika" · "10 kez" — "120 sn" YOK.
- **M-10** Erişilebilirlik: anlam renkten bağımsız sözcükle de verilir; ayrıca ikon, ses, kontrast, yazı boyutu ve görsel-işitsel eşleşme de tek başına anlaşılır olmalı.
- **M-11 (YENİ) SOMUT EYLEM:** Çocuk metni teknik kavramı açıklamaz; çocuğun yapacağı somut eylemi söyler. Temel soru: "Çocuk şimdi ne yapacak?"
- **M-12 (YENİ) YÜZEY AYRIMI:** Çocuk/veli/uzman aynı görevi farklı ayrıntıda anlatır. Teknik terimin çocuktan çıkarılması, teknik karşılığının sistemden çıkarılması DEĞİLDİR.
- **M-13 (YENİ) TERİM EŞLEME:** Her teknik kavramın uzman yüzeyinde TEK kanonik adı; çocukta yaşa uygun eylem ifadesi (birebir eşanlamlılık şart değil).
- **M-14 (YENİ) ÇOCUK UYGUNLUĞU FİLTRESİ:** Jargon filtresi ≠ çocuk uygunluğu filtresi. **Bir ölçüm, çocuk için eyleme veya anlamlı geri bildirime dönüşmüyorsa çocuk yüzeyinde GÖSTERİLMEZ** (uzman/veli kartına taşınır). Teknik terim içermeyen metin de çocuğa uygun olmayabilir. **Veli sınırı:** veli yüzeyine taşınan ölçüm = KAYIT GÖSTERİMİ; tanı/kapasite/bilişsel özellik/klinik yorum/"iyi-kötü" değerlendirmesine DÖNÜŞMEZ (ör. "Okuma temponu haftalık kayıtlarla görmek." kabul — "okuma hızın düşük" yorumu YASAK).

### İKİ-BANT ALT KURALI (K-717)
- **5–7 yaş:** kısa · somut · tek eylem · soru yerine doğrudan yönerge.
- **8–10 yaş:** AYNI temel dil; gerektiğinde kısa açıklama + basit öz-değerlendirme sorusu (asla teknikleşmez).
- Ana kural: **"Her çocuk metni en küçük yaşın anlayacağı kadar açık; ama gereksiz bebeksi DEĞİL."** Yeni ürün/klasör/komponent gerektirmez — aynı protokolün alt kuralı.

### KAPTAN SESİ — 5 KURAL (K-717 + K-716 + K-718)
1. Asla başka çocukla kıyaslama (arkadaş/sıralama/şampiyon YOK).
2. Hatayı çocuğun özelliği değil, görevin parçası say — geri bildirim gözlenen eyleme dayanır; zihinsel süreç çıkarımı YOK.
3. Sonucu yargılama (başarılı/başarısız/yetenekli/çok iyi YOK) — sıradaki küçük adımı göster.
4. Uzman/terapist/öğretmen/ebeveyn YERİNE GEÇMEZ. Kapasite iddiası ("Sen bunu başarabilirsin çünkü…") ve sorgulama ("Neden böyle yaptın?") YOK. İdeal: "Hazırsan başlayalım." · "Önce X'i bul." · "Olmadıysa bir kez daha deneyelim."
5. Çocuk METNİNDE sosyal-arkadaş dili YOK ("dostun", "arkadaşın", "arkadaş canlısı") — işlevsel eşlik dili kullanılır: "Kaptan Fener ile görevler" · "Kaptan eşliğinde" · "Kaptan Nota'nın görevleri". (K-703 "dost robot" TASARIM sıfatı ayrıdır ve korunur; kural yalnız çocuk METNİNİ kapsar.)

### EDİTORYAL KONTROL (10 madde — her yeni çocuk metni için)
1. Çocuk şimdi ne yapacak? (tek ve açık değilse yeniden yazılır) · 2. Teknik kavram var mı? (uzmana taşınır) · 3. Soyut kavram var mı? (somut eyleme) · 4. Mecaz gerekli mi? (değilse kaldırılır) · 5. Olumsuzluk var mı? (olumlu eyleme) · 6. Çocuğun duygusu/özelliği varsayılıyor mu? (kaldırılır) · 7. Performans baskısı var mı? (hız/puan/sıralama/başarı dili kaldırılır) · 8. Birden fazla eylem var mı? (adımlara bölünür) · 9. 5 yaş anlar mı? (sadeleştirilir) · 10. 9–10 yaş için bebeksi mi? (teknikleştirmeden doğallaştırılır).

### DİL-REGRESYON KONTROL LİSTELERİ (K-719 — Faz-3 0-hit dayanağı)
- **(a) M-3 YASAKLI JARGON listesi** (açık liste) → Faz-3'te ÇOCUK YÜZEYİNDE 0-hit.
- **(b) B-LİSTE — mecaz/baskı/etiketleme dili** (örnek liste, KAPALI DEĞİL; kaynak: dış görüş raporu §9 + sahip incelemeleri K-717/K-718) → Faz-3'te 0-hit:
  *refleks gibi · inat etmeden · eski kurala yapışmak · göğsünü sakinleştirmek · aklının kapanması · parçala-birleştir kası · harfin şekliyle sesiyle buluşsun · tempo · ne çabuk · kendi saatini gerçek saate yaklaştırmak · dostun/arkadaşın/arkadaş canlısı (çocuk metninde) · panik · güçlü kal · takılıyorsun · not (okul çağrışımı) · ne kadar sakindin · düzgün · puan · kıyas dili (daha hızlı / en iyi / arkadaşından / birinci ol)*
- **(c) Faz-3 dil-regresyon kapsamı:** (a) 0-hit + (b) 0-hit + EDİTORYAL KONTROL m.1..10 tam geçiş. (b) listesinde olmayan yeni mecaz/baskı ifadesi, EDİTORYAL KONTROL m.4/5/6/7 ile yakalanır; bu kural kapalı-liste aşımını önler.
- **(d) Tarama YÜZEYİ (K-720):** 0-hit taraması yalnız ÇOCUK YÜZEYİNDE yapılır (student/* + Kaptan + rol seçim metinleri). Uzman/veli/öğretmen/kurum yüzeylerinde M-3 ve B-liste terimleri serbesttir. KORU statüsündeki ifadeler (ör. "Odaklan, güçlen, ilerle!" sloganı, "süper güçler", K-703 "dost robot" TASARIM sıfatı) tarama kapsamı DIŞINDADIR.
- **(e) 'puan' kapsamı (K-720):** B-liste "puan" yasağı = ölçüm/sonuç/performans puanı. Gamification birimi (XP/yıldız — K-703) ayrı kanonik karardır; bu yasağa tabi DEĞİLDİR.

## 7. KAHRAMAN ADI KARARI (YENİ v1.1 — F-2, K-714)
Sahip kararı (10.09.2026): Ayna doktrini doğrulanmıştır — kahraman adları **aile-özgüdür** (DEHB/odak teması ↔ ÖÖG/hece teması; tıpkı ürün isimleri gibi). **Kanon (K-715 sahibi kararı, 10.09.2026): SEDUVA = Kaptan Fener · LEXIVA = Kaptan Nota.** Seçilen yaratıcı adlar; Faz-3 uygulamasına girer (kod + görsel: KaptanFokusAvatar→KaptanFenerAvatar, KaptanHeceAvatar→KaptanNotaAvatar). Sözlük v1.4 §3-H tek kaynak olarak güncellenmiştir.

~~~~

### VAMOLA-KANONIK-TERIM-SOZLUGU_v1.6.md

SHA-256 `aec734d82e9444b35e065b1d26654717d4cbcf918d1ce19783a20c67731c783e`

~~~~markdown
# VAMOLA — KANONİK TERİM SÖZLÜĞÜ v1.6

> **v1.6 minimum tutarlılık düzeltmesi (11.09.2026 — K-758; ayrı sahip A onayı):** M-7'nin iki eski alıntısı mevcut Protokol v1.2 cümlesine hizalandı; §3-D Klinik Rehber kaydı K-709'a çekildi, Uzman Masası ayrımı açıklandı. Yeni sözlük/protokol veya ürün sürümü üretilmedi. Eski dış görüş briefindeki ek, inceleme tarihinin sabit kopyasıdır.
> **v1.6 revizyonu (10.09.2026 — K-748; Tur-6-sonrası):** §3-H'ye **Kahraman adı gerekçesi** eklendi (sahibin seçim gerekçesinin kaydı — F-2'nin "adaylar sahibin değerlendirmesindedir" hükmü karşılık buldu). Yinelenen v1.2 revizyon satırı temizlendi (v1.4'ten devralınan doküman hatası). v1.5 hükümleri korunmuştur.
> **v1.5 revizyonu (10.09.2026 — K-746; Tur-6):** §3-H'ye **Yolculuk Yıldızı** maddesi eklendi (K4 doktrini: ödül-ekonomisi değil birey-içi ilerleme; M-7 dürüst-not ilişkisi; dayanak: ÜRÜN-MİMARİSİ §6.4/§6.9). v1.4 hükümleri korunmuştur.
> **v1.4 revizyonu (10.09.2026 — K-717; pedagojik revizyon — KANON ONAYLI, K-722):** §3-H metrik satırı M-14'e göre güncellendi (çocukta ölçüm gösterilmez → Kaptan sonraki-adım satırı) + §3-I dış görüş sözlüğü eklendi (çocuk↔veli↔uzman terim eşlemesi, ~55 satır).
> **v1.3 revizyonu (10.09.2026 — K-714; METİN DİLİ Faz-1, sahip onaylı) + K-715 düzeltmesi:** kahraman adları sahibin kararıyla güncellendi (SEDUVA: Kaptan Fener · LEXIVA: Kaptan Nota). §3-H "Çocuk Yüzeyi Lexiği" eklendi (M-6 bir-kavram-bir-ad standardı; mola/odak-dikkat/seans ayrımı; kahraman adları aile-özgü — F-2 sahibi kararı). M-1..M-14 ilke metni `STRATEJIK-HIZALAMA-VE-DIL-PROTOKOLU v1.2` §6'dadır. V1.1/V1.2 hükümleri korunmuştur.
> **v1.2 revizyonu (09.09.2026 — K-617; TUR-5 UX-1):** Dış görüş doğrultusunda "Normsuz Raporlama" tanımı güncellendi. "Birey-içi İlerleme (Intra-individual Progress)" kavramı eklenerek normsuzluğun ölçümsüzlük/puansızlık olmadığı, nicel performans kıyası içerdiği güvence altına alındı. V1.1 hükümleri korunmuştur.

> **v1.1 revizyonu (05.09.2026 — K-454):** Özne bölümüne yaş bandı 6–18 eklendi. Konum satırı düzeltildi.

**Tarih:** 09.09.2026 · **Konum:** `ORTAK-BELGELER/` (zip-İÇİ)

---

## 1) 🟢 KANONİK FARK: NORMSUZLUK VE BİREY-İÇİ İLERLEME (YENİ v1.2)
Sistemin teşhis veya medikal tanı koymadığı kararı (K-02 kırmızı çizgisi) gereği; ölçme-değerlendirme söyleminde **"birey-içi (intra-individual) nicel ölçüm"** kanonik terim olarak benimsenmiştir.

| Terim | Tanım (Kanonik) | Ne Değildir? (Yasaklılar) |
|---|---|---|
| **Normsuz Raporlama (Norm-Free Reporting)** | Öğrencinin gelişimini kendi yaşıtlarına, ulusal normlara veya standart sapma havuzlarına kıyaslamayan değerlendirme felsefesi. | "Ölçümsüzlük" veya "Puansızlık" değildir. Raporlar ampirik metrik içerir. |
| **Birey-içi İlerleme (Intra-individual Progress)** | Çocuğun başarısını veya destek ihtiyacını **dünkü ve önceki performansıyla (kendi öz geçmişiyle)** kıyaslayarak nicel (rakamsal) olarak sergileyen ölçüm türü (Örn: *Son 3 haftada görev tamamlamadaki görsel ipucu ihtiyacı %40 azaldı*). | Akran kıyası, teşhis puanı, zeka puanı, % persentil yüzdesi DEĞİLDİR. |
| **Öğrenme Örüntüsü (Learning Pattern)** | Çocuğun görevleri "hangi sürede, hangi bağlamda, hangi destek türleriyle" en verimli şekilde tamamlayabildiğini gösteren eğitsel analiz çıktısı. | Tıbbi tanı, klinik karar DEĞİLDİR. |

---

## 2) 🟢 HİYERARŞİ ZATEN TUTARLI — ÇELİŞKİ YOK

K-381'de *"hangisi üst kavram belirsiz"* demiştim. Tanım cümleleri tarandığında **üçünün de kendi belgesinde net tanımlandığı** ve **birbiriyle çelişmediği** görüldü:
| **CLEN™** | *"CLEN™ (Closed-Loop Executive Network / Kapalı Devre Yürütücü İşlev Ağı)… **tek bir arayüzün adı değil; ekosistemin tüm kurumsal B2B pazar düğümlerini besleyen ortak siber veri ve ağ mimarisidir**"* | **MİMARİ** (teknik belgeler) |
| **SEDUVA_RUNTIME** | *"**monorepo kod dizin yapısının en üst katmanında**, 01_ENGINE klasörü altında… **yerel görev kütüphanesini koşturan ana motor katmanıdır**"* | **KOD/DİZİN** (repo düzeyi) |

⇒ **Sorun çelişki değil, tek yerde toplanmış tanımın olmamasıydı.** Bu sözlük onu kapatır.

**Kanonik kullanım kuralı:**
- **Dış iletişim** (pitch, tanıtım, başvuru) → **SEDUVA CORE Engine™**
- **Teknik/mimari belge** → **CLEN™** (ilk geçişte açılımıyla)
- **Kod, dizin, repo** → **SEDUVA_RUNTIME** (yalnız teknik bağlam; pazarlama metninde geçmez)
- ⛔ Üçü **eş anlamlı gibi** kullanılmaz.

---

## 2) 🟢 "TERMİNAL" TANIMLANDI

50 hit tarandı; kullanım **tutarlı** çıktı: **Terminal = çocuğun ders/görev ekranı (uygulama arayüzü)**.

**Kanonik tanım:**
> **Terminal:** Çocuğun görev ve ders oturumlarını yürüttüğü **SEDUVA uygulama ekranı**. Bir marka adı değil, **ekran/arayüz katmanının** adıdır.

**Üç cihaz katmanı** (CURRICULUM §2'de tanımlı, korunur):

| Katman | Cihaz | Rol |
|---|---|---|
| **Deep Work Station** | PC/Mac | 30-45 dk ana müfredat seansı; "Karantina Modu" |
| **Mobile Terminal** | Tablet | Çoklu dokunmatik ana eğitim cihazı |
| **Satellite Hub** | Akıllı telefon | 5 dk kalibrasyon · hatırlatıcı · **veli izleme** |

**Yazım kuralı:** *"SEDUVA Terminali"* (ekran) · *"Mobile Terminal"* (cihaz katmanı, İngilizce özel ad) · ilk geçişte **"Terminal (çocuğun ders ekranı)"** açıklaması yazılır.
**⚠️ Not:** `Satellite Hub` **velinin telefonudur** — çocuk cihazı değil; "Terminal" ailesine dâhil edilmemelidir.

---

## 3) KANONİK TERİM TABLOSU (birleşik)

### A. Özne (kim?)
| Bağlam | Terim | ⛔ Kullanılmaz |
|---|---|---|
| Ürün ekranı, veli iletişimi | **çocuk** | operatör · hasta |
| Okul (Scholaria) | **öğrenci** | |
| Pilot/araştırma | **katılımcı** | denek |
| Danışma (Mentoria) | **danışan** | |
| Teknik mimari/log | **kullanıcı** | |
| Seansı yürüten yetişkin | **seans yürütücüsü** | operatör *(EK-C'de doğru kullanım — yetişkin)* |

**Yaş bandı (K-454, 05.09 — kullanıcı onayı):** Hedef çocuk kitlesi **6–18** (MEB okul öncesi + temel
eğitim + ortaöğretim paraleli). Pilot örneklem bantları (ör. PERSONA pilotu 7–10; LX-10 8–10) protokollerinde
ayrıca tanımlanır; ölçek norm yaş aralıkları (ör. TİFALDİ 2–12) ilgili ölçüm belgelerinde geçerlidir.

### B. Ürün düğümleri (K-373/K-381)
**SEDUVA** = çatı/ekosistem · **Persona™** (Consumer Bundle, B2C-ev) · **Scholaria™** (School Node, okul) · **Supporta™** (Support Node, özel eğitim/rehabilitasyon) · **Mentoria™** (Mentor Node, danışma).
⛔ **Clinical Node · Expert Node** — kanonik değil, kullanılmaz.

### C. Sistem katmanları
**SEDUVA CORE Engine™** (ürün motoru) · **CLEN™** (mimari) · **SEDUVA_RUNTIME** (kod) · **Terminal** (çocuk ekranı) · **Edge AI** (cihaz üstü işleme).

### D. Ekran/panel adları
**Expert Dashboard (Uzman Paneli)** · **Teacher Dashboard (Öğretmen Paneli)** · **Klinik Rehber** (Mentoria `navigator` alt ekranı; K-709) · **Satellite Hub** (veli mobil).
**Kural:** ilk geçişte İngilizce ad + parantez içinde Türkçe karşılık. **K-709 istisnası:** Klinik Rehber, onaylı Türkçe ürün adıdır; eski Guidance Navigator adına geri döndürülmez. **Uzman Masası** ise Protokol v1.2 §1’deki karşılama ekranıdır; Klinik Rehber ile aynı ekran değildir.

### E. Kurum
**VAMOLA EduLabs** (Ar-Ge) · **VAMOLA Academy** (eğitim/danışmanlık). İlk geçişte tam yazılır, sonra **EduLabs** serbest. ⛔ `VAMOLA EDULABS` (tümü büyük).

### F. Metrikler — değişmez
`S_c` (Focus Stability) · `TB` (Temporal Bias) · `F_slope` · `G_fi` (Gaze Fixation) · `P_hc` (Haptic Pressure).
**Şerh:** `G_fi` webcam **30-60 Hz**; `1 kHz` yalnız akıllı kalem taktil örneklemesi (K-01).

### H. Çocuk Yüzeyi Lexiği (YENİ v1.3 — M-6 standardı)
Persona çocuk ekranları (görevler, takvim, Kaptan diyalogları, mola, karşılama) için ad standardı. Uzman/veli/öğretmen yüzeylerinde ilgili terim serbesttir.

| Kavram | Çocuk yüzeyi (kanonik) | ⛔ Çocukta kullanılmaz | Uzman yüzeyi |
|---|---|---|---|
| Kısa ara | **mola** | ara · molaya ihtiyacın var mı (emir) | mola kullanımı |
| Dikkat odağı | **odak** ("odaklı kalmak") | dikkat (uzman yüzeyi) | dikkat |
| Çalışma turu | **oturum** | seans (×10/×7 kalıntı — Faz-2 temizliği) | seans |
| Görev adı | oyun/task ismi + tek adımlı yönerge | modül · katman · batarya | modül |
| Metrik etiketi | GÖSTERİLMEZ (M-14) — yerine Kaptan sonraki-adım satırı | ms · % · SD · katsayı · "(görev performansı)" · öz-değerlendirme sorusu | tam metrik |
| Hata geri bildirimi | yumuşak + tekrar daveti | hata oranı · commission · başarısız | hata oranı |
| Kahraman (SEDUVA) | **Kaptan Fener** | — | aynı |
| Kahraman (LEXIVA) | **Kaptan Nota** | — | aynı |
| İlerleme birimi | **Yolculuk Yıldızı** | XP · puan · coin · rozet-madalya (ödül-ekonomisi dili) | birey-içi ilerleme göstergesi |

**Şerh (F-2 — K-714 sahibi kararı):** Kahraman adları AİLE-ÖZGÜDÜR (ayna doktrini: aynı KAVRAM, farklı AD — DEHB/odak teması ↔ ÖÖG/hece teması). 1:1 ayna, adın kendisinde DEĞİL, kavram-seviyede yürür. Yaratıcı alternatif adayları sahibin değerlendirmesindedir (öneri — K-714); değişirse bu tablo tek kaynak olarak güncellenir.
**Dürüst-not (M-7):** çocukta puan/teşhis dili yerine: "Burada puan yok. Nasıl yaptığını birlikte göreceğiz."
**Kahraman adı gerekçesi (sahip kararı — K-748):**
- **Kaptan Fener (SEDUVA):** yol gösterme, dikkat/odak ve yön bulma çağrışımı güçlüdür — fener ışığı dikkati tek noktada toplar (odak teması), karanlıkta/yorgunluk anında yol gösterir (Kaptan'ın görev-yönlendirme rolü), yön bulma yürütücü işlev temalarıyla uyumludur; "Işık Yakala" göreviyle aile-içi bağ taşır (K-714 aday notu).
- **Kaptan Nota (LEXIVA):** okuma-yazma, ses, dil ve müzik çağrışımı nedeniyle ürün kimliğiyle doğal bağ kurar — nota, sesin yazıya/dize geçişidir (okuma-yazma alanının simgesi); ses-farkındalık ve hece-ritim görevleriyle (Ses Oyunu · Harf Dedektifi · akıcı okuma) doğrudan bağlantılıdır.
- **Ortak zemin:** "Kaptan" öneki rehberlik-yolculuk metaforunu taşır (Yolculuk Yıldızı evreniyle tutarlı); iki ad M-6 tek-ad standardına uyar, M-7 dürüst-not diliyle çelişmez (rehber var, puan yok). Adlar aile-özgü ayna çiftidir (F-2) — bu madde F-2'nin "yaratıcı alternatif adayları sahibin değerlendirmesindedir" hükmünün sahip kararıyla karşılığıdır.
**Yolculuk Yıldızı (v1.5 — K-738/K4 doktrini):** SEDUVA ve LEXIVA çocuk yüzeylerinde ilerleme biriminin tek adı; üç düğümde ortak (M-6 bir-kavram-bir-ad). Ödül-ekonomisi aracı DEĞİLDİR: ilerleme çocuğun kendi öz geçmişiyle kıyaslanır (birey-içi ilerleme — §1; ÜRÜN-MİMARİSİ §6.4/§6.9 ödül doktrini). Sayılar ilerleme göstergesi olarak görünür (ör. `+150 Yolculuk Yıldızı` · `Seviye 5 için son {n} Yolculuk Yıldızı`); puan/teşhis dili çocukta yasaktır (M-7 dürüst-not: "Burada puan yok. Nasıl yaptığını birlikte göreceğiz."). Kod düzeyindeki `currentXp`/`nextLevelXp`/`xpReward` alan adları teknik tanımlayıcı olarak kalır; çocukta GÖSTERİLMEZ (K-738 kaydı).

### I. Çocuk ↔ Veli ↔ Uzman Terim Eşlemesi (YENİ v1.4 — dış görüş raporu §5)
Görev-odaklı çocuk ifadesi; birebir eşanlamlılık şart DEĞİLDİR (M-13). "—" = çocuk yüzeyinde GÖSTERİLMEZ (M-14).

| Uzman terim | Çocuk yüzeyi | Veli yüzeyi |
|---|---|---|
| sürdürülebilir dikkat | İşine devam et | Dikkatini sürdürme |
| odak | Yaptığın işe bak | Odaklanma |
| dikkat kayması | Başka yere bakma | Dikkatin dağılması |
| göreve geri dönme | Yeniden işe dön | Göreve yeniden yönelme |
| tepki süresi | — (gösterilmez) | Tepki süresi |
| doğruluk | — (gösterilmez) | Doğru yanıt sayısı/oranı |
| hata oranı | — (gösterilmez) | Hata sayısı |
| performans | Görevi yap (yönerge) | Görevdeki sonuçlar |
| zaman algısı | Ne kadar süreceğini tahmin et | Süre tahmini |
| zamansal sapma | Tahminin ile gerçek süre arasındaki fark | Tahmin-gerçek süre farkı |
| kalibrasyon | Tahmin et, yap, sonra karşılaştır | Tahmin ile gerçekleşen sürenin karşılaştırılması |
| bilişsel gruplama | Bilgileri küçük parçalara ayır | Bilgiyi gruplama |
| çalışma belleği | Aklında tut | Bilgiyi kısa süreli akılda tutma |
| sınıflandırma | Benzer olanları bir araya koy | Bilgileri sınıflandırma |
| göreve başlama | İlk adımı yap | Göreve başlama |
| bilişsel esneklik | Kural değişince yeni kurala geç | Kural değişimine uyum |
| perseverasyon | Eski kuralda kalma | Eski kurala devam etme |
| inhibisyon / yanıt engelleme | Basmadan önce dur | Yanıtı durdurma |
| dürtüsel yanıt | Hemen basmak yerine bekle | Erken yanıt verme |
| SSRT | — (gösterilmez) | Durdurma süresi |
| commission error | — (gösterilmez) | Erken yanıt sayısı |
| bilişsel yük | — (gösterilmez) | Görev yükü |
| öz-düzenleme | Dur, nefes al, yeniden dene | Kendini düzenleme |
| stres | Zorlandığında (koşul) | Zorlanma |
| engellenme | İş istediğin gibi gitmediğinde (koşul) | Görev kaynaklı zorlanma |
| sosyal ipucu | Örnekteki ses ve yüze dikkat et (kamera/yüz analizi YOK — hazır materyal) | Sosyal ipuçlarını fark etme |
| prosodi | Sesin nasıl söylendiğine bak | Ses tonu ve vurgu |
| bölünmüş dikkat | Ekrana bak ve sesi dinle | İki kaynağa aynı anda dikkat |
| fonolojik farkındalık | Sesleri fark et | Ses farkındalığı |
| fonem / ses birimi | Kelimedeki sesi bul | Kelimedeki ses |
| başlangıç sesi | Kelimenin ilk sesi | İlk ses |
| hece | Kelimenin parçaları / heceler | Hece |
| fonolojik parçalama | Kelimeyi seslerine ayır | Sözcüğü seslerine ayırma |
| sentez / birleştirme | Sesleri birleştir | Sesleri birleştirme |
| görsel ayırt etme | Doğru harfi bul | Görsel ayırt etme |
| görsel arama | Aradığın harfi bul | Görsel arama |
| seçicilik | Hedefini bul | Hedef uyaranı seçme |
| akıcılık | Daha rahat oku | Okuma akıcılığı |
| doğru sözcük/dk | — (çocukta gösterilmez) | Dakikadaki doğru sözcük sayısı |
| tepki tutarlılığı | — (çocukta gösterilmez) | Yanıt tutarlılığı |
| ölçüm | Nasıl yaptığını birlikte görelim | Çocuğun görev sonuçlarını izleme |
| puan | Burada puan yok | — |
| paradigma | Görev | Etkinlik/görev |
| batarya | Görevler | Görev grubu |
| telemetri / katsayı / SD / ms / % / eşik-bant | — (çocukta gösterilmez) | — |

**Kullanım notu:** çocuk ifadesi görevle doğrudan ilişkili olmalı; teknik terim uzman yüzeyinde korunur; "—" terimler için çocuk yüzeyinde karşılık üretilmez. **Sütun semantiği (K-719):** Çocuk sütunu = çocuğa gösterilecek İFADE — eylem yönergesi VEYA koşul cümlesi olabilir; birebir tanım karşılığı DEĞİLDİR (M-13). " (yönerge)" = görev yönergesi; "(koşul)" = durum cümlesi. **Veli yüzeyindeki karşılıklar KAYIT GÖSTERİMİDİR; tanı/kapasite/bilişsel özellik/klinik yorum/"iyi-kötü" değerlendirmesi DEĞİLDİR** (M-14 veli sınırı — K-718). **Ölçüm-sonuç sorusu (K-720):** ölçüm SONUCUNU soran ifadeler çocuk yüzeyinde GÖSTERİLMEZ ("— (gösterilmez)"); çocuğa yalnız görev yönergesi (eylem) verilir; sonuç uzman+veli kartında yaşar.

### G. Yasak diller (K-295 Daimî-RED + K-02)
⛔ AI-HAM · Neural-Sync · Berard · Tomatis · Sağ Kulak Baskınlığı · Alfa dalgası · nörofeedback
⛔ prefrontal korteks · bazal ganglion · nöral ağ · beyin lobu · dopamin (nöro-anatomik iddia)
⛔ terapötik · Klinik Protokol · klinik tablo · tedavi/terapi (olumsuzlama şerhi dışında)
⛔ %100 uyum/başarı · tersine mühendislik
✅ İzinli karşılık: **"ses ortamı yönetimi (işitsel çeldirici azaltma)"** · **"yürütücü işlev"** · **"eğitsel"**

---

## 4) DÜRÜSTLÜK
- Sözlük **mevcut kullanımı derler**; yeni kavram icat etmez. Tanımlar kaynak belgelerden **birebir** alındı.
- **Hiçbir docx bu turda değiştirilmedi** — sözlük referans belgedir; uygulama ayrı karar.
- "Terminal" için **50 hit tarandı, hepsi tek tek okunmadı**; örneklem (14 bağlam) tutarlıydı.
- **Deep Work Station / Mobile Terminal / Satellite Hub** donanım katmanıdır; **pilotta kullanılmıyor** (yazılım-tek, K-374).
- Sözlüğün **kanonik statüye alınması** kullanıcı onayı ile KESİNLEŞTİ (K-722 · 10.09.2026); HARİTA satırı v1.4'e bağlandı (ölü v1.1 referansı kapatıldı).

~~~~

## Ek B — karar/ürün-belge bağlamı

Kararlar tarihî kapsamlarıyla okunur; aşağıdaki alıntılar bugünkü ürünün tüm işlevlerinin çalıştığına kanıt değildir.

~~~~markdown
### K-554 — 08.09.2026 — SCHOLARIA CANLI-EKRAN-TURU (kullanıcı: "neredeyse tüm menüler boş ve pasif" — 4-bulgu diskte-teyitli) — v0.2.2 ×3
**Bulgu (K-276 denetim):** SCHOLARIA v0.2.1 = temel-çatı: yalnız H-c TransferKartı canlı (6-state/3-click/localStorage); Cockpit=2-satırlık açıklama · EBA=yalnız [EBA POST]-etiketi · pano/sinif/izleme/ogrenci/ses/rapor/yardım statik; PCV-brifing v1.0 görev-A..H'nin yalnız D'si (H-c) ürünle-yapılabilir → PCV-HAZIR-değil iddiası.
**İcra (kullanıcı-kararı: tam_tur — 9-ekran):** YENİ: `data/seriler.ts` (seed'li sin-dalga deterministik-MOCK) · `ogretmen/Cockpit.tsx` (Fslope-satırları+renk-eşik ≥0.07 · d(SDRT)/dt sınıf-eğrisi · Nefes Halkası 4-4-4 + yönlendirme-kartı; cihaza-komut-yok şerhi) · `eba/EbaPaneli.tsx` (3-adım salt-okunur akış · yerel daily-insight TASLAĞI H-c-kaydından · "PLANLI ENTEGRASYON-gönderim-YOK" rozeti · Başarı-Notu-Yazılmaz/Maske-UID · K-331/K-334) · `ses/SesPaneli.tsx` (izolasyon-slider + dalga-görsel-simülasyonu; donanım-PLANLI şerhi) · `izleme/IzlemePaneli.tsx` (öğrenci-seçimi + kişi-eğrisi; K-14 akran-yok) · `rapor/RaporOzeti.tsx` (görev-H: H-c'den gözlemlenebilir-dil not-önizlemesi; yazdırma-YOK PCV-kural-1) · App.tsx yeniden-yazım: Pano tıklanır-nabız · Sınıf seçici↔veri+G_contrast eğrisi · Öğrenci görev-detay+dürtü-kilidi 3-sn demosu (PRD §3.B) · Yardım şerh-sözlüğü+hızlı-tur; Ayarlar bilinçli-statik (K-334).
**Derleme:** pkg 0.2.1→**0.2.2** · tsc 0 · single/pilot/tam ×3 → **DEMO 252.161 B `7df972e6…`** (rozet-izsiz — v0.2.1-DEMO-deseni) · **PILOT 252.510 B `71d09422a4b846f0…`** (rozetli) · **TAM 252.506 B `9b4a9e47…`** (rozetli) · single-check güncellendi (sürüm-0.2.2 +5-yeni-test: cockpit/eba-yok/rapor-H/dürtü-kilidi/ses) → **14/14 ×3** · Mentoria-0 ×3 · 14-bundle-grep ✓. v0.2.1 ×3 AYNEN (tarihî); rozet-injection v0.2.1-deseninden türetildi (title+data-k540, K-545→K-554).
**Zarf-02/brifing:** `SCHOLARIA-MVP-PCV_PILOT-v0.2.2.html` sha-eş (v0.2.1-kopya silindi) · **brifing v1.1** (sürüm+dosya-adı+v0.2.2-canlı-tur-notu; v1.0 tarihî) zarf-kopyasıyla · README-zarf ×5 (SCHOLARIA-satırları; MENTORIA/SUPPORTA v1.0-atıfları doğru-güncel).
**PCV-durumu:** brifing A–H görevleri artık ürünle-yapılabilir (D önceden canlıydı; A/B/C/E/F/G/H bu turda canlandı; H-deseni Rapor-ekranında). K-511: mühür v7.64.04 kullanıcı-talimatında.
~~~~

~~~~markdown
### K-558 — 08.09.2026 — YOL-2: SCHOLARIA BEP-HAZIRLIK (hedef-şablonu + probe-izgarası) — v0.2.4 ×3
**Kaynak:** K-556 Yol-2 — Frontline/Goalbook-deseninin sınır-uyarlaması.
**İcra:** `bep/BepHedef.tsx` YENİ — kazanım(62)→**BEP-hedef-şABLONU** üretimi (öğretmen-düzenler; "resmî BEP belgesi değildir" ×2-şerh; K-263-deseni) + **haftalık gözlem-probu izgarası** (4-hücre; 3-durum tıkla-dön: yok/kısmen/gözlemlendi; eğilim-yorumu/puan/karşılaştırma YOK — K-02/K-04/K-14) + ekosistem-köprüsü: "MENTORIA Z-17 TASLAK kanıt-paketine taşınır" (Z-17 tek-geçiş bilinçli; Mentoria™-0 kanama-yok) · nav 13→14 ('BEP Hazırlık'); localStorage `scholaria_bep_defteri_v024`.
**Derleme:** pkg 0.2.4 · tsc 0 · DEMO 291.045 B `65327af914227008…` · **PILOT 291.322 B `8cfec1ce2df4feee…`** · TAM 291.318 B `026ae711326fd38c…` — single-check **23/23 ×3** (+BEP ×2-test). v0.2.3 ×3 AYNEN.
**Zarf/brifing:** SCHOLARIA-PCV_PILOT-**v0.2.4** sha-eş · **brifing v1.3** (yeni görev-K: BEP Hazırlık) · README-zarf ×5 (PERSONA v0.2.5 + SCHOLARIA v0.2.4 + brifing v1.3; 0 eski-iz) · README-pilot v0.2.5-bölüm · README-TAM_v1.15.6.md. **K-511: mühür v7.64.05 kullanıcı-talimatında** (kapsam: K-557+K-558).
~~~~

~~~~markdown
### K-649 — 09.09.2026 — SEDUVA GÜNCELLEMESİ 2. ADIM: SCHOLARIA (OKUL) YÜZEYİNE FRICTION MAP EKLENMESİ
**Açıklama:** Mühür işleminin ardından, planın 2. adımı olan SCHOLARIA (Öğretmen/Okul) modülünün geliştirilmesine başlanmıştır.
**İcra:** 
1. `SEDUVA_SCHOLARIA/src/components/izleme` altına `FrictionMap.tsx` (Öğrenme Sürtünme Haritası) bileşeni kodlanacaktır. 
2. Bu bileşen, Persona'dan gelen verileri (Başlama/Sürdürme/Sonlandırma) 3 renkli bir ısı haritası olarak öğretmenin sınıf ekranına yansıtacaktır.
~~~~

~~~~markdown
### K-700 — 09.09.2026 — LEXIVA TAM UYARLAMA: MARKA + DOMAIN (SEDUVA KALINTILARI SIFIR)
**Açıklama:** Kullanıcı düzeltmesi: "Ürünler için SEDUVA yapıları aynen kopyaladın ancak LEXIVA için uyarlama yapılmadı." K-683 klonunda anlaşılan "marka hizalaması" kalemi yerine getirilmemişti; bu oturumda 4 düğümün tamamında marka (SEDUVA→LEXIVA) + domain (DEHB→ÖÖG/okuma-fonolojik, K-683 ürün tanımları) uyarlaması tamamlanmış ve 4 tek-dosya build v2.10.0 olarak yeniden üretilmiştir.
**İcra (düğüm düğüm):**
1. **Persona:** Kaptan Hece kahraman kimliği; uzman ekranı "Telemetri İnceleme + Resmî Sonuç İçe Aktarımı" (SNAP-IV/Vanderbilt/ADHD-RS-5/Conners-4/WFIRS-TR devredilmedi); ölçüm laboratuvarı 6 görev ailesi (SBA, Akıcılık M-4, Yazım hata sınıfı, MEB-M1, Sayı Blokları, Görsel Ayırt Etme); nav/rozet/splash "9 Paradigma/Kaptan Fokus" sızıntıları temiz; SBA + Harf Dedektifi + Süre Algısı (EQ-10) modülleri; telemetri `lexiva_telemetry_*.jsonl`. Smoke (123 madde) LEXIVA'ya hizalandı: 123/123 geçiyor, konsol hatası 0.
2. **Supporta:** BGM-12 DEHB yürütücü-işlev menüsü **devredilmedi** → EQ-01..EQ-12 okuma/fonolojik içerik menüsü (Ses Merdiveni, SBA, Hece, Harf Çizim, Söyleneni Yaz, Akıcılık M-4, Sözcük Çantası, Anlama, Sayı Blokları, Süre Algısı, Transfer, Okuma Özerkliği); `dehbAlan`→`okumaAlani`; K-02/K-04 dürüstlük şerhleri korundu; AILE kartları MEB ÖGG Aile Rehberi kaynaklı. Smoke 127/127.
3. **Mentoria:** veri katmanı kalan DEHB kalıntıları (Dikkat Bahçesi/FS-1-CC-3, Zaman Kutusu, "Bağlam Kaydı dikkat") LEXIVA görevlerine (Hece Avcısı/ETK-02, Sesli Okuma M-4, "Bağlam Kaydı okuma") çevrildi; etkinlik kataloğu (ETK-01..) ve resmi sonuç kanalı zaten uyumlu. Build temiz.
4. **Scholaria:** B2B sınıf düğümü = Bilişsel Gelişim Laboratuvarı; DEHB metrik yüzeyi (GFI/Fslope/d(SDRT)/dt, Gaze-Lock, Dynamic Gating, Görsel Dikkat/Bölünmüş Dikkat görevleri, Nefes Halkası) → katılım/yorgunluk eğimi/yanıt zamanı eğrisi, görev etkileşim oranı, sınıf ritim eğrisi, Sayı Blokları/Ritim-Hece Avcısı görevleri, Nefes Molası (4-4-4). Smoke 12/12.
**Doğrulama:** 4 HTML'de DEHB/ölçek/paradigma token taraması: **sıfır** (istisna: Persona'da PilotKapsamDisi K-02 dürüstlük notundaki "SEDUVA DEHB bataryası devredilmedi" cümlesi — bilinçli kalıntı, K-02 kanonu). package.json sürümleri 2.10.0; `__SURUM__` hizalı. tsc: 4 düğümde 0 hata.
**Artefaktlar:** `LEXIVA-PERSONA-v2.10.0.html` (1.448.597 B) · `LEXIVA-SUPPORTA-v2.10.0.html` (320.174 B) · `LEXIVA_MENTORIA-v2.10.0.html` (423.696 B) · `LEXIVA-SCHOLARIA-v2.10.0.html` (300.596 B) — kök dizinleri + `LEXIVA-TAM-v2.10.0.zip` (360 dosya; SHA-256: c512888dd4e740df09c98e13a3387e92ae45c1a2434a8e5d76fa45b4df4359ab).
**Mühür (kullanıcı talimatı 09.09.2026):** `VAMOLA ÇALIŞMALARI — v7.65.16.zip` (sha256 `e2c9143122ec86542195837326b62f33142576e68989770847b194b839aac9af`) + `SHA256-MANIFEST_v7.65.16.json` (1.042 dosya, sha256 `3489f9cf4584c89660f842744ad40fca123e317c027a757dca7f853e6c25fc77`); TESLIM-KAYDI.md v7.65.16 kaydı açıldı.
**Ders (tekrarlayan hata):** marka grep ≠ domain grep; census token listesi görev adlarını da içermeli ve final doğrulama build-HTML üzerinde domain-vokabül taramasıyla kapanmalı. Kopyala-uyarla operasyonlarında smoke-test de "ürünün" parçasıdır; LEXIVA smoke hizalaması bu kararın kapsamındadır.
~~~~

~~~~markdown
### K-709 — 10.09.2026 — ONAYLI MENÜ-JARGON LİSTESİ KONTROLÜ + TAMAMLAMA (İKİ AİLE, 8 DÜĞÜM)
**Sahibin tespiti:** konuşmada kararlaştırılan isim değişikliklerinin bir kısmı SEDUVA ve LEXIVA'da uygulanmamıştı (örnek: **Navigator → Klinik Rehber**). K-708 turunda benim "Vaka Yönlendirici" adımı YANLIŞTI — sahibin onaylı listesi kanoniktir; "Klinik Rehber" uygulandı.
**Denetim (8 düğüm, src+build):** onaylı liste madde-madde tarandı: 18 isim (8 jargon + 4 modül + 6 Scholaria). Bulgular:
- **SEDUVA-MENTORIA:** 5 eksik — "Vaka Yönlendirici" (yanlış isim) 5 yerde · "Öğretmen Senkron" ekran h2+glossary 2 · "Pedagojik Değerlendirme Bataryası" 10 UI string (nav "Değerlendirme Ölçekleri" idi, ekran h2+rapor+yazdır+prose hâlâ eski) · "Trend" prose 2 · kurum ekranı h2 "Kurum" (nav "Uzman Masası" ile uyuşmaz) · bayat K-550 yorumu (K-660'a çelişki).
- **LEXIVA-MENTORIA:** neredeyse TAMAM — nav 7 eski isim (Navigator · Kanıt (Z-12/Z-17) · Aile (5N1K) · MEB Hizalama · Öğretmen Senkron · Tam (Admin) · Kanıt İzleme (T1/T2)) + pano/kurum ×2 dup + 3 ekran h2'si (Guidance Navigator — Oİ/GT/G_growth · MEB Hizalama — 2021 DEP · Öğretmen Senkron) + glossary 3 + 2 Z-12 UI + **15 YASA- user-visible string** (klon, SEDUVA temizliği öncesinden geldi).
- **Scholaria (İKİ aile):** nav "Gelişim İzleme" → onaylı "Gelişim Takibi" (ekran h2 zaten doğruydu) + nav "Yardım" → onaylı "Sistem Kılavuzu ve Terimler" (ekran h2 zaten doğruydu) · LEXIVA Portfoy'da "(Veli Köprüsü)" kalıntısı 1.
- **Supporta + Persona (İKİ aile):** düzeltme GEREKMİYOR — eski hitler yalnız kod tanımlayıcıları (Pano bileşeni · ParentDashboard/TeacherDashboard/ExpertDashboard · id'ler); yüzey etiketleri zaten onaylı isimler (Eğitmen Kürsüsü ✓ · Gelişim Özeti ✓).
**Uygulanan:**
- **SEDUVA-MENTORIA → v1.5.5:** Klinik Rehber (nav+panel+başlık+boş-durum+glossary 5) · Öğretmen Eşleme (h2+glossary) · "Pedagojik Değerlendirme Bataryası"→"Değerlendirme Ölçekleri" (10 UI: ekran h2, danışan notu, grafik, rapor prose+başlık, B-4, yazdır başlığı) · "Trend"→"Gelişim Grafiği" (2 prose) · kurum ekranı h2 "Uzman Masası" (nav ile uyum) · bayat K-550 yorumu → K-660.
- **LEXIVA-MENTORIA → v2.11.1:** nav 7 rename + **pano dashboard KORUNDU** (LEXIVA'da pano ÖLÜ DEĞİLDİ — K-700 uyumlu, temiz kopyalı Uzman Masası danışan-kartları paneli; dup çözümü: pano="Uzman Masası", kurum="Kurum") · ekran h2'leri (Klinik Rehber — Oİ/GT/Gelişim Hızı · MEB İle Uyumlama (2021 DEP · salt-okunur) · Öğretmen Eşleme) · glossary 3 · 2 Z-12 UI stringi düştü · **15 YASA- UI stringi temizlendi** (anlam korundu; SEDUVA v1.5.4 emsali) · tsc hatası (ölü 'pano' karşılaştırması) pano'yu geri almayla doğal olarak çözüldü.
- **SEDUVA-SCHOLARIA → v0.2.7 + LEXIVA-SCHOLARIA → v2.10.1:** nav "Gelişim Takibi" + "Sistem Kılavuzu ve Terimler" · LEXIVA Portfoy "(Veli Köprüsü)"→"(Aile Bilgilendirme)".
**Doğrulama:** tsc **4/4 TEMİZ** · smoke: LEXIVA-MENTORIA **12/12** · SEDUVA-SCHOLARIA **12/12** · LEXIVA-SCHOLARIA **12/12** (hardcoded "sürüm rozeti 2.10.0" kontrolü K-368'e çekildi: package.json'dan okur) · 4 build içeriği: eski isimlerin **tümü 0**, yeni isimler >0 (Klinik Rehber 5/5 · Değerlendirme Ölçekleri 12 · Uzman Masası 2/2 · Gelişim Takibi 2/2 · Sistem Kılavuzu ve Terimler 2/2 · YASA-=0/0) · SEDUVA SUPPORTA/MENTORIA-smake dokunulmadı (v1.5.5/v0.2.7 öncesi yeşil geçerli).
**Kanon-notu:** sahibin onaylı isim listesi (bu mesaj + K-659..667) tek kanoniktir; agent-önerisi isimler (örn. "Vaka Yönlendirici", "Gözlem İzleme") sahibin listesiyle çakışıyorsa sahibin listesi geçerlidir.
**Mühür:** v7.65.23 çifti tarama ÖNCE silindi (K-706; SHA zincirde) → **v7.65.24** (TESLIM-KAYDI'da).
~~~~

### Tarihî kapsam kaynakları / güncel derleme ayrımı

- LEX: `VAMOLA - Lexiva/LEXIVA_SCHOLARIA/LEXIVA-SCHOLARIA-KAPSAM-BELGESI_v1.0.md` — K-450 faz-A ve sınırlara ilişkin tarihî belge; §3 eski envanter bugün “yok” kanıtı değildir. K-700 alan uyarlaması ve K-709 güncel menü adları ayrıca okunur.
- SED: `VAMOLA - Seduva/SEDUVA_SCHOLARIA/VAMOLA_EDULABS_SEDUVA_SCHOLARIA_PRD_v1.3.docx` — hedef mimari/kurumsal master şartname. §2 donanım, §3 analitik, §4 SSO/PUT/optimize-etti iddiaları mevcut TAM'ın işlev kanıtı değildir. Gizlilik ibaresi taşıyan PRD bu dış briefte bütünüyle çoğaltılmadı; paylaşım iznini sahibi ayrıca değerlendirir.
- SED PCV: `VAMOLA - Seduva/SEDUVA_BELGELER/VAMOLA-PCV-BRIFINGI-SCHOLARIA_v1.4.md` — görev/oturum protokolü ayrı belgedir; bu turun TAM kanıtıyla eski pilot profili karıştırılmaz.
- Her iki ürün README'si tarihî sürüm satırları taşır; güncel sürüm package.json ve mevcut TAM rozetiyle çapraz kontrol edildi. Bu belgeler değiştirilmedi.
- Haricî MEB/API/pedagoji/bilim/telif kaynakları bu hazırlıkta web üzerinden yeniden doğrulanmadı. Alıntılanan yerel belgelerin atıfları dış kaynak doğrulaması diye sunulmaz.

## Ek C — ürün-başı DOM, kaynak havuzu ve tam ham bağlam

# Ek C-LEX — SCHOLARIA-LEX bağımsız kanıt paketi

## C-LEX-1 — 25 DOM durumu

Tarayıcı tarihi/saatleri test anını gösterir. ÖĞR/ARD ve benzeri kodlar üründeki sentetik örneklerdir; test notu gerçek öğrenciye ait değildir.

### SCH-LEX-DOM-nav-pano

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf Özeti (Shared Evidence Akışı)

Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır.

2A Sınıfı
Yok
Öğr. Sayı: 2 · Ort. Y-Eğim: 0.04
Gün-içi nabzı aç →
2B Sınıfı
Yorgunluk Uyarısı
Öğr. Sayı: 1 · Ort. Y-Eğim: 0.07
Gün-içi nabzı aç →
4A Sınıfı
Yok
Öğr. Sayı: 1 · Ort. Y-Eğim: 0.04
Gün-içi nabzı aç →

MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde.
~~~~

### SCH-LEX-DOM-nav-sinif

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf (Sınıf Ritim Eğrisi)

Ders esnasında sınıf içi gürültü ve çeldirici dengesi. Seçili sınıfın göstergeleri:

Hedef Sınıf:
SUB-2A
SUB-2B
SUB-4A
Aktif Parametre: Sınıf Ritim Eğrisi (sentetik) — 0.31 · 2A · Öğrenci 2 · Ort. Y-Eğim 0.04 [PRD §3.A deseninden MOCK]
Ritim eğrisi — gün içi (sentetik-gösterim)
ARD-05
Katılım 0.82 · Y-Eğim 0.03 · görev PVC-101
ARD-06
Katılım 0.75 · Y-Eğim 0.05 · görev PVC-102
~~~~

### SCH-LEX-DOM-nav-ogrenci

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğrenci (Cihaz & Olay Dinleyicileri)

Öğrenci Terminal UI. EventListener başlama-kilitleri (PRD §3.B) planlı başlamayı gösterir — mini-simülasyonda deneyin.

Matematik: Sayı Blokları Eşleştirme
MAT-2 | M1
Hareket: Ritim ve Süre Tahmini
HKM-2 | M2
Türkçe: Hece Avcısı (Okuma)
TUR-2 | M3
~~~~

### SCH-LEX-DOM-nav-ogretmen

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Y-Eğim ≥ 0.07 → Nefes Molası.
Toplu Yorgunluk Eğimi — 2A
ARD-05
Y-Eğim 0.03
Katılım 0.82
ARD-06
Y-Eğim 0.05
Katılım 0.75
Yanıt zamanı eğimi sınıf-eğrisi (sentetik-gösterim)
Nefes Molası (4-4-4)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
YZ Önerisi İste
~~~~

### SCH-LEX-DOM-nav-transfer

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Transfer Gözlem Kartı

Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.

Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).

MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
Öğrenci (sentetik):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Gözlenen etkinlik:
Matematik: Sayı Blokları Eşleştirme
Hareket: Ritim ve Süre Tahmini
Türkçe: Hece Avcısı (Okuma)
Gözlenen davranışlar (işaretleyerek):
○ Göreve kendi başladı (yönlendirme olmadan)○ Zorlanınca ipucu istedi ve sürdürdü○ Mola verdi ve döndü (akışı korudu)○ Sözel yönerge tek başına yeterli oldu
Kısa not (isteğe bağlı):
Kaydet (yerel)
0 kayıt · yalnız bu tarayıcıda
~~~~

### SCH-LEX-DOM-nav-ders

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Matematik: Sayı Blokları Eşleştirme
Hareket: Ritim ve Süre Tahmini
Türkçe: Hece Avcısı (Okuma)
Ders-işleme yönergesi (MAT.2.1.1): Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (0)

Defter boş — yukarıdan atama işleyin.

Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-LEX-DOM-nav-veli

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Aile Bilgilendirme

Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.

Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).

Haftalık Aile Bülteni — TASLAK
2A
2B
4A
Bülten taslağı üret

Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.

Veli Görüşme — Randevu Defteri
Haftalık gözlem paylaşımı
H-c kart-turu değerlendirme paylaşımı
Gelişim-görüşmesi (gözlem-özetli)
Diğer
Randevu kaydet

Defter boş — randevu kaydedin.

Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.
~~~~

### SCH-LEX-DOM-nav-bep

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
BEP Hazırlık

Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.

Sınır-şerhi: Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
Hedef-şablonu üretimi
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Hedef-şablonunu deftere ekle

Defter boş — yukarıdan hedef-şablonu üretin.
~~~~

### SCH-LEX-DOM-nav-eba

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
MEB EBA Entegrasyonu

Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.

Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:

1 · Cihaz (Terminal)
EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
2 · daily-insight TASLAĞI
Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
3 · [EBA POST] /api/v1/report/daily-insight
PLANLI ENTEGRASYON — bu önizlemede gönderim YOK
K-331: salt-okunur çağrı — ödev/içerik yazılmaz
e-sınav girişi YOK
K-334: idari-mali otomasyon dışarı
Başarı Notu Yazılmaz · Maskeli UID
Insight Taslağı Üret (yerel)

OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
~~~~

### SCH-LEX-DOM-nav-izleme

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Gelişim Takibi

Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin.

MOCK: seriler sentetik-gösterimdir (K-05); XR/Görev-panosu Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Yanıt zamanı eğimi — ARD-05 (12 gözlem-noktası)
Görev etkileşim oranı: %88.4 (sentetik-sabit · Faz-3 Görev-M11)
Aktif görev: PVC-101 · Katılım: 0.82 · Y-Eğim: 0.03
K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.
Gelişim-takibi (gözlem-çizelgesi) — ARD-05
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Katılım/Y-Eğim serisi (MOCK-gösterim)
Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04).
H-c gözlem-zaman-çizelgesi (0 kayıt)

Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun.
~~~~

### SCH-LEX-DOM-nav-ses

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf İçi Ses Yönetimi

Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın.

PLANLI-KATMAN şerhi: donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü ayrımının görsel-simülasyonu vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik).
Ana Sinyal İzolasyonu — 60%
ana-sinyal
ortam-gürültüsü (izolasyon-arttıkça söner)
Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır)
~~~~

### SCH-LEX-DOM-nav-rapor

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

### SCH-LEX-DOM-nav-ayarlar

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ayarlar

Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır.

2. Sınıf A Şubesi (24 slot)
2. Sınıf B Şubesi (22 slot)
4. Sınıf A Şubesi (25 slot)

MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda.
~~~~

### SCH-LEX-DOM-nav-yardim

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sistem Kılavuzu ve Terimler

Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu.

K-05: Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır.
K-02: Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil.
K-331: MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok.
K-334: Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok).
K-05/MOCK: ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez.
MOCK-değerleri: {"idariMaliKapsamDisi":true,"mebEbaSaltOkunur":true,"kvkkYerelMaskeleme":true,"telifiSifir":true,"surum":"v0.1.0"}
Hızlı-tur (PCV-brifing A–H ile uyumlu): ① Pano'dan bir sınıf-kartına tıkla (nabız) → ② Sınıf'ta ritim eğrisini oku → ③ Öğrenci'de başlama-kilidi demosu → ④ Transfer Gözlem (H-c): kartı 2 kez doldur (30-sn hedefi) → ⑤ Cockpit'te yorgunluk-satırları + Nefes Molası → ⑥ EBA'da salt-okunur akış + insight-taslağı → ⑦ Rapor'da görev-H not-önizlemesi → ⑧ Ses/İzleme'de sentetik-gösterimler.
~~~~

### SCH-LEX-DOM-ogrenci-gorev-detay

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğrenci (Cihaz & Olay Dinleyicileri)

Öğrenci Terminal UI. EventListener başlama-kilitleri (PRD §3.B) planlı başlamayı gösterir — mini-simülasyonda deneyin.

Matematik: Sayı Blokları Eşleştirme
MAT-2 | M1
Hareket: Ritim ve Süre Tahmini
HKM-2 | M2
Türkçe: Hece Avcısı (Okuma)
TUR-2 | M3
Matematik: Sayı Blokları Eşleştirme — Terminal önizlemesi (MOCK)

Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): aceleci tıklama yerine planlı başlama.

Göreve Başla (kilit-demosu)Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir.
~~~~

### SCH-LEX-DOM-transfer-kayitli

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Transfer Gözlem Kartı

Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.

Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).

MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
Öğrenci (sentetik):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Gözlenen etkinlik:
Matematik: Sayı Blokları Eşleştirme
Hareket: Ritim ve Süre Tahmini
Türkçe: Hece Avcısı (Okuma)
Gözlenen davranışlar (işaretleyerek):
○ Göreve kendi başladı (yönlendirme olmadan)○ Zorlanınca ipucu istedi ve sürdürdü○ Mola verdi ve döndü (akışı korudu)○ Sözel yönerge tek başına yeterli oldu
Kısa not (isteğe bağlı):
Kaydet (yerel)
1 kayıt · yalnız bu tarayıcıda
Son kayıtlar:
hepsini temizle
ARD-05 · Matematik: Sayı Blokları Eşleştirme · 1 davranış · “SENTETIK BRIEF TESTI — gerçek öğrenci değildir.” (10.09.2026 23:27:39)
~~~~

### SCH-LEX-DOM-rapor-kayitli

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

### SCH-LEX-DOM-eba-taslak

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
MEB EBA Entegrasyonu

Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.

Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:

1 · Cihaz (Terminal)
EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
2 · daily-insight TASLAĞI
Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
3 · [EBA POST] /api/v1/report/daily-insight
PLANLI ENTEGRASYON — bu önizlemede gönderim YOK
K-331: salt-okunur çağrı — ödev/içerik yazılmaz
e-sınav girişi YOK
K-334: idari-mali otomasyon dışarı
Başarı Notu Yazılmaz · Maskeli UID
Insight Taslağı Üret (yerel)

OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
~~~~

Alan `eba-taslagi` · readOnly=True

~~~~text
GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez)
Tarih: 2026-09-10 · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02)

• ••• (maske-UID ÖĞR-•••) — görev: 1 davranış-gözlemi; ör. "Göreve kendi başladı (yönlendirme olmadan)" (gözlemlenebilir-sayılabilir dil).

[Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA'ya yazma-yok]
~~~~

### SCH-LEX-DOM-veli-kayitli

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Aile Bilgilendirme

Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.

Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).

Haftalık Aile Bülteni — TASLAK
2A
2B
4A
Bülten taslağı üret

Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.

Veli Görüşme — Randevu Defteri
Haftalık gözlem paylaşımı
H-c kart-turu değerlendirme paylaşımı
Gelişim-görüşmesi (gözlem-özetli)
Diğer
Randevu kaydet

Defter boş — randevu kaydedin.

Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.
~~~~

### SCH-LEX-DOM-yz-oneri

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Y-Eğim ≥ 0.07 → Nefes Molası.
Toplu Yorgunluk Eğimi — 2A
ARD-05
Y-Eğim 0.03
Katılım 0.82
ARD-06
Y-Eğim 0.05
Katılım 0.75
Yanıt zamanı eğimi sınıf-eğrisi (sentetik-gösterim)
Nefes Molası (4-4-4)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı)

Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin.

Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.
İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma.
Nefes Molası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.
Yer-seçimi: çeldirici-anında öne-yakın sessiz-masa önerin.
Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin.
✓ Onayla ve Yürürlüğe Al
✕ Reddet ve Gerekçelendir
~~~~

Alan `oneri-notu` · readOnly=True

~~~~text
EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · ARD-05 · 2A):
• Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.
• Nefes Molası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.

⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer.
~~~~

### SCH-LEX-DOM-yz-reddet

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Y-Eğim ≥ 0.07 → Nefes Molası.
Toplu Yorgunluk Eğimi — 2A
ARD-05
Y-Eğim 0.03
Katılım 0.82
ARD-06
Y-Eğim 0.05
Katılım 0.75
Yanıt zamanı eğimi sınıf-eğrisi (sentetik-gösterim)
Nefes Molası (4-4-4)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)

YZ Önerisi Öğretmen Tarafından Reddedildi

Kaydet
~~~~

### SCH-LEX-DOM-bep-taslak-probe

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
BEP Hazırlık

Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.

Sınır-şerhi: Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
Hedef-şablonu üretimi
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Hedef-şablonunu deftere ekle
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
sil
Haftalık gözlem-probu izgarası (1/4):
H1 · 2026-09-10 · yok
+ haftalık-probe ekle

İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14).
~~~~

Alan `bep-sablon-metin` · readOnly=True

~~~~text
GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir)
Öğrenci: ARD-05 (maske-ÖĞR) · Kazanım: MAT.2.1.1 — Sayı postası: oku-yaz-eşle

Hedef-cümlesi (gözlemlenebilir-dil, K-14): ARD-05, sayı postası: oku-yaz-eşle kazanımına bağlı sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.

İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara.
Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır.
~~~~

### SCH-LEX-DOM-ders-atamali

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Matematik: Sayı Blokları Eşleştirme
Hareket: Ritim ve Süre Tahmini
Türkçe: Hece Avcısı (Okuma)
Ders-işleme yönergesi (MAT.2.1.1): Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (1)
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
Matematik: Sayı Blokları Eşleştirme · 2026-09-10
sil
Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-LEX-DOM-ders-turkce

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Matematik: Sayı Blokları Eşleştirme
Hareket: Ritim ve Süre Tahmini
Türkçe: Hece Avcısı (Okuma)
Ders-işleme yönergesi (T.D.1.1): Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (1)
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
Matematik: Sayı Blokları Eşleştirme · 2026-09-10
sil
Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-LEX-DOM-portfoy-atamali

~~~~text
LEXIVA Scholaria: Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).

v2.10.1 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

## C-LEX-2 — Kaynak metin adayları

ID kaynağın bu tarihteki satırına bağlıdır; refactor sonrası satır kayabilir. JSX/template parçası birebir tam cümle değildir.

| ID | Kaynak:satır | Tür | Ham parça (↵=satır sonu) | Görünürlük sınıfı |
|---|---|---|---|---|
| SCH-LEX-0001 | `App.tsx:42` | StringLiteral | B2B Yönetici | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0002 | `App.tsx:44` | JsxText | · VAMOLA Scholaria - Öğretmen Sınıf Panosu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0003 | `App.tsx:49` | JsxText | Sınıf Özeti (Shared Evidence Akışı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0004 | `App.tsx:50` | JsxText | Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0005 | `App.tsx:57` | JsxText | Sınıfı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0006 | `App.tsx:60` | JsxText | Öğr. Sayı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0007 | `App.tsx:60` | JsxText | · Ort. Y-Eğim: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0008 | `App.tsx:61` | JsxText | Gün-içi nabzı aç → | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0009 | `App.tsx:65` | JsxText | MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0010 | `App.tsx:71` | JsxText | Sınıf (Sınıf Ritim Eğrisi) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0011 | `App.tsx:72` | JsxText | Ders esnasında sınıf içi gürültü ve çeldirici dengesi. Seçili sınıfın göstergeleri: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0012 | `App.tsx:74` | JsxText | Hedef Sınıf: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0013 | `App.tsx:85` | JsxText | Aktif Parametre: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0014 | `App.tsx:85` | JsxText | Sınıf Ritim Eğrisi (sentetik) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0015 | `App.tsx:85` | TemplateHead | Öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0016 | `App.tsx:85` | TemplateMiddle | · Ort. Y-Eğim | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0017 | `App.tsx:85` | JsxText | [PRD §3.A deseninden MOCK] | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0018 | `App.tsx:87` | JsxText | Ritim eğrisi — gün içi (sentetik-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0019 | `App.tsx:95` | JsxText | Katılım | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0020 | `App.tsx:95` | JsxText | · Y-Eğim | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0021 | `App.tsx:95` | JsxText | · görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0022 | `App.tsx:107` | JsxText | Gelişim Takibi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0023 | `App.tsx:108` | JsxText | Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0024 | `App.tsx:116` | JsxText | Öğrenci (Cihaz & Olay Dinleyicileri) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0025 | `App.tsx:117` | JsxText | Öğrenci Terminal UI. EventListener başlama-kilitleri (PRD §3.B) planlı başlamayı gösterir — mini-simülasyonda deneyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0026 | `App.tsx:132` | JsxText | — Terminal önizlemesi (MOCK) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0027 | `App.tsx:133` | JsxText | Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): aceleci tıklama yerine planlı başlama. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0028 | `App.tsx:137` | TemplateHead | Kilit — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0029 | `App.tsx:137` | StringLiteral | Göreve Başla (kilit-demosu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0030 | `App.tsx:139` | JsxText | Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0031 | `App.tsx:148` | JsxText | Öğretmen Paneli (Teacher Cockpit) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0032 | `App.tsx:158` | JsxText | Ders & Görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0033 | `App.tsx:159` | JsxText | 2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0034 | `App.tsx:167` | JsxText | BEP Hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0035 | `App.tsx:168` | JsxText | Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0036 | `App.tsx:175` | JsxText | Aile Bilgilendirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0037 | `App.tsx:176` | JsxText | Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0038 | `App.tsx:177` | JsxText | Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0039 | `App.tsx:184` | JsxText | MEB EBA Entegrasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0040 | `App.tsx:185` | JsxText | Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0041 | `App.tsx:186` | JsxText | Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0042 | `App.tsx:193` | JsxText | Sınıf İçi Ses Yönetimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0043 | `App.tsx:194` | JsxText | Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0044 | `App.tsx:201` | JsxText | Rapor | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0045 | `App.tsx:209` | JsxText | Ayarlar | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0046 | `App.tsx:210` | JsxText | Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0047 | `App.tsx:213` | JsxText | slot) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0048 | `App.tsx:216` | JsxText | MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0049 | `App.tsx:222` | JsxText | Sistem Kılavuzu ve Terimler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0050 | `App.tsx:223` | JsxText | Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0051 | `App.tsx:225` | JsxText | K-05: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0052 | `App.tsx:225` | JsxText | Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0053 | `App.tsx:226` | JsxText | K-02: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0054 | `App.tsx:226` | JsxText | Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0055 | `App.tsx:227` | JsxText | K-331: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0056 | `App.tsx:227` | JsxText | MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0057 | `App.tsx:228` | JsxText | K-334: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0058 | `App.tsx:228` | JsxText | Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0059 | `App.tsx:229` | JsxText | K-05/MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0060 | `App.tsx:229` | JsxText | ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0061 | `App.tsx:230` | JsxText | MOCK-değerleri: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0062 | `App.tsx:233` | JsxText | Hızlı-tur (PCV-brifing A–H ile uyumlu): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0063 | `App.tsx:233` | JsxText | ① Pano'dan bir sınıf-kartına tıkla (nabız) → ② Sınıf'ta ↵             ritim eğrisini oku → ③ Öğrenci'de başlama-kilidi demosu → ④ | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0064 | `App.tsx:234` | JsxText | Transfer Gözlem (H-c) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0065 | `App.tsx:234` | JsxText | : kartı 2 kez doldur ↵             (30-sn hedefi) → ⑤ Cockpit'te yorgunluk-satırları + Nefes Molası → ⑥ EBA'da salt-okunur akış + insight-taslağı ↵             → ⑦ Rapor'da görev-H not-önizlemesi → ⑧ Ses/İzleme'de sentetik-gösterimler. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0066 | `components/bep/BepHedef.tsx:20` | StringLiteral | kısmen | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0067 | `components/bep/BepHedef.tsx:20` | StringLiteral | gözlemlendi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0068 | `components/bep/BepHedef.tsx:31` | FirstTemplateToken | GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0069 | `components/bep/BepHedef.tsx:32` | TemplateHead | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0070 | `components/bep/BepHedef.tsx:32` | TemplateMiddle | (maske-ÖĞR) · Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0071 | `components/bep/BepHedef.tsx:33` | TemplateHead | Hedef-cümlesi (gözlemlenebilir-dil, K-14): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0072 | `components/bep/BepHedef.tsx:33` | LastTemplateToken | kazanımına bağlı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0073 | `components/bep/BepHedef.tsx:34` | TemplateHead | sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0074 | `components/bep/BepHedef.tsx:35` | FirstTemplateToken | İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0075 | `components/bep/BepHedef.tsx:36` | FirstTemplateToken | Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0076 | `components/bep/BepHedef.tsx:59` | JsxText | Sınır-şerhi: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0077 | `components/bep/BepHedef.tsx:59` | JsxText | Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu ↵         taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0078 | `components/bep/BepHedef.tsx:64` | JsxText | Hedef-şablonu üretimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0079 | `components/bep/BepHedef.tsx:66` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0080 | `components/bep/BepHedef.tsx:71` | JsxText | Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0081 | `components/bep/BepHedef.tsx:79` | JsxText | Hedef-şablonunu deftere ekle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0082 | `components/bep/BepHedef.tsx:85` | JsxText | Defter boş — yukarıdan hedef-şablonu üretin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0083 | `components/bep/BepHedef.tsx:94` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0084 | `components/bep/BepHedef.tsx:99` | JsxText | Haftalık gözlem-probu izgarası ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0085 | `components/bep/BepHedef.tsx:102` | StringLiteral | tıkla: durum değişir (yok→kısmen→gözlemlendi) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0086 | `components/bep/BepHedef.tsx:109` | JsxText | + haftalık-probe ekle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0087 | `components/bep/BepHedef.tsx:113` | JsxText | İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0088 | `components/defter/SonucNotu.tsx:31` | JsxText | Sınav/gözlem Sonuç-Notu Defteri (sınırlı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0089 | `components/defter/SonucNotu.tsx:33` | JsxText | Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. ↵         Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0090 | `components/defter/SonucNotu.tsx:38` | StringLiteral | ör. "Pazartesi kısa-sayma-yazılısı — sınıf-geneli notu defterimde" (kategori-yazmayın) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0091 | `components/defter/SonucNotu.tsx:40` | JsxText | Deftere yaz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0092 | `components/defter/SonucNotu.tsx:44` | JsxText | Defter boş. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0093 | `components/defter/SonucNotu.tsx:48` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0094 | `components/ders/GorevAtama.tsx:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0095 | `components/ders/GorevAtama.tsx:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0096 | `components/ders/GorevAtama.tsx:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0097 | `components/ders/GorevAtama.tsx:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0098 | `components/ders/GorevAtama.tsx:40` | JsxText | kazanım-ağacı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0099 | `components/ders/GorevAtama.tsx:40` | JsxText | kazanım (Matematik 25 + Türkçe 37). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0100 | `components/ders/GorevAtama.tsx:45` | JsxText | Ders: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0101 | `components/ders/GorevAtama.tsx:46` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0102 | `components/ders/GorevAtama.tsx:47` | JsxText | Matematik (25) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0103 | `components/ders/GorevAtama.tsx:49` | JsxText | Türkçe (37) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0104 | `components/ders/GorevAtama.tsx:53` | JsxText | Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0105 | `components/ders/GorevAtama.tsx:58` | JsxText | Öğrenci (maskeli): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0106 | `components/ders/GorevAtama.tsx:63` | JsxText | Etkinlik: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0107 | `components/ders/GorevAtama.tsx:71` | JsxText | Ders-işleme yönergesi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0108 | `components/ders/GorevAtama.tsx:76` | JsxText | Atamayı deftere işle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0109 | `components/ders/GorevAtama.tsx:79` | JsxText | Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması ↵           PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0110 | `components/ders/GorevAtama.tsx:85` | JsxText | Atama-defteri ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0111 | `components/ders/GorevAtama.tsx:87` | JsxText | Defter boş — yukarıdan atama işleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0112 | `components/ders/GorevAtama.tsx:99` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0113 | `components/ders/OneriSablonlari.tsx:10` | StringLiteral | Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0114 | `components/ders/OneriSablonlari.tsx:11` | StringLiteral | İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0115 | `components/ders/OneriSablonlari.tsx:12` | StringLiteral | Nefes Molası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0116 | `components/ders/OneriSablonlari.tsx:13` | StringLiteral | Yer-seçimi: çeldirici-anında öne-yakın sessiz-masa önerin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0117 | `components/ders/OneriSablonlari.tsx:14` | StringLiteral | Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0118 | `components/ders/OneriSablonlari.tsx:26` | TemplateHead | EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0119 | `components/ders/OneriSablonlari.tsx:28` | FirstTemplateToken | ⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0120 | `components/ders/OneriSablonlari.tsx:32` | JsxText | Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0121 | `components/ders/OneriSablonlari.tsx:33` | JsxText | YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0122 | `components/ders/OneriSablonlari.tsx:36` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0123 | `components/ders/OneriSablonlari.tsx:40` | JsxText | YZ Önerisi İste | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0124 | `components/ders/OneriSablonlari.tsx:46` | JsxText | BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0125 | `components/ders/OneriSablonlari.tsx:47` | JsxText | Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0126 | `components/ders/OneriSablonlari.tsx:61` | JsxText | ✓ Onayla ve Yürürlüğe Al | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0127 | `components/ders/OneriSablonlari.tsx:62` | JsxText | ✕ Reddet ve Gerekçelendir | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0128 | `components/ders/OneriSablonlari.tsx:69` | JsxText | YZ Önerisi Öğretmen Tarafından Reddedildi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0129 | `components/ders/OneriSablonlari.tsx:70` | StringLiteral | Gerekçe (Örn: Sınıf dinamiklerine bugün uygun değil) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0130 | `components/ders/OneriSablonlari.tsx:71` | JsxText | Kaydet | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0131 | `components/eba/EbaPaneli.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0132 | `components/eba/EbaPaneli.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0133 | `components/eba/EbaPaneli.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0134 | `components/eba/EbaPaneli.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0135 | `components/eba/EbaPaneli.tsx:28` | StringLiteral | gözlem-girişi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0136 | `components/eba/EbaPaneli.tsx:29` | TemplateMiddle | (maske-UID ÖĞR-•••) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0137 | `components/eba/EbaPaneli.tsx:29` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0138 | `components/eba/EbaPaneli.tsx:29` | TemplateMiddle | davranış-gözlemi; ör. " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0139 | `components/eba/EbaPaneli.tsx:29` | LastTemplateToken | " (gözlemlenebilir-sayılabilir dil). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0140 | `components/eba/EbaPaneli.tsx:33` | StringLiteral | • Bugün H-c kaydı yok — örnek-desen (sentetik): "ARD-05, Hece Avcısı görevi sırasında 2 kez görevi kendisi başlattı; 1 kez ipucu istedi ve sürdürdü." | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0141 | `components/eba/EbaPaneli.tsx:35` | StringLiteral | GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0142 | `components/eba/EbaPaneli.tsx:36` | TemplateHead | Tarih: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0143 | `components/eba/EbaPaneli.tsx:36` | LastTemplateToken | · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0144 | `components/eba/EbaPaneli.tsx:38` | StringLiteral | [Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA'ya yazma-yok] | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0145 | `components/eba/EbaPaneli.tsx:45` | JsxText | 1 · Cihaz (Terminal) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0146 | `components/eba/EbaPaneli.tsx:45` | JsxText | EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0147 | `components/eba/EbaPaneli.tsx:48` | JsxText | 2 · daily-insight TASLAĞI | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0148 | `components/eba/EbaPaneli.tsx:48` | JsxText | Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0149 | `components/eba/EbaPaneli.tsx:51` | JsxText | 3 · [EBA POST] /api/v1/report/daily-insight | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0150 | `components/eba/EbaPaneli.tsx:52` | JsxText | PLANLI ENTEGRASYON — bu önizlemede gönderim YOK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0151 | `components/eba/EbaPaneli.tsx:57` | JsxText | K-331: salt-okunur çağrı — ödev/içerik yazılmaz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0152 | `components/eba/EbaPaneli.tsx:58` | JsxText | e-sınav girişi YOK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0153 | `components/eba/EbaPaneli.tsx:59` | JsxText | K-334: idari-mali otomasyon dışarı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0154 | `components/eba/EbaPaneli.tsx:60` | JsxText | Başarı Notu Yazılmaz · Maskeli UID | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0155 | `components/eba/EbaPaneli.tsx:65` | JsxText | Insight Taslağı Üret (yerel) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0156 | `components/eba/EbaPaneli.tsx:72` | JsxText | OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; ↵         bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0157 | `components/izleme/FrictionMap.tsx:18` | StringLiteral | Ali Y. | Bağlı değil: kaynak rezervi |
| SCH-LEX-0158 | `components/izleme/FrictionMap.tsx:19` | StringLiteral | Ayşe T. | Bağlı değil: kaynak rezervi |
| SCH-LEX-0159 | `components/izleme/FrictionMap.tsx:20` | StringLiteral | Can B. | Bağlı değil: kaynak rezervi |
| SCH-LEX-0160 | `components/izleme/FrictionMap.tsx:36` | JsxText | Öğrenme Sürtünme Haritası (Friction Map) | Bağlı değil: kaynak rezervi |
| SCH-LEX-0161 | `components/izleme/FrictionMap.tsx:37` | JsxText | Öğrencilerin görev aşamalarındaki bilişsel dirençlerini ve kopma noktalarını gösterir. | Bağlı değil: kaynak rezervi |
| SCH-LEX-0162 | `components/izleme/FrictionMap.tsx:44` | JsxText | Öğrenci | Bağlı değil: kaynak rezervi |
| SCH-LEX-0163 | `components/izleme/FrictionMap.tsx:45` | JsxText | Görev | Bağlı değil: kaynak rezervi |
| SCH-LEX-0164 | `components/izleme/FrictionMap.tsx:46` | JsxText | Başlama Direnci | Bağlı değil: kaynak rezervi |
| SCH-LEX-0165 | `components/izleme/FrictionMap.tsx:47` | JsxText | Görev Sürdürme | Bağlı değil: kaynak rezervi |
| SCH-LEX-0166 | `components/izleme/FrictionMap.tsx:48` | JsxText | Geçiş / Sonlandırma | Bağlı değil: kaynak rezervi |
| SCH-LEX-0167 | `components/izleme/FrictionMap.tsx:78` | JsxText | Eğitsel Çıkarım Örneği: | Bağlı değil: kaynak rezervi |
| SCH-LEX-0168 | `components/izleme/FrictionMap.tsx:78` | JsxText | Ali'nin MAT-02 görevine başlaması çok zor (Yüksek Direnç) ancak başladıktan sonra akıcı bir şekilde bitiriyor (Düşük Sürdürme Direnci). Ali'ye göreve başlarken kısa bir görsel tetikleyici vermek sürtünmeyi (friction) kırabilir. | Bağlı değil: kaynak rezervi |
| SCH-LEX-0169 | `components/izleme/IzlemePaneli.tsx:16` | JsxText | MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0170 | `components/izleme/IzlemePaneli.tsx:16` | JsxText | seriler sentetik-gösterimdir (K-05); XR/Görev-panosu Faz-3 PLANLI-katmandır — bu ekranda koşmaz. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0171 | `components/izleme/IzlemePaneli.tsx:20` | JsxText | Öğrenci (maskeli): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0172 | `components/izleme/IzlemePaneli.tsx:28` | JsxText | Yanıt zamanı eğimi — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0173 | `components/izleme/IzlemePaneli.tsx:28` | JsxText | (12 gözlem-noktası) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0174 | `components/izleme/IzlemePaneli.tsx:35` | JsxText | Görev etkileşim oranı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0175 | `components/izleme/IzlemePaneli.tsx:35` | JsxText | (sentetik-sabit · Faz-3 Görev-M11) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0176 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | Aktif görev: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0177 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | Katılım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0178 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | Y-Eğim: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0179 | `components/izleme/IzlemePaneli.tsx:40` | JsxText | K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0180 | `components/ogretmen/Cockpit.tsx:17` | StringLiteral | SNF | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0181 | `components/ogretmen/Cockpit.tsx:22` | JsxText | MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0182 | `components/ogretmen/Cockpit.tsx:22` | JsxText | tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için ↵         yönlendirme-desteğidir (K-02) · eşik-önerisi: Y-Eğim ≥ 0.07 → Nefes Molası. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0183 | `components/ogretmen/Cockpit.tsx:27` | JsxText | Toplu Yorgunluk Eğimi — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0184 | `components/ogretmen/Cockpit.tsx:35` | JsxText | Y-Eğim | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0185 | `components/ogretmen/Cockpit.tsx:36` | JsxText | Katılım | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0186 | `components/ogretmen/Cockpit.tsx:37` | JsxText | yorgunluk-uyarısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0187 | `components/ogretmen/Cockpit.tsx:42` | JsxText | Yanıt zamanı eğimi sınıf-eğrisi (sentetik-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0188 | `components/ogretmen/Cockpit.tsx:50` | JsxText | Nefes Molası (4-4-4) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0189 | `components/ogretmen/Cockpit.tsx:57` | JsxText | Kılavuz-tempo: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0190 | `components/ogretmen/Cockpit.tsx:57` | JsxText | 4 sn al — 4 sn tut — 4 sn ver | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0191 | `components/ogretmen/Cockpit.tsx:57` | JsxText | · sınıf-öncesi/arası 2 tur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0192 | `components/ogretmen/Cockpit.tsx:59` | JsxText | öğrenci eşik-üstü → yönlendirme-önerisi hazır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0193 | `components/ogretmen/Cockpit.tsx:60` | StringLiteral | Eşik-üstü öğrenci yok. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0194 | `components/ogretmen/Cockpit.tsx:65` | JsxText | Yönlendirme-kartı üret | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0195 | `components/ogretmen/Cockpit.tsx:69` | JsxText | — gözlem-notu (MOCK): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0196 | `components/ogretmen/Cockpit.tsx:69` | StringLiteral | sınıf-geneli | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0197 | `components/ogretmen/Cockpit.tsx:69` | JsxText | için ↵             Nefes Molası tempo (4-4-4) denenebilir. Bu kart cihaza komut GÖNDERMEZ; öğretmen-sözüyle yürütülür. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0198 | `components/ogretmen/TransferGozlemKarti.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0199 | `components/ogretmen/TransferGozlemKarti.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0200 | `components/ogretmen/TransferGozlemKarti.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0201 | `components/ogretmen/TransferGozlemKarti.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0202 | `components/ogretmen/TransferGozlemKarti.tsx:79` | JsxText | Transfer Gözlem Kartı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0203 | `components/ogretmen/TransferGozlemKarti.tsx:80` | JsxText | Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0204 | `components/ogretmen/TransferGozlemKarti.tsx:82` | JsxText | Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. ↵             Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0205 | `components/ogretmen/TransferGozlemKarti.tsx:89` | JsxText | MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0206 | `components/ogretmen/TransferGozlemKarti.tsx:94` | JsxText | Öğrenci (sentetik): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0207 | `components/ogretmen/TransferGozlemKarti.tsx:101` | JsxText | Gözlenen etkinlik: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0208 | `components/ogretmen/TransferGozlemKarti.tsx:110` | JsxText | Gözlenen davranışlar (işaretleyerek): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0209 | `components/ogretmen/TransferGozlemKarti.tsx:125` | JsxText | Kısa not (isteğe bağlı): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0210 | `components/ogretmen/TransferGozlemKarti.tsx:127` | StringLiteral | Örn. tahta örneğinden sonra kendi uygulamasına geçti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0211 | `components/ogretmen/TransferGozlemKarti.tsx:134` | JsxText | Kaydet (yerel) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0212 | `components/ogretmen/TransferGozlemKarti.tsx:137` | JsxText | kayıt · yalnız bu tarayıcıda | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0213 | `components/ogretmen/TransferGozlemKarti.tsx:144` | JsxText | Son kayıtlar: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0214 | `components/ogretmen/TransferGozlemKarti.tsx:147` | JsxText | hepsini temizle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0215 | `components/ogretmen/TransferGozlemKarti.tsx:153` | JsxText | davranış | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0216 | `components/portfoy/Portfoy.tsx:12` | StringLiteral | Gözlem-kartı (H-c) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0217 | `components/portfoy/Portfoy.tsx:13` | StringLiteral | Görev-ataması | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0218 | `components/portfoy/Portfoy.tsx:14` | StringLiteral | BEP-hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0219 | `components/portfoy/Portfoy.tsx:15` | StringLiteral | Sonuç-notu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0220 | `components/portfoy/Portfoy.tsx:32` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0221 | `components/portfoy/Portfoy.tsx:32` | TemplateMiddle | davranış-gözlemi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0222 | `components/portfoy/Portfoy.tsx:35` | TemplateHead | etkinlik atandı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0223 | `components/portfoy/Portfoy.tsx:35` | TemplateMiddle | · kazanım | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0224 | `components/portfoy/Portfoy.tsx:38` | TemplateHead | BEP-hazırlık hedefi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0225 | `components/portfoy/Portfoy.tsx:38` | LastTemplateToken | haftalık-probu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0226 | `components/portfoy/Portfoy.tsx:41` | TemplateHead | sonuç-notu: " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0227 | `components/portfoy/Portfoy.tsx:54` | JsxText | Öğrenci Defteri — yazılı-portfolyo | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0228 | `components/portfoy/Portfoy.tsx:56` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0229 | `components/portfoy/Portfoy.tsx:61` | JsxText | Defterleri tara | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0230 | `components/portfoy/Portfoy.tsx:62` | JsxText | kayıt · 4-defter salt-okunur | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0231 | `components/portfoy/Portfoy.tsx:65` | JsxText | Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0232 | `components/portfoy/Portfoy.tsx:78` | JsxText | Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla ↵         bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0233 | `components/rapor/RaporOzeti.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0234 | `components/rapor/RaporOzeti.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0235 | `components/rapor/RaporOzeti.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0236 | `components/rapor/RaporOzeti.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0237 | `components/rapor/RaporOzeti.tsx:28` | StringLiteral | gözlem | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0238 | `components/rapor/RaporOzeti.tsx:29` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0239 | `components/rapor/RaporOzeti.tsx:29` | StringLiteral | gözlem-girişi yok | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0240 | `components/rapor/RaporOzeti.tsx:29` | TemplateHead | ; öğretmen-notu: " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0241 | `components/rapor/RaporOzeti.tsx:34` | JsxText | Görev-H deseni: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0242 | `components/rapor/RaporOzeti.tsx:34` | JsxText | "40 dk derste 3 kez yerinden kalktı" tipi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0243 | `components/rapor/RaporOzeti.tsx:34` | JsxText | gözlemlenebilir-sayılabilir dil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0244 | `components/rapor/RaporOzeti.tsx:34` | JsxText | . ↵         Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0245 | `components/rapor/RaporOzeti.tsx:38` | JsxText | Günün Ev–Okul Notu Taslağı (H-c kaynaklı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0246 | `components/rapor/RaporOzeti.tsx:41` | JsxText | Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0247 | `components/rapor/RaporOzeti.tsx:48` | JsxText | Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0248 | `components/ses/SesPaneli.tsx:16` | JsxText | PLANLI-KATMAN şerhi: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0249 | `components/ses/SesPaneli.tsx:16` | JsxText | donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü ↵         ayrımının | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0250 | `components/ses/SesPaneli.tsx:17` | JsxText | görsel-simülasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0251 | `components/ses/SesPaneli.tsx:17` | JsxText | vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0252 | `components/ses/SesPaneli.tsx:21` | JsxText | Ana Sinyal İzolasyonu — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0253 | `components/ses/SesPaneli.tsx:29` | JsxText | ana-sinyal | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0254 | `components/ses/SesPaneli.tsx:30` | JsxText | ortam-gürültüsü (izolasyon-arttıkça söner) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0255 | `components/ses/SesPaneli.tsx:35` | JsxText | Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0256 | `components/shell/Kabuk.tsx:6` | StringLiteral | Sınıf Özeti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0257 | `components/shell/Kabuk.tsx:7` | StringLiteral | Sınıf | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0258 | `components/shell/Kabuk.tsx:8` | StringLiteral | Öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0259 | `components/shell/Kabuk.tsx:9` | StringLiteral | Öğretmen | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0260 | `components/shell/Kabuk.tsx:10` | StringLiteral | Transfer Gözlem Kartı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0261 | `components/shell/Kabuk.tsx:11` | StringLiteral | Ders & Görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0262 | `components/shell/Kabuk.tsx:12` | StringLiteral | Aile Bilgilendirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0263 | `components/shell/Kabuk.tsx:13` | StringLiteral | BEP Hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0264 | `components/shell/Kabuk.tsx:14` | StringLiteral | MEB EBA Entegrasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0265 | `components/shell/Kabuk.tsx:15` | StringLiteral | Gelişim Takibi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0266 | `components/shell/Kabuk.tsx:16` | StringLiteral | Sınıf İçi Ses Yönetimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0267 | `components/shell/Kabuk.tsx:19` | StringLiteral | Sistem Kılavuzu ve Terimler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0268 | `components/shell/Kabuk.tsx:32` | JsxText | LEXIVA Scholaria™ | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0269 | `components/shell/Kabuk.tsx:33` | JsxText | School Node · v | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0270 | `components/shell/Kabuk.tsx:50` | JsxText | Rol: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0271 | `components/shell/Kabuk.tsx:50` | JsxText | · B2B Sınıf Düğümü (School Node) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0272 | `components/shell/Kabuk.tsx:55` | JsxText | LEXIVA Scholaria: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0273 | `components/shell/Kabuk.tsx:55` | JsxText | Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0274 | `components/takip/GelisimTakibi.tsx:24` | JsxText | Gelişim-takibi (gözlem-çizelgesi) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0275 | `components/takip/GelisimTakibi.tsx:26` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0276 | `components/takip/GelisimTakibi.tsx:33` | JsxText | Katılım/Y-Eğim serisi (MOCK-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0277 | `components/takip/GelisimTakibi.tsx:37` | JsxText | Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0278 | `components/takip/GelisimTakibi.tsx:40` | JsxText | H-c gözlem-zaman-çizelgesi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0279 | `components/takip/GelisimTakibi.tsx:40` | JsxText | kayıt) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0280 | `components/takip/GelisimTakibi.tsx:42` | JsxText | Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0281 | `components/takip/GelisimTakibi.tsx:47` | JsxText | davranış-gözlemi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0282 | `components/veli/VeliKoprusu.tsx:12` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0283 | `components/veli/VeliKoprusu.tsx:12` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0284 | `components/veli/VeliKoprusu.tsx:15` | StringLiteral | Eve dönüşte gün-içi bir gözlemi tek-cümleyle paylaşın ("bugün görevine kendi başladı"). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0285 | `components/veli/VeliKoprusu.tsx:16` | StringLiteral | Ödevi tek-seferde değil, 10 dakikalık iki-bölüm olarak planlayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0286 | `components/veli/VeliKoprusu.tsx:17` | StringLiteral | Ekran-öncesi kısa nefes-rutini (4-4-4) birlikte deneyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0287 | `components/veli/VeliKoprusu.tsx:18` | StringLiteral | Talimatları tek-tek ve sırayla verin; tamamlanınca sözel takdir edin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0288 | `components/veli/VeliKoprusu.tsx:19` | StringLiteral | Uyku ve oyun-düzeni gözlem-notlarını hafta-sonu karşılaştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0289 | `components/veli/VeliKoprusu.tsx:30` | StringLiteral | Haftalık gözlem paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0290 | `components/veli/VeliKoprusu.tsx:39` | TemplateHead | HAFTALIK SINIF BÜLTENİ — TASLAK (yerel-üretim; gönderilmez) ↵ Sınıf: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0291 | `components/veli/VeliKoprusu.tsx:39` | TemplateMiddle | · Tarih: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0292 | `components/veli/VeliKoprusu.tsx:40` | TemplateHead | Sınıf-gözlemi (MOCK): öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0293 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · ort. Y-Eğim | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0294 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · son-alarm: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0295 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · bu-hafta | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0296 | `components/veli/VeliKoprusu.tsx:40` | LastTemplateToken | gözlem-kartı (H-c). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0297 | `components/veli/VeliKoprusu.tsx:41` | FirstTemplateToken | Bu haftanın genel-önerileri (sınıf-geneli; kişi-değerlendirmesi yok — K-02): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0298 | `components/veli/VeliKoprusu.tsx:43` | FirstTemplateToken | Aile-EĞİTİMİ programı ve kişiye-özel içerik SUPPORTA ürünündedir; bu bülten yalnız bilgilendirme-notudur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0299 | `components/veli/VeliKoprusu.tsx:48` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0300 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0301 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0302 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0303 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0304 | `components/veli/VeliKoprusu.tsx:58` | JsxText | Haftalık Aile Bülteni — TASLAK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0305 | `components/veli/VeliKoprusu.tsx:63` | JsxText | Bülten taslağı üret | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0306 | `components/veli/VeliKoprusu.tsx:66` | JsxText | Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0307 | `components/veli/VeliKoprusu.tsx:70` | JsxText | Veli Görüşme — Randevu Defteri | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0308 | `components/veli/VeliKoprusu.tsx:75` | JsxText | Haftalık gözlem paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0309 | `components/veli/VeliKoprusu.tsx:76` | JsxText | H-c kart-turu değerlendirme paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0310 | `components/veli/VeliKoprusu.tsx:77` | JsxText | Gelişim-görüşmesi (gözlem-özetli) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0311 | `components/veli/VeliKoprusu.tsx:78` | JsxText | Diğer | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0312 | `components/veli/VeliKoprusu.tsx:80` | StringLiteral | görüşme-notu (isteğe bağlı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0313 | `components/veli/VeliKoprusu.tsx:82` | JsxText | Randevu kaydet | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0314 | `components/veli/VeliKoprusu.tsx:85` | JsxText | Defter boş — randevu kaydedin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0315 | `components/veli/VeliKoprusu.tsx:98` | JsxText | Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0316 | `data/mock.ts:5` | StringLiteral | 2. Sınıf A Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0317 | `data/mock.ts:6` | StringLiteral | 2. Sınıf B Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0318 | `data/mock.ts:7` | StringLiteral | 4. Sınıf A Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0319 | `data/mock.ts:11` | StringLiteral | Matematik: Sayı Blokları Eşleştirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0320 | `data/mock.ts:12` | StringLiteral | Hareket: Ritim ve Süre Tahmini | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0321 | `data/mock.ts:13` | StringLiteral | Türkçe: Hece Avcısı (Okuma) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0322 | `data/mock.ts:25` | StringLiteral | Yorgunluk Uyarısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0323 | `data/mufredatYonerge.ts:9` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0324 | `data/mufredatYonerge.ts:13` | StringLiteral | Sayı postası: oku-yaz-eşle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0325 | `data/mufredatYonerge.ts:13` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0326 | `data/mufredatYonerge.ts:13` | StringLiteral | Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0327 | `data/mufredatYonerge.ts:14` | StringLiteral | Onluk-birlik çantası | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0328 | `data/mufredatYonerge.ts:14` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0329 | `data/mufredatYonerge.ts:14` | StringLiteral | Nesneleri 10'luk torbalara koydurarak onluk-birlik ayrımını somutlaştırın; tahtadaki tabloya birlikte işleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0330 | `data/mufredatYonerge.ts:15` | StringLiteral | Sayı doğrusu düellosu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0331 | `data/mufredatYonerge.ts:15` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0332 | `data/mufredatYonerge.ts:15` | StringLiteral | Yer-matında sayı doğrusu çizip komşu-sayılar arasında yürüyerek yer-değiştirme oyunu oynatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0333 | `data/mufredatYonerge.ts:16` | StringLiteral | Yüzlük tablo zıplaş | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0334 | `data/mufredatYonerge.ts:16` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0335 | `data/mufredatYonerge.ts:16` | StringLiteral | Yüzlük tabloda 1'er ve 10'ar atlamaları renkli-kalemle boyattırın; kuralı öğrenciye sözlü teyit ettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0336 | `data/mufredatYonerge.ts:17` | StringLiteral | Örüntü treni: kural-kur-devam-et | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0337 | `data/mufredatYonerge.ts:17` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0338 | `data/mufredatYonerge.ts:17` | StringLiteral | Şekil/sayı-kartlarıyla 2'şer-5'er-10'ar örüntüler kurdurtun; kuralı sözlutturup sıradaki-halkayı tahmin ettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0339 | `data/mufredatYonerge.ts:18` | StringLiteral | Tahmin kavanozu: grupla-tahmin et | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0340 | `data/mufredatYonerge.ts:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0341 | `data/mufredatYonerge.ts:18` | StringLiteral | Kavanozdaki nesneleri önce 10'luk gruplatıp tahmin yazdırın; sonra saydırarak tahmini doğrulatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0342 | `data/mufredatYonerge.ts:19` | StringLiteral | Bütün-yarım-çeyrek pizza | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0343 | `data/mufredatYonerge.ts:19` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0344 | `data/mufredatYonerge.ts:19` | StringLiteral | Kâğıt-daireleri katlatıp keserek yarım/çeyrek/bütün ilişkisini yapıştırma-panosunda kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0345 | `data/mufredatYonerge.ts:20` | StringLiteral | Kasaba para turu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0346 | `data/mufredatYonerge.ts:20` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0347 | `data/mufredatYonerge.ts:20` | StringLiteral | Sınıf-mağazası dramatizasyonu kurun; TL-banknot kopyalarıyla alışveriş yaptırıp harcama-çizelgesi doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0348 | `data/mufredatYonerge.ts:21` | StringLiteral | Tam saat, yarım saat: saat-avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0349 | `data/mufredatYonerge.ts:21` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0350 | `data/mufredatYonerge.ts:21` | StringLiteral | Kart-saatlerle tam/yarım-saat ayırımı yaptırın; gün-içi rutini saat-bilgisiyle eşleştirme-turu kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0351 | `data/mufredatYonerge.ts:22` | StringLiteral | Karış mı, cetvel mi? | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0352 | `data/mufredatYonerge.ts:22` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0353 | `data/mufredatYonerge.ts:22` | StringLiteral | Aynı uzunluğu karış, adım ve cetvel ile ölçtürüp sonuçları karşılaştırın; standart-ölçü gereğini tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0354 | `data/mufredatYonerge.ts:23` | StringLiteral | Tahmin çubuğu: ölç-karşılaştır | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0355 | `data/mufredatYonerge.ts:23` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0356 | `data/mufredatYonerge.ts:23` | StringLiteral | Uzunlukları önce tahmin ettirip yazdırın; sonra cetveliyle ölçtürüp tahmin-ölçü tablosunu doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0357 | `data/mufredatYonerge.ts:24` | StringLiteral | Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0358 | `data/mufredatYonerge.ts:24` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0359 | `data/mufredatYonerge.ts:24` | StringLiteral | Sınıf-içi senaryolardan toplama-çıkarma problemleri kurdurtun; çözümü tek-cümleyle anlattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0360 | `data/mufredatYonerge.ts:25` | StringLiteral | Tahmin et, zihinden işle, tutarlılığı açıkla | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0361 | `data/mufredatYonerge.ts:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0362 | `data/mufredatYonerge.ts:25` | StringLiteral | İşlemi önce zihinden-tahmin ettirin; sonra yazıyla doğrulatıp tahminle-sonucu karşılaştırıp açıklattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0363 | `data/mufredatYonerge.ts:26` | StringLiteral | Toplama-çıkarma ters-ilişkisi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0364 | `data/mufredatYonerge.ts:26` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0365 | `data/mufredatYonerge.ts:26` | StringLiteral | Toplamadan çıkarma ürettirtin (a+b=c → c−b=a); boşluklu-kartlarla eşleştirme-oyunuyla pekiştirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0366 | `data/mufredatYonerge.ts:27` | StringLiteral | Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0367 | `data/mufredatYonerge.ts:27` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0368 | `data/mufredatYonerge.ts:27` | StringLiteral | Eş-öbek dizilimleri kurdurtun; toplamanın-kısa-yolu olarak çarpma yazdırın (2+2+2 = 3×2). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0369 | `data/mufredatYonerge.ts:28` | StringLiteral | Çarpan ve çarpım: bileşenler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0370 | `data/mufredatYonerge.ts:28` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0371 | `data/mufredatYonerge.ts:28` | StringLiteral | 3×4 gibi işlemlerde parça-adlarını öğretin (çarpan-çarpan-çarpım); geriden-seçme oyunu oynatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0372 | `data/mufredatYonerge.ts:29` | StringLiteral | Eşitliğin anlamları: denge | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0373 | `data/mufredatYonerge.ts:29` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0374 | `data/mufredatYonerge.ts:29` | StringLiteral | Terazi-deseninde boşluğa sayı yazdırarak eşitliği kurdurtun (5+3=□+2); dengeyi cümleyle açıklatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0375 | `data/mufredatYonerge.ts:30` | StringLiteral | Geometri ayırma bandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0376 | `data/mufredatYonerge.ts:30` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0377 | `data/mufredatYonerge.ts:30` | StringLiteral | Şekil-kartlarını kenar ve köşe-özelliklerine göre sınıflandırma-bandına yerleştirtin; ayrımı sözlü gerekçelendirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0378 | `data/mufredatYonerge.ts:31` | StringLiteral | Küp kule inşaatı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0379 | `data/mufredatYonerge.ts:31` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0380 | `data/mufredatYonerge.ts:31` | StringLiteral | Küp-kule inşa ettirin; küp-sayısını önce-tahmin sonra-saydırarak karşılaştırma-satırı yazdırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0381 | `data/mufredatYonerge.ts:32` | StringLiteral | Şekil mozaik atölyesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0382 | `data/mufredatYonerge.ts:32` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0383 | `data/mufredatYonerge.ts:32` | StringLiteral | Kare/üçgen mozaiklerle yeni-şekiller oluşturtun; hangi-şekillerden oluştuğunu anlattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0384 | `data/mufredatYonerge.ts:33` | StringLiteral | Döndür-karşılaştır: aynı mı, farklı mı? | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0385 | `data/mufredatYonerge.ts:33` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0386 | `data/mufredatYonerge.ts:33` | StringLiteral | Kesik-şekilleri döndürüp aynı/farklı ayırımı yaptırın; döndürünce adın-değişmediğini tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0387 | `data/mufredatYonerge.ts:34` | StringLiteral | Bardak sorusu: tahmin-ölç | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0388 | `data/mufredatYonerge.ts:34` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0389 | `data/mufredatYonerge.ts:34` | StringLiteral | Aynı sıvıyı ince/geniş bardaklara döktürüp miktarın-değişmediğini gözlemletin (korunum-yargısı kurdurmadan). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0390 | `data/mufredatYonerge.ts:35` | StringLiteral | Hedefe yol: planla-izle-analiz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0391 | `data/mufredatYonerge.ts:35` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0392 | `data/mufredatYonerge.ts:35` | StringLiteral | Sınıf-planında A→B arası yolları çizdirtin; en-kısayı seçtirtin ve adım-adım plan-izle-analiz turu yapın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0393 | `data/mufredatYonerge.ts:36` | StringLiteral | Ayna avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0394 | `data/mufredatYonerge.ts:36` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0395 | `data/mufredatYonerge.ts:36` | StringLiteral | Harf ve şekil-kartlarını aynaya tutturtup simetrikleri avlattırın; simetri-çizgisini kendilerine bozdurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0396 | `data/mufredatYonerge.ts:37` | StringLiteral | İki grup, bir grafik | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0397 | `data/mufredatYonerge.ts:37` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0398 | `data/mufredatYonerge.ts:37` | StringLiteral | Basit sınıf-anketi yapılıp sonuçları resimli-grafiğe işlettirin; "kaç-fazla/kaç-az" soruları sordurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0399 | `data/mufredatYonerge.ts:39` | StringLiteral | Dinleme/izlemeyi yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0400 | `data/mufredatYonerge.ts:39` | StringLiteral | Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0401 | `data/mufredatYonerge.ts:40` | StringLiteral | Dinlediklerinden anlam kurma: ana-fikir avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0402 | `data/mufredatYonerge.ts:40` | StringLiteral | Kısa-hikâye dinlettirin; ana-fikri tek-cümleyle tahmin ettirip sınıfça tartışın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0403 | `data/mufredatYonerge.ts:41` | StringLiteral | Dinlediklerini/izlediklerini çözümleyebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0404 | `data/mufredatYonerge.ts:41` | StringLiteral | Sebep-sonuç içeren masal dinlettirin; "neden-bekledi?" sorularıyla çözümleme-tartışması kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0405 | `data/mufredatYonerge.ts:42` | StringLiteral | Dinleme/izleme sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0406 | `data/mufredatYonerge.ts:42` | StringLiteral | Dinleme-sonu "ne-anladım" paylaşım-çemberi yaptırın; kendi-dinlemesine bakan cümle kurdurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0407 | `data/mufredatYonerge.ts:43` | StringLiteral | Dinleme/izlemeyi yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0408 | `data/mufredatYonerge.ts:43` | StringLiteral | Haber/duyuru dinlettin; kim-ne-zaman ipuçlarını dinlerken resimli-not aldırtın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0409 | `data/mufredatYonerge.ts:44` | StringLiteral | Dinledikleri/izledikleri ile ilgili anlam oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0410 | `data/mufredatYonerge.ts:44` | StringLiteral | Kurallar-metni dinlettirip dinlediklerinden tek-cümlelik anlam-özeti ürettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0411 | `data/mufredatYonerge.ts:45` | StringLiteral | Dinlediklerini/izlediklerini çözümleyebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0412 | `data/mufredatYonerge.ts:45` | StringLiteral | Sıralı-olay anlatımı dinlettin; önce/sonra kartlarını doğru-sıraya dizdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0413 | `data/mufredatYonerge.ts:46` | StringLiteral | Dinleme/izleme sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0414 | `data/mufredatYonerge.ts:46` | StringLiteral | Gürültülü ve sessiz ortamda kısa-dinleme karşılaştırması yaptırın; farkı birlikte tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0415 | `data/mufredatYonerge.ts:47` | StringLiteral | Dinleme/izleme sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0416 | `data/mufredatYonerge.ts:47` | StringLiteral | Dinlediği-hikâyeyi özetlettirin; güçlü-dinleme belirtilerini birlikte listelettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0417 | `data/mufredatYonerge.ts:48` | StringLiteral | Konuşmalarını yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0418 | `data/mufredatYonerge.ts:48` | StringLiteral | Toplantı-çemberinde söz-sırası kuralıyla kısa-konuşmalar yaptırın; el-kaldırma rutinini pekiştirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0419 | `data/mufredatYonerge.ts:49` | StringLiteral | Konuşmalarında içerik oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0420 | `data/mufredatYonerge.ts:49` | StringLiteral | Kim/zaman/yer/olay ipuçlarını içeren olay-anlatımı görevi verin; ipuçlarını kullanma-adımını gözlemleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0421 | `data/mufredatYonerge.ts:50` | StringLiteral | Konuşma kurallarını uygulayabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0422 | `data/mufredatYonerge.ts:50` | StringLiteral | Göz-teması ve ses-şiddeti hedefleriyle rol-oyunu konuşmaları kurdurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0423 | `data/mufredatYonerge.ts:51` | StringLiteral | Konuşma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0424 | `data/mufredatYonerge.ts:51` | StringLiteral | Konuşma-sonu "anlatabildim-mi" öz-tartışma çemberi yaptırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0425 | `data/mufredatYonerge.ts:52` | StringLiteral | Konuşmalarını yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0426 | `data/mufredatYonerge.ts:52` | StringLiteral | Sınıf-tartışmasında sıra-alma kartları kullanın; dinle-söyle rutini kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0427 | `data/mufredatYonerge.ts:53` | StringLiteral | Konuşmalarında içerik oluşturabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0428 | `data/mufredatYonerge.ts:53` | StringLiteral | Gezi/gün-anlatısında önce-sonra-en-son bağlaçlarını kullanma-hedefi verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0429 | `data/mufredatYonerge.ts:54` | StringLiteral | Konuşma kurallarını uygulayabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0430 | `data/mufredatYonerge.ts:54` | StringLiteral | Telefon-dramatizasyonu kurdurtun; selam-amaç-kapanış üçlüsünü denettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0431 | `data/mufredatYonerge.ts:55` | StringLiteral | Konuşma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0432 | `data/mufredatYonerge.ts:55` | StringLiteral | Ortam-seçiminin anlaşılırlığa etkisini oyunla gözlemletip tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0433 | `data/mufredatYonerge.ts:56` | StringLiteral | Konuşma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0434 | `data/mufredatYonerge.ts:56` | StringLiteral | Konuşma-sonu iki-güçlü-yön bir-gelişim-alanı paylaşımı yaptırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0435 | `data/mufredatYonerge.ts:57` | StringLiteral | Okuma sürecini yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0436 | `data/mufredatYonerge.ts:57` | StringLiteral | Sessiz-okuma rutini kurun; satır-takip kartıyla odaklanma davranışını gözlem-notuyla izleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0437 | `data/mufredatYonerge.ts:58` | StringLiteral | Okuduklarından anlam kurma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0438 | `data/mufredatYonerge.ts:58` | StringLiteral | Kısa-metin okutturup yanıtı metinde-bulunur sorular sorun; işaretlettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0439 | `data/mufredatYonerge.ts:59` | StringLiteral | Okuduklarını çözümleyebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0440 | `data/mufredatYonerge.ts:59` | StringLiteral | Karakter/yer-bilgisi isteyen çözümleme-sorularıyla metin-tartışması kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0441 | `data/mufredatYonerge.ts:60` | StringLiteral | Okuma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0442 | `data/mufredatYonerge.ts:60` | StringLiteral | Okuma-ortamını birlikte düzenlettirin; gürültünün anlamaya-etkisini gözlemletin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0443 | `data/mufredatYonerge.ts:61` | StringLiteral | Okuma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0444 | `data/mufredatYonerge.ts:61` | StringLiteral | Okuduğunu-yeniden-anlatma çifti kurun; kendi-anlamasını kontrol-cümlesiyle bağdattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0445 | `data/mufredatYonerge.ts:62` | StringLiteral | Okuma sürecini yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0446 | `data/mufredatYonerge.ts:62` | StringLiteral | Satır-takip kartı kullanımını modelleyip her-okurda uygulattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0447 | `data/mufredatYonerge.ts:63` | StringLiteral | Okudukları ile ilgili anlam oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0448 | `data/mufredatYonerge.ts:63` | StringLiteral | Yanıtı metinde-olan sorular sorun; buldukları-satırı gösterdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0449 | `data/mufredatYonerge.ts:64` | StringLiteral | Okuduklarını çözümleyebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0450 | `data/mufredatYonerge.ts:64` | StringLiteral | İleti-bulma sorusuyla kısa-hikâye tartışması yaptırın ("bu-hikâye ne-öğretti?"). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0451 | `data/mufredatYonerge.ts:65` | StringLiteral | Okuma sürecine etki eden durumları gözden geçirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0452 | `data/mufredatYonerge.ts:65` | StringLiteral | Bilinmeyen-kelime sözlük-köşesi kurun; bakma-adımını modelleyip uygulattın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0453 | `data/mufredatYonerge.ts:66` | StringLiteral | Okuma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0454 | `data/mufredatYonerge.ts:66` | StringLiteral | Hikâye-özetini kendi-kelimeleriyle anlattırın; anlamasını gözden-geçirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0455 | `data/mufredatYonerge.ts:67` | StringLiteral | Yazılı anlatım becerilerini yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0456 | `data/mufredatYonerge.ts:67` | StringLiteral | Oturuş ve kalem-tutuş kontrol-listesiyle yazma-hazırlığı yaptırın; listeyi öğrenciyle birlikte doldurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0457 | `data/mufredatYonerge.ts:68` | StringLiteral | Yazılarında içerik oluşturma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0458 | `data/mufredatYonerge.ts:68` | StringLiteral | Gün-içi olayı üç-cümleyle yazdirtin; önce-sonra kelimelerini kullanma-hedefi verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0459 | `data/mufredatYonerge.ts:69` | StringLiteral | Yazma kurallarını uygulayabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0460 | `data/mufredatYonerge.ts:69` | StringLiteral | Cümle-başı büyük-harf ve nokta-avcılığı yaptırın; yazısını kendine-tarattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0461 | `data/mufredatYonerge.ts:70` | StringLiteral | Yazma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0462 | `data/mufredatYonerge.ts:70` | StringLiteral | Yazıyı sesli-okuyarak-kontrol rutini kurup arkadaşa-okutma turu yapın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0463 | `data/mufredatYonerge.ts:71` | StringLiteral | Yazılı anlatım becerilerini yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0464 | `data/mufredatYonerge.ts:71` | StringLiteral | Yazma-öncesi üç-kelimelik mini-plan yaptırıp taslağa geçirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0465 | `data/mufredatYonerge.ts:72` | StringLiteral | Yazılarında içerik oluşturabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0466 | `data/mufredatYonerge.ts:72` | StringLiteral | Tarih-hitap-ileti-imza şablonuyla sınıf-içi mektup yazdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0467 | `data/mufredatYonerge.ts:73` | StringLiteral | Yazma kurallarını uygulayabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0468 | `data/mufredatYonerge.ts:73` | StringLiteral | Noktalama-kartlarıyla cümle-düzeltme yarışı kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0469 | `data/mufredatYonerge.ts:74` | StringLiteral | Yazma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0470 | `data/mufredatYonerge.ts:74` | StringLiteral | Kalem-tutuşu düzeltme egzersizlerini kısa-turlarla yaptırın; yorgunluk-belirtisini gözlemleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0471 | `data/mufredatYonerge.ts:75` | StringLiteral | Yazma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0472 | `data/mufredatYonerge.ts:75` | StringLiteral | Yazım-noktalama-anlam üçlü-kontrol listesini birlikte doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0473 | `data/mufredatYonerge.ts:78` | StringLiteral | 2. sınıf | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-LEX-0474 | `data/mufredatYonerge.ts:80` | StringLiteral | Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |

## C-LEX-3 — Tam TS/TSX kaynak bağlamı

Ürün kodu değiştirilmeden kopyalandı; bu bölüm UI listesi değildir. Teknik alanlar/yorumlar/bağlı olmayan bileşenler görünür metinden ayrı okunur. Satır sayımı aşağıdaki blokların ilk satırından başlar.

### `App.tsx`

14211 B · SHA-256 `ba846992a33191bb7ec5344779c73c62fe3cc30ce78c07fc4f6c7feca7f53611`

~~~~tsx
/**
 * SCHOLARIA App — K-554 CANLI-EKRAN-TURU (9/11 ekran artık etkileşimli; v0.2.2).
 * Canlı: Pano (tıklanır sınıf-nabız) · Sınıf (seçici↔veri + ritim eğrisi) · Öğrenci (görev-detay +
 * başlama-kilidi mini-simülasyon) · Öğretmen-Cockpit · EBA (salt-okunur akış + yerel insight-taslağı) ·
 * İzleme (öğrenci-eğrisi) · Ses (görsel-simülasyon) · Rapor (görev-H özeti) · Yardım (şerh-sözlüğü).
 * Statik-kalan: Ayarlar (K-334 idari-mali dışarı). Transfer Gözlem (H-c): v0.2.0'dan beri canlı (K-451).
 * Tüm veriler sentetik/mock (K-05); "ölçen değil, gözlemleyen" (K-02); sunucusuz (K-05).
 */
import { useEffect, useState } from 'react';
import Kabuk, { type EkranId } from './components/shell/Kabuk';
import { SINIF_DURUMU, GOREVLER, SUBELER } from './data/mock';
import { ritimSeri, noktalar } from './data/seriler';
import { KISITLAR } from './data/kisitlar';
import TransferGozlemKarti from './components/ogretmen/TransferGozlemKarti';
import Cockpit from './components/ogretmen/Cockpit';
import EbaPaneli from './components/eba/EbaPaneli';
import SesPaneli from './components/ses/SesPaneli';
import IzlemePaneli from './components/izleme/IzlemePaneli';
import RaporOzeti from './components/rapor/RaporOzeti';
import GorevAtama from './components/ders/GorevAtama';
import VeliKoprusu from './components/veli/VeliKoprusu';
import GelisimTakibi from './components/takip/GelisimTakibi';
import OneriSablonlari from './components/ders/OneriSablonlari';
import SonucNotu from './components/defter/SonucNotu';
import BepHedef from './components/bep/BepHedef';
import Portfoy from './components/portfoy/Portfoy';

export default function App() {
  const [ekran, setEkran] = useState<EkranId>('pano');
  const [secSinif, setSecSinif] = useState<string>('2A');
  const [secGorev, setSecGorev] = useState<string | null>(null);
  const [geriSay, setGeriSay] = useState<number | null>(null);

  useEffect(() => {
    if (geriSay === null) return;
    if (geriSay === 0) { setGeriSay(null); return; }
    const t = setTimeout(() => setGeriSay((g) => (g === null ? null : g - 1)), 1000);
    return () => clearTimeout(t);
  }, [geriSay]);

  return (
    <Kabuk ekran={ekran} setEkran={setEkran} rol="B2B Yönetici">
      <div data-testid="surum-modu" className="mb-3 flex flex-wrap gap-2 items-center justify-center rounded-xl border px-3 py-2 text-[11px] font-semibold bg-slate-50 border-slate-200 text-slate-700">
        <span>v{__SURUM__} · VAMOLA Scholaria - Öğretmen Sınıf Panosu</span>
      </div>

      {ekran === 'pano' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf Özeti (Shared Evidence Akışı)</h2>
          <p className="text-sm text-slate-600">Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır.</p>
          <div className="grid md:grid-cols-3 gap-3">
            {SINIF_DURUMU.map((s) => (
              <button key={s.sinifId} type="button" data-testid={`pano-sinif-${s.sinifId}`}
                onClick={() => { setSecSinif(s.sinifId); setEkran('sinif'); }}
                className="text-left border border-slate-200 p-4 rounded-xl space-y-1 bg-white hover:border-indigo-300 cursor-pointer">
                <div className="flex items-center justify-between">
                  <span className="font-bold">{s.sinifId} Sınıfı</span>
                  <span className={`text-[10px] px-1.5 py-0.5 rounded-full font-bold ${s.sonAlarm === 'Yok' ? 'bg-emerald-100 text-emerald-700' : 'bg-amber-100 text-amber-700'}`}>{s.sonAlarm}</span>
                </div>
                <div className="text-xs text-slate-500">Öğr. Sayı: {s.ogrenciler.length} · Ort. Y-Eğim: {s.ortalamaYorgunluk.toFixed(2)}</div>
                <div className="text-[10px] text-indigo-600">Gün-içi nabzı aç →</div>
              </button>
            ))}
          </div>
          <p className="text-[11px] text-slate-500">MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde.</p>
        </div>
      )}

      {ekran === 'sinif' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf (Sınıf Ritim Eğrisi)</h2>
          <p className="text-sm text-slate-600">Ders esnasında sınıf içi gürültü ve çeldirici dengesi. Seçili sınıfın göstergeleri:</p>
          <label className="inline-flex items-center gap-2 text-xs font-semibold text-slate-700">
            Hedef Sınıf:
            <select data-testid="sinif-secici" value={secSinif} onChange={(e) => setSecSinif(e.target.value)} className="rounded-lg border border-slate-200 bg-white px-2 py-1 text-xs">
              {SUBELER.map((s) => <option key={s.id} value={s.id.replace('SUB-', '')}>{s.id}</option>)}
            </select>
          </label>
          {(() => {
            const d = SINIF_DURUMU.find((x) => x.sinifId === secSinif);
            const seri = ritimSeri(secSinif);
            return (
              <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="sinif-paneli">
                <div className="p-3 bg-amber-50 border border-amber-200 rounded-xl text-xs text-amber-900">
                  <b>Aktif Parametre:</b> Sınıf Ritim Eğrisi (sentetik) — <b>{seri[seri.length - 1].toFixed(2)}</b> · {secSinif} · {d ? `Öğrenci ${d.ogrenciler.length} · Ort. Y-Eğim ${d.ortalamaYorgunluk.toFixed(2)}` : ''} [PRD §3.A deseninden MOCK]
                </div>
                <div className="mt-3 text-xs font-semibold text-slate-700">Ritim eğrisi — gün içi (sentetik-gösterim)</div>
                <svg width="100%" height={64} viewBox="0 0 280 64" className="mt-1" data-testid="sinif-egri">
                  <polyline points={noktalar(seri, 280, 64)} fill="none" stroke="#f59e0b" strokeWidth="2" />
                </svg>
                <div className="mt-3 space-y-1">
                  {(d?.ogrenciler ?? []).map((o) => (
                    <div key={o.id} className="flex items-center gap-2 text-xs">
                      <span className="w-16 font-semibold">{o.takmaAd}</span>
                      <span className="text-slate-500">Katılım {o.katilim.toFixed(2)} · Y-Eğim {o.yorgunluk.toFixed(2)} · görev {o.aktifGorev}</span>
                    </div>
                  ))}
                </div>
              </div>
            );
          })()}
        </div>
      )}

      {ekran === 'izleme' && (
        <div className="space-y-3">
          <h2 className="font-bold">Gelişim Takibi</h2>
          <p className="text-xs text-slate-500 mb-4">Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin.</p>
          <IzlemePaneli />
          <GelisimTakibi />
        </div>
      )}

      {ekran === 'ogrenci' && (
        <div className="space-y-3">
          <h2 className="font-bold">Öğrenci (Cihaz & Olay Dinleyicileri)</h2>
          <p className="text-sm text-slate-600">Öğrenci Terminal UI. EventListener başlama-kilitleri (PRD §3.B) planlı başlamayı gösterir — mini-simülasyonda deneyin.</p>
          <div className="grid md:grid-cols-3 gap-3">
            {GOREVLER.map((g) => (
              <button key={g.id} type="button" data-testid={`ogrenci-gorev-${g.id}`}
                onClick={() => { setSecGorev(g.id); setGeriSay(null); }}
                className={`text-left bg-white border p-3 rounded-xl shadow-sm cursor-pointer ${secGorev === g.id ? 'border-indigo-500 ring-2 ring-indigo-100' : 'border-slate-200'}`}>
                <div className="font-bold text-sm">{g.baslik}</div>
                <div className="text-xs text-slate-500">{g.dersId} | {g.modul}</div>
              </button>
            ))}
          </div>
          {secGorev && (() => {
            const g = GOREVLER.find((x) => x.id === secGorev)!;
            return (
              <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="ogrenci-gorev-detay">
                <div className="font-bold text-sm">{g.baslik} — Terminal önizlemesi (MOCK)</div>
                <p className="text-xs text-slate-600 mt-1">Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): aceleci tıklama yerine planlı başlama.</p>
                <button type="button" data-testid="ogrenci-baslama-kilidi" disabled={geriSay !== null}
                  onClick={() => setGeriSay(3)}
                  className={`mt-2 px-4 py-2 rounded-xl text-sm font-semibold ${geriSay !== null ? 'bg-slate-200 text-slate-400 cursor-not-allowed' : 'bg-indigo-600 text-white hover:bg-indigo-700'}`}>
                  {geriSay !== null ? `Kilit — ${geriSay} sn` : 'Göreve Başla (kilit-demosu)'}
                </button>
                {geriSay === null && <span className="ml-3 text-xs text-emerald-700 font-semibold" data-testid="ogrenci-gorev-acildi">Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir.</span>}
              </div>
            );
          })()}
        </div>
      )}

      {ekran === 'ogretmen' && (
        <div className="space-y-3">
          <h2 className="font-bold">Öğretmen Paneli (Teacher Cockpit)</h2>
          <Cockpit secSinif={secSinif} />
          <OneriSablonlari secSinif={secSinif} />
        </div>
      )}

      {ekran === 'transfer' && <TransferGozlemKarti />}

      {ekran === 'ders' && (
        <div className="space-y-3">
          <h2 className="font-bold">Ders & Görev</h2>
          <p className="text-sm text-slate-600">2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).</p>
          <GorevAtama />
          <SonucNotu />
        </div>
      )}

      {ekran === 'bep' && (
        <div className="space-y-3">
          <h2 className="font-bold">BEP Hazırlık</h2>
          <p className="text-sm text-slate-600">Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.</p>
          <BepHedef />
        </div>
      )}

      {ekran === 'veli' && (
        <div className="space-y-3">
          <h2 className="font-bold">Aile Bilgilendirme</h2>
          <p className="text-xs text-slate-500 mb-4">Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.</p>
          <p className="text-sm text-slate-600">Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).</p>
          <VeliKoprusu />
        </div>
      )}

      {ekran === 'eba' && (
        <div className="space-y-3">
          <h2 className="font-bold">MEB EBA Entegrasyonu</h2>
          <p className="text-xs text-slate-500 mb-4">Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.</p>
          <p className="text-sm text-slate-600">Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:</p>
          <EbaPaneli />
        </div>
      )}

      {ekran === 'ses' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf İçi Ses Yönetimi</h2>
          <p className="text-xs text-slate-500 mb-4">Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın.</p>
          <SesPaneli />
        </div>
      )}

      {ekran === 'rapor' && (
        <div className="space-y-3">
          <h2 className="font-bold">Rapor</h2>
          <RaporOzeti />
          <Portfoy />
        </div>
      )}

      {ekran === 'ayarlar' && (
        <div className="space-y-3">
          <h2 className="font-bold">Ayarlar</h2>
          <p className="text-sm text-slate-600">Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır.</p>
          <div className="flex flex-wrap gap-2">
            {SUBELER.map((s) => (
              <div key={s.id} className="text-xs bg-slate-50 p-2 rounded border">{s.ad} ({s.ogrenciSayisi} slot)</div>
            ))}
          </div>
          <p className="text-[11px] text-slate-500">MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda.</p>
        </div>
      )}

      {ekran === 'yardim' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sistem Kılavuzu ve Terimler</h2>
          <p className="text-xs text-slate-500 mb-4">Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu.</p>
          <div className="rounded-2xl border border-slate-200 bg-white p-4 text-xs space-y-2" data-testid="yardim-sozluk">
            <div><b>K-05:</b> Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır.</div>
            <div><b>K-02:</b> Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil.</div>
            <div><b>K-331:</b> MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok.</div>
            <div><b>K-334:</b> Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok).</div>
            <div><b>K-05/MOCK:</b> ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez.</div>
            <div><b>MOCK-değerleri:</b> <code>{JSON.stringify(KISITLAR)}</code></div>
          </div>
          <div className="rounded-2xl border border-slate-200 bg-white p-4 text-xs" data-testid="yardim-tur">
            <b>Hızlı-tur (PCV-brifing A–H ile uyumlu):</b> ① Pano'dan bir sınıf-kartına tıkla (nabız) → ② Sınıf'ta
            ritim eğrisini oku → ③ Öğrenci'de başlama-kilidi demosu → ④ <b>Transfer Gözlem (H-c)</b>: kartı 2 kez doldur
            (30-sn hedefi) → ⑤ Cockpit'te yorgunluk-satırları + Nefes Molası → ⑥ EBA'da salt-okunur akış + insight-taslağı
            → ⑦ Rapor'da görev-H not-önizlemesi → ⑧ Ses/İzleme'de sentetik-gösterimler.
          </div>
        </div>
      )}
    </Kabuk>
  );
}

~~~~

### `components/bep/BepHedef.tsx`

7347 B · SHA-256 `62fe87c1bb7025199114bbda17bd8cc76ad805a3125f2ff9b455e46d39de39a1`

~~~~tsx
/**
 * BEP HAZIRLIK — Hedef-şablonu + gözlem-probu izgarası (K-558 · Yol-2; gap-analizi).
 * Kazanım→BEP-hedef-ŞABLONU üretimi (öğretmen düzenler; resmî BEP belgesi BURADA YAZILMAZ —
 * sınıf-öncesi gözlem-hazırlığıdır). Periyodik-probu: haftalık 3-durum gözlem (var/kısmen/yok) →
 * İZGARA (her-hücre bir-probe; eğilim-yorumu YAPILMAZ — K-02/K-04). Ekosistem-köprüsü: MENTORIA
 * Z-17 kanıt-paketi TASLAK'ı kurum-tarafıyla konuşur. Defter yalnız-yerel (K-05).
 */
import { useState } from 'react';
import { Target } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';
import { MUFREDAT_2 } from '../../data/mufredatYonerge';

const DEFTER = 'scholaria_bep_defteri_v024';
interface Probe { tarih: string; durum: 0 | 1 | 2 } // 0=yok · 1=kısmen · 2=gözlemlendi
interface Hedef { id: string; ogrenci: string; kazanımKod: string; metin: string; probe: Probe[] }

function oku(): Hedef[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Hedef[]; } catch { return []; } }
function yaz(h: Hedef[]) { try { localStorage.setItem(DEFTER, JSON.stringify(h)); } catch { /* yerel-yalnız */ } }

const DURUM_ETIKET = ['yok', 'kısmen', 'gözlemlendi'];
const DURUM_RENK = ['bg-slate-100 text-slate-500', 'bg-amber-100 text-amber-700', 'bg-emerald-100 text-emerald-700'];

export default function BepHedef() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [kod, setKod] = useState(MUFREDAT_2[0].kod);
  const [hedefler, setHedefler] = useState<Hedef[]>(() => oku());

  const kazanım = MUFREDAT_2.find((m) => m.kod === kod)!;
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  const sablon =
    `GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir)\n` +
    `Öğrenci: ${o.takmaAd} (maske-ÖĞR) · Kazanım: ${kazanım.kod} — ${kazanım.ad}\n\n` +
    `Hedef-cümlesi (gözlemlenebilir-dil, K-14): ${o.takmaAd}, ${kazanım.ad.toLowerCase()} kazanımına bağlı ` +
    `sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: ${kazanım.yonerge}\n\n` +
    `İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara.\n` +
    `Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır.`;

  function hedefEkle() {
    const h: Hedef = { id: Math.random().toString(36).slice(2, 9), ogrenci, kazanımKod: kod, metin: sablon, probe: [] };
    const yeni = [h, ...hedefler]; setHedefler(yeni); yaz(yeni);
  }
  function probeEkle(id: string) {
    const yeni = hedefler.map((h) => h.id === id
      ? { ...h, probe: [...h.probe, { tarih: new Date().toISOString().slice(0, 10), durum: ([0, 1, 2] as const)[h.probe.length % 3] }] }
      : h);
    setHedefler(yeni); yaz(yeni);
  }
  function probeCevir(id: string, idx: number) {
    const yeni = hedefler.map((h) => h.id !== id ? h : { ...h, probe: h.probe.map((p, k) => k === idx ? { ...p, durum: ((p.durum + 1) % 3) as 0 | 1 | 2 } : p) });
    setHedefler(yeni); yaz(yeni);
  }
  function sil(id: string) {
    const yeni = hedefler.filter((x) => x.id !== id); setHedefler(yeni); yaz(yeni);
  }

  return (
    <div className="space-y-4" data-testid="bep-hazirlik">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>Sınır-şerhi:</b> Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu
        taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4 space-y-3">
        <h3 className="font-bold text-sm flex items-center gap-2"><Target className="w-4 h-4 text-indigo-600" /> Hedef-şablonu üretimi</h3>
        <div className="grid md:grid-cols-2 gap-2 text-xs">
          <label className="font-semibold text-slate-700">Öğrenci:
            <select data-testid="bep-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Kazanım:
            <select data-testid="bep-kazanim" value={kod} onChange={(e) => setKod(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {MUFREDAT_2.map((m) => <option key={m.kod} value={m.kod}>{m.kod} — {m.ad}</option>)}
            </select>
          </label>
        </div>
        <button type="button" data-testid="bep-sablon-uret" onClick={hedefEkle}
          className="px-4 py-2 rounded-xl bg-indigo-600 text-white text-sm font-semibold hover:bg-indigo-700">
          Hedef-şablonunu deftere ekle
        </button>
      </div>

      <div className="space-y-3">
        {hedefler.length === 0 ? (
          <p className="text-sm text-slate-500" data-testid="bep-bos">Defter boş — yukarıdan hedef-şablonu üretin.</p>
        ) : hedefler.slice(0, 6).map((h) => {
          const m = MUFREDAT_2.find((x) => x.kod === h.kazanımKod);
          const oo = OGRENCILER.find((x) => x.id === h.ogrenci);
          return (
            <div key={h.id} className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="bep-hedef-kart">
              <div className="flex items-center gap-2 text-xs">
                <span className="font-bold">{oo?.takmaAd}</span>
                <span className="text-slate-500">{h.kazanımKod} · {m?.ad}</span>
                <button type="button" onClick={() => sil(h.id)} className="ml-auto text-rose-600 text-[11px] font-semibold">sil</button>
              </div>
              <textarea readOnly rows={5} value={h.metin} data-testid="bep-sablon-metin"
                className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-[11px] font-mono" />
              <div className="mt-2 flex flex-wrap items-center gap-2 text-xs">
                <span className="font-semibold text-slate-700">Haftalık gözlem-probu izgarası ({h.probe.length}/4):</span>
                {h.probe.map((p, k) => (
                  <button key={k} type="button" data-testid={`bep-probe-${k}`} onClick={() => probeCevir(h.id, k)}
                    title="tıkla: durum değişir (yok→kısmen→gözlemlendi)"
                    className={`px-2 py-1 rounded-lg text-[10px] font-bold cursor-pointer ${DURUM_RENK[p.durum]}`}>
                    H{k + 1} · {p.tarih} · {DURUM_ETIKET[p.durum]}
                  </button>
                ))}
                {h.probe.length < 4 && (
                  <button type="button" onClick={() => probeEkle(h.id)} data-testid="bep-probe-ekle"
                    className="px-2 py-1 rounded-lg bg-slate-800 text-white text-[10px] font-bold">+ haftalık-probe ekle</button>
                )}
              </div>
              <p className="text-[11px] text-slate-500 mt-1">
                İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14).
              </p>
            </div>
          );
        })}
      </div>
    </div>
  );
}

~~~~

### `components/defter/SonucNotu.tsx`

3033 B · SHA-256 `968827d3432cc289c24040ee9be469ed390899d353c4823c42e4477219884abb`

~~~~tsx
/**
 * SONUÇ-NOTU DEFTERİ (K-555-4, SINIRLI-çerçeve): öğretmenin KENDİ sınıf-içi ölçme-işi (MEB öğretmeni
 * yapar) burada İŞLENMEZ — yalnız tarih + serbest-not defteri tutulur; kategori/eşik-yorumu ÜRETİLMEZ
 * (K-02/K-04: ürün ölçme-arağı değildir). "Ders & Görev" ekranına gömülü.
 */
import { useState } from 'react';
import { NotebookPen } from 'lucide-react';

const DEFTER = 'scholaria_sonuc_notu_v023';
interface Satir { id: string; zaman: string; metin: string }

function oku(): Satir[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Satir[]; } catch { return []; } }

export default function SonucNotu() {
  const [metin, setMetin] = useState('');
  const [satirlar, setSatirlar] = useState<Satir[]>(() => oku());

  function ekle() {
    if (!metin.trim()) return;
    const s: Satir = { id: Math.random().toString(36).slice(2, 9), zaman: new Date().toISOString(), metin: metin.trim() };
    const yeni = [s, ...satirlar]; setSatirlar(yeni); setMetin('');
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }
  function sil(id: string) {
    const yeni = satirlar.filter((x) => x.id !== id); setSatirlar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }

  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="sonuc-notu">
      <h3 className="font-bold text-sm flex items-center gap-2"><NotebookPen className="w-4 h-4 text-slate-600" /> Sınav/gözlem Sonuç-Notu Defteri (sınırlı)</h3>
      <p className="text-[11px] text-slate-500 mt-1">
        Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız.
        Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.
      </p>
      <div className="mt-2 flex gap-2">
        <input data-testid="sonuc-notu-gir" value={metin} onChange={(e) => setMetin(e.target.value)}
          placeholder='ör. "Pazartesi kısa-sayma-yazılısı — sınıf-geneli notu defterimde" (kategori-yazmayın)'
          className="flex-1 rounded-xl border border-slate-300 px-3 py-2 text-xs" />
        <button type="button" data-testid="sonuc-notu-ekle" onClick={ekle} className="px-3 py-2 rounded-xl bg-slate-800 text-white text-xs font-semibold">Deftere yaz</button>
      </div>
      <div className="mt-2 space-y-1">
        {satirlar.length === 0 ? (
          <p className="text-xs text-slate-500" data-testid="sonuc-bos">Defter boş.</p>
        ) : satirlar.slice(0, 6).map((s) => (
          <div key={s.id} data-testid="sonuc-satiri" className="flex items-center gap-2 text-[11px] rounded-lg border border-slate-200 px-2 py-1">
            <span className="text-slate-400">{s.zaman.slice(0, 10)}</span><span>{s.metin}</span>
            <button type="button" onClick={() => sil(s.id)} className="ml-auto text-rose-600 font-semibold">sil</button>
          </div>
        ))}
      </div>
    </div>
  );
}

~~~~

### `components/ders/GorevAtama.tsx`

6569 B · SHA-256 `6595fac05cd05f4b913ec1d3eef602382cb57b66ab8fb6fe229bb717a4cccce3`

~~~~tsx
/**
 * DERS & GÖREV — Görev Atama (K-555-1/5): öğretmen, MOCK-öğrenciye MEB-haritalı kazanım + etkinlik
 * ATAMASI yapar; kazanım-başına ders-işleme-yönergesi gösterilir (mufredatYonerge.ts — özgün).
 * Atama yalnız YEREL-deftere işlenir (K-05): çocuğa/cihaza gönderim YOKTUR; etkinliği çalıştıran
 * katman PERSONA'dır (MEB Ders Görevleri/Çocuk-modu) — SCHOLARIA atayan-katmandır.
 */
import { useState } from 'react';
import { BookOpen, ClipboardList } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';
import { MUFREDAT_2, MUFREDAT_KAYNAK_NOTU, MUFREDAT_SINIF } from '../../data/mufredatYonerge';

const DEFTER = 'scholaria_atama_defteri_v023';
interface Atama { id: string; zaman: string; ogrenci: string; kazanımKod: string; etkinlik: string }

function oku(): Atama[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Atama[]; } catch { return []; } }

export default function GorevAtama() {
  const [ders, setDers] = useState<'MAT' | 'TR'>('MAT');
  const [kod, setKod] = useState<string>(MUFREDAT_2[0].kod);
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [etkinlik, setEtkinlik] = useState(GOREVLER[0].id);
  const [atamalar, setAtamalar] = useState<Atama[]>(() => oku());

  const kazanım = MUFREDAT_2.find((m) => m.kod === kod)!;
  const listem = ders === 'MAT' ? MUFREDAT_2.filter((m) => m.ders === 'MAT') : MUFREDAT_2.filter((m) => m.ders === 'TR');

  function isle() {
    const a: Atama = { id: Math.random().toString(36).slice(2, 9), zaman: new Date().toISOString(), ogrenci, kazanımKod: kod, etkinlik };
    const yeni = [a, ...atamalar]; setAtamalar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }
  function sil(id: string) {
    const yeni = atamalar.filter((x) => x.id !== id); setAtamalar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }

  return (
    <div className="space-y-4" data-testid="gorev-atama">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>{MUFREDAT_SINIF} kazanım-ağacı</b> · {MUFREDAT_2.length} kazanım (Matematik 25 + Türkçe 37). {MUFREDAT_KAYNAK_NOTU}
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4 space-y-3">
        <div className="flex flex-wrap gap-2 items-center text-xs">
          <span className="font-semibold text-slate-700 flex items-center gap-1"><BookOpen className="w-4 h-4 text-indigo-600" /> Ders:</span>
          <button type="button" data-testid="ders-mat" onClick={() => { setDers('MAT'); setKod('MAT.2.1.1'); }}
            className={`px-3 py-1.5 rounded-xl font-semibold ${ders === 'MAT' ? 'bg-indigo-600 text-white' : 'bg-slate-100 text-slate-700'}`}>Matematik (25)</button>
          <button type="button" data-testid="ders-tr" onClick={() => { setDers('TR'); setKod('T.D.1.1'); }}
            className={`px-3 py-1.5 rounded-xl font-semibold ${ders === 'TR' ? 'bg-indigo-600 text-white' : 'bg-slate-100 text-slate-700'}`}>Türkçe (37)</button>
        </div>

        <div className="grid md:grid-cols-3 gap-2 text-xs">
          <label className="font-semibold text-slate-700">Kazanım:
            <select data-testid="mufredat-sec" value={kod} onChange={(e) => setKod(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {listem.map((m) => <option key={m.kod} value={m.kod}>{m.kod} — {m.ad}</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Öğrenci (maskeli):
            <select data-testid="atama-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {OGRENCILER.map((o) => <option key={o.id} value={o.id}>{o.takmaAd} ({o.id})</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Etkinlik:
            <select data-testid="atama-etkinlik" value={etkinlik} onChange={(e) => setEtkinlik(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {GOREVLER.map((g) => <option key={g.id} value={g.id}>{g.baslik}</option>)}
            </select>
          </label>
        </div>

        <div className="rounded-xl border border-indigo-200 bg-indigo-50 p-3 text-xs" data-testid="mufredat-yonerge">
          <b>Ders-işleme yönergesi ({kazanım.kod}):</b> {kazanım.yonerge}
        </div>

        <button type="button" data-testid="atama-isle" onClick={isle}
          className="px-4 py-2 rounded-xl bg-indigo-600 text-white text-sm font-semibold hover:bg-indigo-700">
          Atamayı deftere işle
        </button>
        <p className="text-[11px] text-slate-500">
          Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması
          PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.
        </p>
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><ClipboardList className="w-4 h-4 text-indigo-600" /> Atama-defteri ({atamalar.length})</h3>
        {atamalar.length === 0 ? (
          <p className="text-sm text-slate-500 mt-2" data-testid="atama-bos">Defter boş — yukarıdan atama işleyin.</p>
        ) : (
          <div className="mt-2 space-y-1.5">
            {atamalar.slice(0, 10).map((a) => {
              const o = OGRENCILER.find((x) => x.id === a.ogrenci);
              const g = GOREVLER.find((x) => x.id === a.etkinlik);
              const m = MUFREDAT_2.find((x) => x.kod === a.kazanımKod);
              return (
                <div key={a.id} data-testid="atama-satiri" className="flex items-center gap-2 text-xs rounded-xl border border-slate-200 px-3 py-2">
                  <span className="font-semibold">{o?.takmaAd}</span>
                  <span className="text-slate-500">{a.kazanımKod} · {m?.ad.slice(0, 32)}{m && m.ad.length > 32 ? '…' : ''}</span>
                  <span className="text-slate-400">{g?.baslik} · {a.zaman.slice(0, 10)}</span>
                  <button type="button" onClick={() => sil(a.id)} className="ml-auto text-rose-600 text-[11px] font-semibold">sil</button>
                </div>
              );
            })}
          </div>
        )}
      </div>
    </div>
  );
}

~~~~

### `components/ders/OneriSablonlari.tsx`

5225 B · SHA-256 `142a0aaa17d8e8acd2784c55fe21eb4fe57e83576ee1a25e2f74c7efd9384eac`

~~~~tsx
/**
 * ÖĞRENCİ EĞİTİMSEL DESTEK ÖNERİLERİ (Human-Accountable AI): davranış-gözlemine bağlı sınıf-yönlendirme-önerileri;
 * tanı/kişi-yargısı yok (K-02) — öğretmen-sözüyle yürütülür. Cockpit'in altında çalışır.
 */
import { useState } from 'react';
import { Brain } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';

const SABLONLAR = [
  'Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.',
  'İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma.',
  'Nefes Molası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.',
  'Yer-seçimi: çeldirici-anında öne-yakın sessiz-masa önerin.',
  'Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin.',
];

export default function OneriSablonlari({ secSinif }: { secSinif: string }) {
  const [secili, setSecili] = useState<number[]>([]);
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [yzMod, setYzMod] = useState(false);
  const [reddedildi, setReddedildi] = useState(false);
  
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  
  const metin = secili.length === 0 ? null :
    `EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · ${o.takmaAd} · ${secSinif}):\n` +
    secili.map((i) => `• ${SABLONLAR[i]}`).join('\n') +
    `\n\n⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer.`;
    
  return (
    <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="oneri-sablonlari">
      <h3 className="font-bold text-sm flex items-center gap-2 text-indigo-900"><Brain className="w-4 h-4 text-indigo-600" /> Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri</h3>
      <p className="text-[11px] text-indigo-700 leading-relaxed mb-3 mt-1">YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.</p>
      
      <div className="mt-2 flex items-center gap-2 text-xs">
        <span className="font-semibold text-slate-700">Öğrenci:</span>
        <select data-testid="oneri-ogrenci-sec" value={ogrenci} onChange={(e) => { setOgrenci(e.target.value); setYzMod(false); setReddedildi(false); setSecili([]); }} className="rounded-lg border border-slate-200 px-2 py-1">
          {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
        </select>
        {!yzMod && <button type="button" onClick={() => { setYzMod(true); setSecili([0, 2]); }} className="ml-2 bg-indigo-600 text-white px-3 py-1.5 rounded-lg font-semibold hover:bg-indigo-700">YZ Önerisi İste</button>}
      </div>
      
      {yzMod && !reddedildi && (
        <div className="mt-3">
          <div className="space-y-2 bg-white p-3 rounded-xl border border-indigo-100">
            <span className="text-[10px] font-bold text-amber-700 bg-amber-50 px-2 py-0.5 rounded-full border border-amber-200">BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı)</span>
            <p className="text-[11px] text-slate-600">Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin.</p>
            
            <div className="mt-2 space-y-1">
              {SABLONLAR.map((s, i) => (
                <label key={i} className="flex items-center gap-2 text-xs">
                  <input type="checkbox" data-testid={`oneri-${i}`} checked={secili.includes(i)}
                    onChange={() => setSecili((p) => (p.includes(i) ? p.filter((x) => x !== i) : [...p, i]))} />
                  {s}
                </label>
              ))}
            </div>
          </div>
          
          <div className="flex flex-wrap gap-2 mt-3">
            <button type="button" className="px-3 py-1.5 rounded-lg bg-teal-600 text-white text-xs font-semibold hover:bg-teal-700">✓ Onayla ve Yürürlüğe Al</button>
            <button type="button" onClick={() => setReddedildi(true)} className="px-3 py-1.5 rounded-lg bg-white border border-rose-200 text-rose-700 text-xs font-semibold hover:bg-rose-50">✕ Reddet ve Gerekçelendir</button>
          </div>
        </div>
      )}
      
      {reddedildi && (
         <div className="mt-3 p-3 bg-rose-50 border border-rose-200 rounded-xl space-y-2">
            <p className="text-xs font-bold text-rose-800">YZ Önerisi Öğretmen Tarafından Reddedildi</p>
            <input type="text" placeholder="Gerekçe (Örn: Sınıf dinamiklerine bugün uygun değil)" className="w-full text-xs p-2 rounded-lg border border-rose-300" />
            <button type="button" onClick={() => { setReddedildi(false); setYzMod(false); setSecili([]); }} className="px-3 py-1.5 bg-rose-600 text-white text-xs font-semibold rounded-lg mt-2">Kaydet</button>
         </div>
      )}
      
      {metin && yzMod && !reddedildi && <textarea readOnly rows={5} value={metin} data-testid="oneri-notu" className="w-full mt-3 rounded-xl border border-indigo-200 bg-white p-3 text-[11px] font-mono shadow-sm" />}
    </div>
  );
}
~~~~

### `components/eba/EbaPaneli.tsx`

4589 B · SHA-256 `3aa6da26a90473e259b6c48d2b8555eda27710edef51d038576a7d3e247d7361`

~~~~tsx
/**
 * MEB EBA — salt-okunur akış + yerel daily-insight TASLAĞI (K-554; PCV-brifing görev-F).
 * K-331: EBA'dan yalnız çağrılır, yazılmaz (ödev/içerik/e-sınav girişi YOK) · K-334 idari-mali dışarı ·
 * KVKK: EBA-UID cihazda maskelenir · [EBA POST] = PLANLI entegrasyon-adıdır — bu önizlemede ağ-gönderimi YOK (K-05).
 */
import { useState } from 'react';
import { ShieldCheck } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020'; // TransferGozlemKarti deposu — burada SALT-OKUNUR okunur
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

const DAVRANISLAR = [
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
];

export default function EbaPaneli() {
  const [taslak, setTaslak] = useState<string | null>(null);
  function uret() {
    let kayitlar: HcKayit[] = [];
    try { kayitlar = JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[]; } catch { kayitlar = []; }
    const satirlar = kayitlar.slice(0, 5).map((k) => {
      const o = OGRENCILER.find((x) => x.id === k.ogrenci);
      const g = GOREVLER.find((x) => x.id === k.gorev);
      const ilk = k.davranislar?.[0] !== undefined ? DAVRANISLAR[k.davranislar[0]] : 'gözlem-girişi';
      return `• ${o?.takmaAd ?? '•••'} (maske-UID ÖĞR-•••) — ${g?.baslik ?? 'görev'}: ${k.davranislar?.length ?? 0} davranış-gözlemi; ör. "${ilk}" (gözlemlenebilir-sayılabilir dil).`;
    });
    const govde = satirlar.length > 0
      ? satirlar.join('\n')
      : '• Bugün H-c kaydı yok — örnek-desen (sentetik): "ARD-05, Hece Avcısı görevi sırasında 2 kez görevi kendisi başlattı; 1 kez ipucu istedi ve sürdürdü."';
    setTaslak(
      'GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez)\n' +
      `Tarih: ${new Date().toISOString().slice(0, 10)} · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02)\n\n` +
      govde +
      '\n\n[Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA\'ya yazma-yok]'
    );
  }
  return (
    <div className="space-y-4" data-testid="eba-paneli">
      <div className="grid md:grid-cols-3 gap-3" data-testid="eba-akis">
        <div className="rounded-xl border border-slate-200 bg-white p-3 text-xs">
          <b>1 · Cihaz (Terminal)</b><br />EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
        </div>
        <div className="rounded-xl border border-slate-200 bg-white p-3 text-xs">
          <b>2 · daily-insight TASLAĞI</b><br />Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
        </div>
        <div className="rounded-xl border border-emerald-300 bg-emerald-50 p-3 text-xs">
          <b>3 · [EBA POST] /api/v1/report/daily-insight</b><br />
          <span data-testid="eba-yok-rozeti" className="inline-block mt-1 px-2 py-0.5 rounded-full bg-emerald-600 text-white font-bold">PLANLI ENTEGRASYON — bu önizlemede gönderim YOK</span>
        </div>
      </div>

      <div className="flex flex-wrap gap-2 text-[11px]">
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">K-331: salt-okunur çağrı — ödev/içerik yazılmaz</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">e-sınav girişi YOK</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">K-334: idari-mali otomasyon dışarı</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">Başarı Notu Yazılmaz · Maskeli UID</span>
      </div>

      <button type="button" data-testid="eba-taslagi-uret" onClick={uret}
        className="px-4 py-2 rounded-xl bg-emerald-600 text-white text-sm font-semibold hover:bg-emerald-700">
        Insight Taslağı Üret (yerel)
      </button>
      {taslak && (
        <textarea data-testid="eba-taslagi" readOnly value={taslak} rows={9}
          className="w-full rounded-xl border border-slate-300 p-3 text-xs font-mono" />
      )}
      <p className="text-[11px] text-slate-500 flex items-center gap-1">
        <ShieldCheck className="w-3.5 h-3.5" /> OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur;
        bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
      </p>
    </div>
  );
}

~~~~

### `components/izleme/FrictionMap.tsx`

4020 B · SHA-256 `7eb9534884375219f1fbd6734c51a5240c4753aa9d4a69e03217ca29b8cac3eb`

~~~~tsx
// K-649: SCHOLARIA - Öğrenme Sürtünme Haritası (Learning Friction Map)
// Öğretmen ekranında öğrencilerin zorlanma alanlarını (yanlış/doğru diye değil) 
// başlama, sürdürme ve sonlandırma süreçlerindeki direnç olarak ısı haritasıyla gösterir.

// React importu projede otomatik ekleniyorsa siliyoruz. TS6133
// import React from 'react';

// Persona modülünden (patternStore) aktarılacak olan varsayımsal kanıt verisi
interface OgrenciFrictionVerisi {
  ogrenciAd: string;
  gorevKodu: string;
  baslamaDirenc: 'dusuk' | 'orta' | 'yuksek';
  surdurmeDirenc: 'dusuk' | 'orta' | 'yuksek';
  gecisDirenc: 'dusuk' | 'orta' | 'yuksek';
}

const MOCK_DATA: OgrenciFrictionVerisi[] = [
  { ogrenciAd: 'Ali Y.', gorevKodu: 'MAT-02', baslamaDirenc: 'yuksek', surdurmeDirenc: 'dusuk', gecisDirenc: 'orta' },
  { ogrenciAd: 'Ayşe T.', gorevKodu: 'TR-05', baslamaDirenc: 'dusuk', surdurmeDirenc: 'orta', gecisDirenc: 'dusuk' },
  { ogrenciAd: 'Can B.', gorevKodu: 'MAT-02', baslamaDirenc: 'orta', surdurmeDirenc: 'yuksek', gecisDirenc: 'yuksek' },
];

const getColor = (seviye: string) => {
  switch (seviye) {
    case 'dusuk': return 'bg-green-100 text-green-700'; // Akıcı
    case 'orta': return 'bg-yellow-100 text-yellow-700'; // Gecikmeli
    case 'yuksek': return 'bg-red-100 text-red-700'; // Dirençli (Kopma noktası)
    default: return 'bg-slate-100 text-slate-500';
  }
};

export default function FrictionMap() {
  return (
    <div className="p-5 bg-white rounded-lg shadow border border-slate-200">
      <div className="mb-4 border-b pb-2">
        <h2 className="text-lg font-bold text-slate-800">Öğrenme Sürtünme Haritası (Friction Map)</h2>
        <p className="text-xs text-slate-500">Öğrencilerin görev aşamalarındaki bilişsel dirençlerini ve kopma noktalarını gösterir.</p>
      </div>

      <div className="overflow-x-auto">
        <table className="w-full text-left text-sm">
          <thead>
            <tr className="bg-slate-50 border-b">
              <th className="p-2 font-medium text-slate-600">Öğrenci</th>
              <th className="p-2 font-medium text-slate-600">Görev</th>
              <th className="p-2 font-medium text-slate-600">Başlama Direnci</th>
              <th className="p-2 font-medium text-slate-600">Görev Sürdürme</th>
              <th className="p-2 font-medium text-slate-600">Geçiş / Sonlandırma</th>
            </tr>
          </thead>
          <tbody>
            {MOCK_DATA.map((veri, idx) => (
              <tr key={idx} className="border-b last:border-0 hover:bg-slate-50">
                <td className="p-2 font-medium">{veri.ogrenciAd}</td>
                <td className="p-2 text-slate-500">{veri.gorevKodu}</td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.baslamaDirenc)}`}>
                    {veri.baslamaDirenc.toUpperCase()}
                  </span>
                </td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.surdurmeDirenc)}`}>
                    {veri.surdurmeDirenc.toUpperCase()}
                  </span>
                </td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.gecisDirenc)}`}>
                    {veri.gecisDirenc.toUpperCase()}
                  </span>
                </td>
              </tr>
            ))}
          </tbody>
        </table>
      </div>
      
      <div className="mt-4 p-3 bg-blue-50 text-blue-800 text-xs rounded border border-blue-200">
        <strong>Eğitsel Çıkarım Örneği:</strong> Ali'nin MAT-02 görevine başlaması çok zor (Yüksek Direnç) ancak başladıktan sonra akıcı bir şekilde bitiriyor (Düşük Sürdürme Direnci). Ali'ye göreve başlarken kısa bir görsel tetikleyici vermek sürtünmeyi (friction) kırabilir.
      </div>
    </div>
  );
}

~~~~

### `components/izleme/IzlemePaneli.tsx`

2540 B · SHA-256 `12757afe78e10df25a342cdecee6c99f355676d270a3eb1c88b40e25aa156b5f`

~~~~tsx
/**
 * İzleme — yanıt zamanı eğimi öğrenci-serisi (K-554; PCV-brifing görev-G-izleme).
 * Sentetik-gösterim (K-05); XR/Görev-panosu Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
 * K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.
 */
import { useState } from 'react';
import { OGRENCILER } from '../../data/mock';
import { yanitSeri, noktalar } from '../../data/seriler';

export default function IzlemePaneli() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  return (
    <div className="space-y-4" data-testid="izleme-paneli">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>MOCK:</b> seriler sentetik-gösterimdir (K-05); XR/Görev-panosu Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
      </div>
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <label className="text-xs font-semibold text-slate-700">
          Öğrenci (maskeli):
          <select data-testid="izleme-ogrenci-sec" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)}
            className="ml-2 rounded-lg border border-slate-200 px-2 py-1 text-xs">
            {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
          </select>
        </label>
        <div className="mt-3 grid md:grid-cols-2 gap-4">
          <div>
            <div className="text-xs font-semibold text-slate-700">Yanıt zamanı eğimi — {o.takmaAd} (12 gözlem-noktası)</div>
            <svg width="100%" height={64} viewBox="0 0 280 64" className="mt-1" data-testid="izleme-egri">
              <polyline points={noktalar(yanitSeri(o.id), 280, 64)} fill="none" stroke="#0ea5e9" strokeWidth="2" />
            </svg>
          </div>
          <div className="text-xs space-y-2">
            <div className="rounded-xl border border-slate-200 p-3">
              <b>Görev etkileşim oranı:</b> %88.4 <span className="text-slate-400">(sentetik-sabit · Faz-3 Görev-M11)</span>
            </div>
            <div className="rounded-xl border border-slate-200 p-3">
              <b>Aktif görev:</b> {o.aktifGorev} · <b>Katılım:</b> {o.katilim.toFixed(2)} · <b>Y-Eğim:</b> {o.yorgunluk.toFixed(2)}
            </div>
            <div className="text-[11px] text-slate-500">K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.</div>
          </div>
        </div>
      </div>
    </div>
  );
}

~~~~

### `components/ogretmen/Cockpit.tsx`

4742 B · SHA-256 `a3e853d35710a759f109963c1b28fafa326b9098a6f3e1b7bb2b84b09af14afb`

~~~~tsx
/**
 * Öğretmen Paneli (Teacher Cockpit) — K-554 CANLI (PCV-brifing görev-E).
 * Toplu yorgunluk eğimi satırları + yanıt zamanı eğimi sınıf-eğrisi + Nefes Molası yönlendirme-kartı.
 * Sentetik veri (K-05 MOCK): yorgunluk/katılım değerleri gösterim-verisidir — sensör-akışı DEĞİLDİR;
 * "ölçen değil, gözlemleyen" konumu (K-02): eşik-geçene YÖNLENDİRME-önerisi üretilir, ölçüm/tanı yok.
 */
import { useState } from 'react';
import { GraduationCap, Wind } from 'lucide-react';
import { SINIF_DURUMU } from '../../data/mock';
import { yanitSeri, noktalar } from '../../data/seriler';

export default function Cockpit({ secSinif }: { secSinif: string }) {
  const [yonlendirildi, setYonlendirildi] = useState(false);
  const durum = SINIF_DURUMU.find((s) => s.sinifId === secSinif);
  const ogrenciler = durum?.ogrenciler ?? [];
  const alarmli = ogrenciler.filter((o) => o.yorgunluk >= 0.07);
  const egri = yanitSeri('SNF' + secSinif);
  const renk = (f: number) => (f >= 0.07 ? 'bg-rose-500' : f >= 0.05 ? 'bg-amber-500' : 'bg-emerald-500');
  return (
    <div className="space-y-4" data-testid="cockpit">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>MOCK:</b> tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için
        yönlendirme-desteğidir (K-02) · eşik-önerisi: Y-Eğim ≥ 0.07 → Nefes Molası.
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><GraduationCap className="w-4 h-4 text-indigo-600" /> Toplu Yorgunluk Eğimi — {secSinif}</h3>
        <div className="mt-3 space-y-2" data-testid="cockpit-fsatirlari">
          {ogrenciler.map((o) => (
            <div key={o.id} className="flex items-center gap-2 text-xs">
              <span className="w-16 font-semibold">{o.takmaAd}</span>
              <div className="flex-1 h-3 rounded-full bg-slate-100 overflow-hidden">
                <div className={`h-full ${renk(o.yorgunluk)}`} style={{ width: `${Math.min(100, o.yorgunluk * 900)}%` }} />
              </div>
              <span className="w-24 text-right text-slate-500">Y-Eğim {o.yorgunluk.toFixed(2)}</span>
              <span className="w-20 text-right text-slate-400">Katılım {o.katilim.toFixed(2)}</span>
              {o.yorgunluk >= 0.07 && <span className="text-[10px] px-1.5 py-0.5 rounded-full bg-rose-100 text-rose-700 font-bold">yorgunluk-uyarısı</span>}
            </div>
          ))}
        </div>
        <div className="mt-4">
          <div className="text-xs font-semibold text-slate-700">Yanıt zamanı eğimi sınıf-eğrisi (sentetik-gösterim)</div>
          <svg width={280} height={56} className="mt-1" data-testid="cockpit-egri">
            <polyline points={noktalar(egri, 280, 56)} fill="none" stroke="#4f46e5" strokeWidth="2" />
          </svg>
        </div>
      </div>

      <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="cockpit-nefes">
        <h3 className="font-bold text-sm flex items-center gap-2"><Wind className="w-4 h-4 text-indigo-600" /> Nefes Molası (4-4-4)</h3>
        <div className="mt-2 flex items-center gap-4">
          <div className="relative w-16 h-16 shrink-0">
            <div className="absolute inset-0 rounded-full bg-indigo-300 animate-ping opacity-60" />
            <div className="absolute inset-2 rounded-full bg-indigo-500 opacity-80" />
          </div>
          <div className="text-xs text-slate-700">
            Kılavuz-tempo: <b>4 sn al — 4 sn tut — 4 sn ver</b> · sınıf-öncesi/arası 2 tur.<br />
            {alarmli.length > 0
              ? <span className="text-rose-700 font-semibold">{alarmli.length} öğrenci eşik-üstü → yönlendirme-önerisi hazır.</span>
              : 'Eşik-üstü öğrenci yok.'}
          </div>
        </div>
        <button type="button" data-testid="cockpit-yonlendir" onClick={() => setYonlendirildi(true)}
          className="mt-3 px-3 py-1.5 rounded-xl bg-indigo-600 text-white text-xs font-semibold hover:bg-indigo-700">
          Yönlendirme-kartı üret
        </button>
        {yonlendirildi && (
          <div className="mt-2 rounded-xl bg-white border border-indigo-200 p-3 text-xs" data-testid="cockpit-yonlendirme-karti">
            <b>{secSinif} — gözlem-notu (MOCK):</b> {alarmli.length > 0 ? alarmli.map((a) => a.takmaAd).join(', ') : 'sınıf-geneli'} için
            Nefes Molası tempo (4-4-4) denenebilir. Bu kart cihaza komut GÖNDERMEZ; öğretmen-sözüyle yürütülür.
          </div>
        )}
      </div>
    </div>
  );
}

~~~~

### `components/ogretmen/TransferGozlemKarti.tsx`

6843 B · SHA-256 `054db5d944b131928f7d4ce02d5f858316d58b057f946d86fe2a5be342ecfd60`

~~~~tsx
/**
 * H(c) — Transfer Gözlem Kartı MOCK (öğretmen formu) · K-451 (P/S kod turu ②)
 * Yerleşim Taslağı v1.0 §3-14: ≤30 sn tek ekran; 3'lü Likert YERİNE davranışsal giriş;
 * sentetik/yerel-önce (K-05). Kişi değerlendirmesi YOK — yalnız gözlenen davranış kaydı (K-02).
 */
import { useEffect, useState } from 'react';
import { ClipboardCheck, Save, Trash2 } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020';

// Davranış anahtarları (Likert değil; "gözlendi / gözlenmedi" girişi)
const DAVRANISLAR = [
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
] as const;

interface HcKayit {
  id: string;
  ogrenci: string;
  gorev: string;
  davranislar: number[];
  not: string;
  zaman: string;
}

function kayitlariOku(): HcKayit[] {
  try {
    return JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[];
  } catch {
    return [];
  }
}

export default function TransferGozlemKarti() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [gorev, setGorev] = useState(GOREVLER[0].id);
  const [secili, setSecili] = useState<number[]>([]);
  const [not, setNot] = useState('');
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);

  useEffect(() => { setKayitlar(kayitlariOku()); }, []);

  function davranisDegistir(i: number) {
    setSecili(oncesi => oncesi.includes(i) ? oncesi.filter(x => x !== i) : [...oncesi, i]);
  }

  function kaydet() {
    const o = OGRENCILER.find(x => x.id === ogrenci);
    const g = GOREVLER.find(x => x.id === gorev);
    const yeni: HcKayit = {
      id: 'HC-' + Date.now(),
      ogrenci: o ? o.takmaAd : ogrenci,
      gorev: g ? g.baslik : gorev,
      davranislar: secili,
      not: not.trim(),
      zaman: new Date().toLocaleString('tr-TR'),
    };
    const guncel = [yeni, ...kayitlar].slice(0, 20);
    localStorage.setItem(ANAHTAR, JSON.stringify(guncel));
    setKayitlar(guncel);
    setSecili([]); setNot('');
  }

  function hepsiniSil() {
    localStorage.removeItem(ANAHTAR);
    setKayitlar([]);
  }

  return (
    <div data-testid="hc-kart" className="space-y-3 max-w-2xl">
      <div className="flex items-center gap-3">
        <div className="w-10 h-10 rounded-xl bg-indigo-100 grid place-items-center">
          <ClipboardCheck size={20} className="text-indigo-700" />
        </div>
        <div>
          <h2 className="font-bold">Transfer Gözlem Kartı</h2>
          <p className="text-xs text-slate-500 mb-4">Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.</p>
          <p className="text-xs text-slate-500">
            Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı.
            Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).
          </p>
        </div>
      </div>

      <div className="bg-amber-50 border border-amber-200 rounded-lg px-3 py-1.5 text-[11px] font-semibold text-amber-800" data-testid="hc-mock-rozet">
        MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
      </div>

      <div className="grid grid-cols-2 gap-2">
        <label className="text-xs font-semibold text-slate-700">
          Öğrenci (sentetik):
          <select data-testid="hc-ogrenci-sec" value={ogrenci} onChange={e => setOgrenci(e.target.value)}
            className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs">
            {OGRENCILER.map(o => <option key={o.id} value={o.id}>{o.takmaAd} ({o.id})</option>)}
          </select>
        </label>
        <label className="text-xs font-semibold text-slate-700">
          Gözlenen etkinlik:
          <select data-testid="hc-gorev-sec" value={gorev} onChange={e => setGorev(e.target.value)}
            className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs">
            {GOREVLER.map(g => <option key={g.id} value={g.id}>{g.baslik}</option>)}
          </select>
        </label>
      </div>

      <div className="space-y-1.5">
        <div className="text-xs font-semibold text-slate-700">Gözlenen davranışlar (işaretleyerek):</div>
        {DAVRANISLAR.map((d, i) => {
          const akt = secili.includes(i);
          return (
            <button key={i} type="button" data-testid={`hc-davranis-${i}`} onClick={() => davranisDegistir(i)}
              className={`w-full text-left px-3 py-2 rounded-xl border text-xs transition-colors ${
                akt ? 'bg-indigo-600 text-white border-indigo-600 font-semibold'
                    : 'bg-white text-slate-700 border-slate-200 hover:bg-slate-50'}`}>
              {akt ? '✓ ' : '○ '}{d}
            </button>
          );
        })}
      </div>

      <label className="block text-xs font-semibold text-slate-700">
        Kısa not (isteğe bağlı):
        <input data-testid="hc-not" value={not} maxLength={140} onChange={e => setNot(e.target.value)}
          placeholder="Örn. tahta örneğinden sonra kendi uygulamasına geçti"
          className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs" />
      </label>

      <div className="flex items-center gap-2">
        <button type="button" data-testid="hc-kaydet" onClick={kaydet}
          className="inline-flex items-center gap-1.5 bg-indigo-600 text-white text-xs font-semibold px-4 py-2 rounded-xl hover:bg-indigo-700">
          <Save size={14} /> Kaydet (yerel)
        </button>
        <span data-testid="hc-kayit-sayisi" className="text-[11px] text-slate-500">
          {kayitlar.length} kayıt · yalnız bu tarayıcıda
        </span>
      </div>

      {kayitlar.length > 0 && (
        <div className="space-y-1.5">
          <div className="flex items-center justify-between">
            <div className="text-xs font-semibold text-slate-700">Son kayıtlar:</div>
            <button type="button" data-testid="hc-temizle" onClick={hepsiniSil}
              className="inline-flex items-center gap-1 text-[11px] text-slate-400 hover:text-red-500">
              <Trash2 size={12} /> hepsini temizle
            </button>
          </div>
          {kayitlar.slice(0, 5).map((k, i) => (
            <div key={k.id} data-testid={`hc-kayit-${i}`}
              className="border border-slate-200 rounded-lg px-3 py-2 text-[11px] bg-white">
              <b>{k.ogrenci}</b> · {k.gorev} · {k.davranislar.length} davranış
              {k.not ? ` · “${k.not}”` : ''} <span className="text-slate-400">({k.zaman})</span>
            </div>
          ))}
        </div>
      )}
    </div>
  );
}

~~~~

### `components/portfoy/Portfoy.tsx`

4755 B · SHA-256 `c23e69cb4b94a5575387d684c36edddcdf0f3f2a916c2861a0ea2bdd64c07b1e`

~~~~tsx
/**
 * ÖĞRENCİ DEFTERİ — yazılı-portfolyo (K-559 · Yol-3; Seesaw-deseninin K-05-metin-yalnız uyarlaması).
 * 4-yerel-defteri (H-c gözlem · atama · BEP-probe · sonuç-notu) SALT-OKUNUR birleştirip
 * öğrenci-bazlı zaman-çizelgesi sunar. Görüntü/ses-yükleme YOK; yazdırma/dışa-aktarım YOK
 * (PCV-kural-1); gerçek-rapor-çıktısı planlı-katmandır. Kimlik: yalnız maskeli-takma-ad (K-05).
 */
import { useEffect, useState } from 'react';
import { FolderOpen } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';

const KAYNAKLAR = [
  { anahtar: 'scholaria_hc_kayitlar_v020', ad: 'Gözlem-kartı (H-c)' },
  { anahtar: 'scholaria_atama_defteri_v023', ad: 'Görev-ataması' },
  { anahtar: 'scholaria_bep_defteri_v024', ad: 'BEP-hazırlık' },
  { anahtar: 'scholaria_sonuc_notu_v023', ad: 'Sonuç-notu' },
] as const;

interface Satir { kaynak: string; zaman: string; metin: string }

function topla(ogrenci: string): Satir[] {
  const satirlar: Satir[] = [];
  function ekle(anahtar: string, ad: string, sec: (r: Record<string, unknown>) => { zaman: string; metin: string } | null) {
    try {
      const liste = JSON.parse(localStorage.getItem(anahtar) ?? '[]') as Array<Record<string, unknown>>;
      liste.filter((r) => !r.ogrenci || r.ogrenci === ogrenci).forEach((r) => {
        const s = sec(r);
        if (s) satirlar.push({ kaynak: ad, zaman: s.zaman, metin: s.metin });
      });
    } catch { /* yerel-okuma-hatası — yoksay */ }
  }
  ekle(KAYNAKLAR[0].anahtar, KAYNAKLAR[0].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `${r.gorev ?? 'görev'}: ${(r.davranislar as number[] | undefined)?.length ?? 0} davranış-gözlemi${r.not ? ` · "${String(r.not)}"` : ''}`,
  }));
  ekle(KAYNAKLAR[1].anahtar, KAYNAKLAR[1].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `etkinlik atandı: ${r.etkinlik ?? ''} · kazanım ${r.kazanımKod ?? r.kazanimKod ?? ''}`,
  }));
  ekle(KAYNAKLAR[2].anahtar, KAYNAKLAR[2].ad, (r) => ({
    zaman: '—', metin: `BEP-hazırlık hedefi (${r.kazanımKod ?? r.kazanimKod ?? ''}) · ${(r.probe as unknown[] | undefined)?.length ?? 0} haftalık-probu`,
  }));
  ekle(KAYNAKLAR[3].anahtar, KAYNAKLAR[3].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `sonuç-notu: "${String(r.metin ?? '')}"`,
  }));
  return satirlar.sort((a, b) => b.zaman.localeCompare(a.zaman));
}

export default function Portfoy() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [satirlar, setSatirlar] = useState<Satir[]>([]);
  const [taze, setTaze] = useState(0);
  useEffect(() => { setSatirlar(topla(ogrenci)); }, [ogrenci, taze]);

  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="portfoy">
      <h3 className="font-bold text-sm flex items-center gap-2"><FolderOpen className="w-4 h-4 text-indigo-600" /> Öğrenci Defteri — yazılı-portfolyo</h3>
      <div className="mt-2 flex flex-wrap gap-2 items-center text-xs">
        <label className="font-semibold text-slate-700">Öğrenci:
          <select data-testid="portfoy-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="ml-2 rounded-lg border border-slate-200 px-2 py-1">
            {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
          </select>
        </label>
        <button type="button" data-testid="portfoy-tazele" onClick={() => setTaze((t) => t + 1)} className="px-3 py-1.5 rounded-xl bg-indigo-600 text-white font-semibold">Defterleri tara</button>
        <span className="text-[11px] text-slate-500">{satirlar.length} kayıt · 4-defter salt-okunur</span>
      </div>
      {satirlar.length === 0 ? (
        <p className="text-sm text-slate-500 mt-2" data-testid="portfoy-bos">Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.</p>
      ) : (
        <div className="mt-3 space-y-1.5" data-testid="portfoy-zaman-cizelgesi">
          {satirlar.slice(0, 14).map((s, i) => (
            <div key={i} className="text-xs rounded-xl border border-slate-200 px-3 py-2">
              <span className="inline-block text-[10px] font-bold px-1.5 py-0.5 rounded-full bg-slate-100 text-slate-600 mr-2">{s.kaynak}</span>
              <span className="text-slate-400 text-[10px] mr-2">{s.zaman ? s.zaman.slice(0, 10) : ''}</span>
              {s.metin}
            </div>
          ))}
        </div>
      )}
      <p className="text-[11px] text-slate-500 mt-2">
        Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla
        bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
      </p>
    </div>
  );
}

~~~~

### `components/rapor/RaporOzeti.tsx`

3034 B · SHA-256 `116a78db9a529d4f59a515c252dc084a4ceca28554f0315565ab88b6059eadc8`

~~~~tsx
/**
 * Rapor — Günlük Ev–Okul gözlem-notu ÖNİZLEMESİ (K-554; PCV-brifing görev-H).
 * H(c) Transfer-kayıtlarından (localStorage, salt-okunur) gözlemlenebilir-sayılabilir dil üretir.
 * Bu ekranda yazdırma/dışa-aktarım YOKTUR (PCV-kural-1); gerçek-rapor-çıktısı planlı-katmandır.
 */
import { useEffect, useState } from 'react';
import { FileText } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020'; // TransferGozlemKarti deposu — salt-okunur
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

const DAVRANISLAR = [ // TransferGozlemKarti listesiyle aynıdır (kaynak-orası; burada salt-okunur gösterim)
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
];

export default function RaporOzeti() {
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);
  useEffect(() => {
    try { setKayitlar(JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[]); } catch { setKayitlar([]); }
  }, []);
  const notlar = kayitlar.slice(0, 8).map((k) => {
    const o = OGRENCILER.find((x) => x.id === k.ogrenci);
    const g = GOREVLER.find((x) => x.id === k.gorev);
    const d = k.davranislar?.map((i) => `"${DAVRANISLAR[i] ?? 'gözlem'}"`).join(', ');
    return `• ${o?.takmaAd ?? '•••'} — ${g?.baslik ?? 'görev'}: ${d || 'gözlem-girişi yok'}${k.not ? `; öğretmen-notu: "${k.not}"` : ''}. (${k.zaman?.slice(0, 10) ?? ''})`;
  });
  return (
    <div className="space-y-4" data-testid="rapor-ozeti">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>Görev-H deseni:</b> "40 dk derste 3 kez yerinden kalktı" tipi <b>gözlemlenebilir-sayılabilir dil</b>.
        Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
      </div>
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><FileText className="w-4 h-4 text-indigo-600" /> Günün Ev–Okul Notu Taslağı (H-c kaynaklı)</h3>
        {notlar.length === 0 ? (
          <p className="text-sm text-slate-500 mt-2" data-testid="rapor-bos">
            Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.
          </p>
        ) : (
          <textarea readOnly rows={7} value={notlar.join('\n')} data-testid="rapor-not-ornegi"
            className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-xs font-mono" />
        )}
        <p className="text-[11px] text-slate-500 mt-2">
          Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.
        </p>
      </div>
    </div>
  );
}

~~~~

### `components/ses/SesPaneli.tsx`

2419 B · SHA-256 `7f48dcf19642652e6c0e4341228679b96fb6972fa2264d0226281932f5505fd6`

~~~~tsx
/**
 * Ses Ortamı Yönetimi — ana-sinyal izolasyonu GÖRSEL-simülasyonu (K-554; PCV-brifing görev-G).
 * Bu önizlemede ses-işleme/donanım YOKTUR (planlı-katman): dalga-grafiği sentetik-gösterimdir (K-05/K-02).
 */
import { useState } from 'react';
import { noktalar } from '../../data/seriler';

const ANA = noktalar(Array.from({ length: 48 }, (_, i) => 0.5 + 0.32 * Math.sin(i * 0.55)), 480, 80);
const GURULTU = noktalar(Array.from({ length: 48 }, (_, i) => 0.5 + 0.3 * Math.sin(i * 2.3) * (0.4 + 0.6 * Math.abs(Math.sin(i * 0.9)))), 480, 80);

export default function SesPaneli() {
  const [izolasyon, setIzolasyon] = useState(60);
  return (
    <div className="space-y-4" data-testid="ses-paneli">
      <div className="bg-amber-50 border border-amber-200 rounded-xl px-3 py-2 text-[11px] text-amber-900" data-testid="ses-planli">
        <b>PLANLI-KATMAN şerhi:</b> donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü
        ayrımının <b>görsel-simülasyonu</b> vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik).
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm">Ana Sinyal İzolasyonu — {izolasyon}%</h3>
        <input type="range" min={0} max={100} value={izolasyon} data-testid="ses-slider"
          onChange={(e) => setIzolasyon(Number(e.target.value))} className="w-full mt-2" />
        <svg width="100%" height={80} viewBox="0 0 480 80" className="mt-2 bg-slate-50 rounded-xl" data-testid="ses-dalga">
          <polyline points={GURULTU} fill="none" stroke="#f59e0b" strokeWidth="1.5" opacity={Math.max(0.06, 1 - izolasyon / 100)} />
          <polyline points={ANA} fill="none" stroke="#4f46e5" strokeWidth="2" />
        </svg>
        <div className="flex gap-3 mt-2 text-[11px] text-slate-600">
          <span className="flex items-center gap-1"><span className="w-3 h-0.5 bg-indigo-600 inline-block" /> ana-sinyal</span>
          <span className="flex items-center gap-1"><span className="w-3 h-0.5 bg-amber-500 inline-block" /> ortam-gürültüsü (izolasyon-arttıkça söner)</span>
        </div>
      </div>

      <label className="flex items-center gap-2 text-xs text-slate-600">
        <input type="checkbox" disabled /> Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır)
      </label>
    </div>
  );
}

~~~~

### `components/shell/Kabuk.tsx`

3302 B · SHA-256 `dd2a74a0442ac2861f44aa859a4feee5672f5e26257c07227a759b76b916e6a9`

~~~~tsx
/** LEXIVA Scholaria kabuğu: B2B sınıf düğümü (Bilişsel Gelişim Laboratuvarı; K-700 ÖÖG uyarlama). Kurumsal panel; öğrenci/öğretmen/sınıf/yönetici rolleri. */
import type { ReactNode } from 'react';
import { LayoutDashboard, Users, GraduationCap, FileText, Settings, Activity, Database, ShieldCheck, HelpCircle, BarChart3, ClipboardCheck, BookOpen, HeartHandshake, Target } from 'lucide-react';

export const EKRANLAR = [
  { id: 'pano', ad: 'Sınıf Özeti', ikon: LayoutDashboard },
  { id: 'sinif', ad: 'Sınıf', ikon: Activity },
  { id: 'ogrenci', ad: 'Öğrenci', ikon: Users },
  { id: 'ogretmen', ad: 'Öğretmen', ikon: GraduationCap },
  { id: 'transfer', ad: 'Transfer Gözlem Kartı', ikon: ClipboardCheck },
  { id: 'ders', ad: 'Ders & Görev', ikon: BookOpen },
  { id: 'veli', ad: 'Aile Bilgilendirme', ikon: HeartHandshake },
  { id: 'bep', ad: 'BEP Hazırlık', ikon: Target },
  { id: 'eba', ad: 'MEB EBA Entegrasyonu', ikon: Database },
  { id: 'izleme', ad: 'Gelişim Takibi', ikon: BarChart3 },
  { id: 'ses', ad: 'Sınıf İçi Ses Yönetimi', ikon: ShieldCheck },
  { id: 'rapor', ad: 'Rapor', ikon: FileText },
  { id: 'ayarlar', ad: 'Ayarlar', ikon: Settings },
  { id: 'yardim', ad: 'Sistem Kılavuzu ve Terimler', ikon: HelpCircle },
] as const;
export type EkranId = (typeof EKRANLAR)[number]['id'];

export default function Kabuk({ ekran, setEkran, rol, children }:
  { ekran: EkranId; setEkran: (e: EkranId) => void; rol: string; children: ReactNode }) {
  return (
    <div className="min-h-screen flex">
      <aside className="w-60 bg-white border-r border-slate-200 flex flex-col shrink-0">
        <div className="px-4 py-4 border-b border-slate-100">
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 rounded-xl bg-indigo-600 text-white grid place-items-center font-black">S</div>
            <div>
              <div className="font-bold text-sm">LEXIVA Scholaria™</div>
              <div className="text-[10px] text-slate-500">School Node · v{__SURUM__}</div>
            </div>
          </div>
        </div>
        <nav className="flex-1 p-2 space-y-0.5">
          {EKRANLAR.map((e) => {
            const I = e.ikon; const akt = ekran === e.id;
            return (
              <button key={e.id} type="button" data-testid={`nav-${e.id}`} onClick={() => setEkran(e.id)}
                className={`w-full flex items-center gap-2 px-3 py-2 rounded-xl text-sm transition-colors ${
                  akt ? 'bg-indigo-600 text-white font-semibold' : 'text-slate-700 hover:bg-slate-100'}`}>
                <I className="w-4 h-4" /> {e.ad}
              </button>
            );
          })}
        </nav>
        <div className="p-3 border-t border-slate-100 text-[10px] text-slate-500">
          Rol: <b>{rol}</b> · B2B Sınıf Düğümü (School Node)
        </div>
      </aside>
      <main className="flex-1 min-w-0">
        <div className="bg-white border-b border-slate-200 px-6 py-2">
          <p className="text-[11px] text-slate-600"><b>LEXIVA Scholaria:</b> Toplu sınıf içi bilişsel gelişim laboratuvarı — ritim ve yorgunluk kalibrasyon düğümü (B2B).</p>
        </div>
        <div className="p-6 space-y-5 max-w-6xl">{children}</div>
      </main>
    </div>
  );
}

~~~~

### `components/takip/GelisimTakibi.tsx`

3156 B · SHA-256 `dfcfe29f24c188fd83139e9339299b15897e2d69200ff2ce6fc18dacc1a3022b`

~~~~tsx
/**
 * GELİŞİM-TAKİBİ (K-555-3) — "gözlem-takibi" (performans-iddiası DİLİ YOK, K-02/K-04):
 * öğrenci-bazlı H-c kayıt-zaman-çizelgesi (salt-okunur) + MOCK Katılım/Y-Eğim serisi (K-05).
 * İzleme ekranına gömülü çalışır.
 */
import { useEffect, useState } from 'react';
import { TrendingUp } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';
import { yanitSeri, noktalar } from '../../data/seriler';

const HC = 'scholaria_hc_kayitlar_v020';
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

export default function GelisimTakibi() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);
  useEffect(() => {
    try { setKayitlar(JSON.parse(localStorage.getItem(HC) ?? '[]') as HcKayit[]); } catch { setKayitlar([]); }
  }, []);
  const benim = kayitlar.filter((k) => k.ogrenci === ogrenci);
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="gelisim-takibi">
      <h3 className="font-bold text-sm flex items-center gap-2"><TrendingUp className="w-4 h-4 text-sky-600" /> Gelişim-takibi (gözlem-çizelgesi) — {o.takmaAd}</h3>
      <label className="text-xs font-semibold text-slate-700 mt-2 inline-block">
        Öğrenci:
        <select data-testid="takip-ogrenci-sec" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="ml-2 rounded-lg border border-slate-200 px-2 py-1 text-xs">
          {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
        </select>
      </label>
      <div className="mt-3 grid md:grid-cols-2 gap-4">
        <div>
          <div className="text-xs font-semibold text-slate-700">Katılım/Y-Eğim serisi (MOCK-gösterim)</div>
          <svg width="100%" height={56} viewBox="0 0 280 56" className="mt-1" data-testid="takip-seri">
            <polyline points={noktalar(yanitSeri(o.id), 280, 56)} fill="none" stroke="#0284c7" strokeWidth="2" />
          </svg>
          <div className="text-[11px] text-slate-500">Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04).</div>
        </div>
        <div>
          <div className="text-xs font-semibold text-slate-700">H-c gözlem-zaman-çizelgesi ({benim.length} kayıt)</div>
          {benim.length === 0 ? (
            <p className="text-xs text-slate-500 mt-1" data-testid="takip-bos">Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun.</p>
          ) : (
            <div className="mt-1 space-y-1">
              {benim.slice(0, 5).map((k) => (
                <div key={k.id} data-testid="takip-satiri" className="text-[11px] rounded-lg border border-slate-200 px-2 py-1">
                  {k.zaman?.slice(0, 10)} · {k.davranislar?.length ?? 0} davranış-gözlemi{k.not ? ` · "${k.not.slice(0, 30)}${k.not.length > 30 ? '…' : ''}"` : ''}
                </div>
              ))}
            </div>
          )}
        </div>
      </div>
    </div>
  );
}

~~~~

### `components/veli/VeliKoprusu.tsx`

7119 B · SHA-256 `7705f37fdfe90bc13caca02059de5299fd8dbccbfc9108917b7b3bac98a47c05`

~~~~tsx
/**
 * VELİ KÖPRÜSÜ (K-555-6/7): ① haftalık aile-bilgilendirme BÜLTENİ TASLAĞI (sınıf-geneli gözlem-dili +
 * genel-öneriler; aile-EĞİTİMİ içeriği SUPPORTA'dadır — buradan yönlendirilir) ② veli görüşme-RANDEVU
 * DEFTERİ (yerel; SMS/hatırlatma-otomasyonu YOK — K-334; MENTORIA-SMS ayrı-rol).
 */
import { useEffect, useState } from 'react';
import { CalendarClock, Home } from 'lucide-react';
import { SINIF_DURUMU } from '../../data/mock';

const RANDEVU = 'scholaria_veli_randevu_v023';
const HC = 'scholaria_hc_kayitlar_v020';
interface Randevu { id: string; tarih: string; saat: string; konu: string; not: string; durum: 'planlandı' | 'gerçekleşti' | 'ertelendi' }

const ONERILER = [
  'Eve dönüşte gün-içi bir gözlemi tek-cümleyle paylaşın ("bugün görevine kendi başladı").',
  'Ödevi tek-seferde değil, 10 dakikalık iki-bölüm olarak planlayın.',
  'Ekran-öncesi kısa nefes-rutini (4-4-4) birlikte deneyin.',
  'Talimatları tek-tek ve sırayla verin; tamamlanınca sözel takdir edin.',
  'Uyku ve oyun-düzeni gözlem-notlarını hafta-sonu karşılaştırın.',
];

function oku(): Randevu[] { try { return JSON.parse(localStorage.getItem(RANDEVU) ?? '[]') as Randevu[]; } catch { return []; } }

export default function VeliKoprusu() {
  const [sinif, setSinif] = useState('2A');
  const [bulten, setBulten] = useState<string | null>(null);
  const [randevular, setRandevular] = useState<Randevu[]>(() => oku());
  const [tarih, setTarih] = useState(new Date().toISOString().slice(0, 10));
  const [saat, setSaat] = useState('16:30');
  const [konu, setKonu] = useState('Haftalık gözlem paylaşımı');
  const [not, setNot] = useState('');

  useEffect(() => { try { localStorage.setItem(RANDEVU, JSON.stringify(randevular)); } catch { /* yerel-yalnız */ } }, [randevular]);

  function bultenUret() {
    const d = SINIF_DURUMU.find((x) => x.sinifId === sinif);
    let hc = 0; try { hc = (JSON.parse(localStorage.getItem(HC) ?? '[]') as unknown[]).length; } catch { hc = 0; }
    setBulten(
      `HAFTALIK SINIF BÜLTENİ — TASLAK (yerel-üretim; gönderilmez)\nSınıf: ${sinif} · Tarih: ${new Date().toISOString().slice(0, 10)}\n\n` +
      `Sınıf-gözlemi (MOCK): öğrenci ${d?.ogrenciler.length ?? 0} · ort. Y-Eğim ${(d?.ortalamaYorgunluk ?? 0).toFixed(2)} · son-alarm: ${d?.sonAlarm ?? '—'} · bu-hafta ${hc} gözlem-kartı (H-c).\n\n` +
      `Bu haftanın genel-önerileri (sınıf-geneli; kişi-değerlendirmesi yok — K-02):\n` +
      ONERILER.map((o, i) => `${i + 1}. ${o}`).join('\n') +
      `\n\nAile-EĞİTİMİ programı ve kişiye-özel içerik SUPPORTA ürünündedir; bu bülten yalnız bilgilendirme-notudur.`
    );
  }

  function randevuEkle() {
    const r: Randevu = { id: Math.random().toString(36).slice(2, 9), tarih, saat, konu, not, durum: 'planlandı' };
    setRandevular((p) => [r, ...p]); setNot('');
  }
  function durumDegistir(id: string) {
    setRandevular((p) => p.map((r) => r.id === id ? { ...r, durum: r.durum === 'planlandı' ? 'gerçekleşti' : r.durum === 'gerçekleşti' ? 'ertelendi' : 'planlandı' } : r));
  }

  return (
    <div className="space-y-4" data-testid="veli-koprusu">
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><Home className="w-4 h-4 text-indigo-600" /> Haftalık Aile Bülteni — TASLAK</h3>
        <div className="mt-2 flex flex-wrap gap-2 items-center text-xs">
          <select data-testid="bulten-sinif" value={sinif} onChange={(e) => setSinif(e.target.value)} className="rounded-lg border border-slate-200 px-2 py-1">
            {SINIF_DURUMU.map((s) => <option key={s.sinifId} value={s.sinifId}>{s.sinifId}</option>)}
          </select>
          <button type="button" data-testid="bulten-uret" onClick={bultenUret} className="px-3 py-1.5 rounded-xl bg-indigo-600 text-white font-semibold hover:bg-indigo-700">Bülten taslağı üret</button>
        </div>
        {bulten && <textarea readOnly rows={9} value={bulten} data-testid="bulten-taslagi" className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-xs font-mono" />}
        <p className="text-[11px] text-slate-500 mt-1">Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.</p>
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><CalendarClock className="w-4 h-4 text-indigo-600" /> Veli Görüşme — Randevu Defteri</h3>
        <div className="mt-2 grid md:grid-cols-4 gap-2 text-xs">
          <input type="date" data-testid="randevu-tarih" value={tarih} onChange={(e) => setTarih(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5" />
          <input type="time" data-testid="randevu-saat" value={saat} onChange={(e) => setSaat(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5" />
          <select data-testid="randevu-konu" value={konu} onChange={(e) => setKonu(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5">
            <option>Haftalık gözlem paylaşımı</option>
            <option>H-c kart-turu değerlendirme paylaşımı</option>
            <option>Gelişim-görüşmesi (gözlem-özetli)</option>
            <option>Diğer</option>
          </select>
          <input data-testid="randevu-not" value={not} onChange={(e) => setNot(e.target.value)} placeholder="görüşme-notu (isteğe bağlı)" className="rounded-lg border border-slate-300 px-2 py-1.5" />
        </div>
        <button type="button" data-testid="randevu-ekle" onClick={randevuEkle} className="mt-2 px-3 py-1.5 rounded-xl bg-indigo-600 text-white text-xs font-semibold hover:bg-indigo-700">Randevu kaydet</button>
        <div className="mt-3 space-y-1.5">
          {randevular.length === 0 ? (
            <p className="text-sm text-slate-500" data-testid="randevu-bos">Defter boş — randevu kaydedin.</p>
          ) : randevular.slice(0, 8).map((r) => (
            <div key={r.id} data-testid="randevu-satiri" className="flex items-center gap-2 text-xs rounded-xl border border-slate-200 px-3 py-2">
              <span className="font-semibold">{r.tarih} {r.saat}</span>
              <span className="text-slate-600">{r.konu}</span>
              {r.not && <span className="text-slate-400">· {r.not}</span>}
              <button type="button" onClick={() => durumDegistir(r.id)}
                className={`ml-auto px-2 py-0.5 rounded-full text-[10px] font-bold ${r.durum === 'planlandı' ? 'bg-amber-100 text-amber-700' : r.durum === 'gerçekleşti' ? 'bg-emerald-100 text-emerald-700' : 'bg-slate-100 text-slate-500'}`}>
                {r.durum}
              </button>
            </div>
          ))}
        </div>
        <p className="text-[11px] text-slate-500 mt-2">Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.</p>
      </div>
    </div>
  );
}

~~~~

### `data/kisitlar.ts`

478 B · SHA-256 `175dec40819eab373811da2152197ee2272e44947cbb013da21495e02b9e1cfa`

~~~~tsx
// LEXIVA Scholaria (K-700 ÖÖG uyarlama) — Kısıtlar (K-334 idari-mali dışarı, MEB salt okunur)

export const KISITLAR = {
  idariMaliKapsamDisi: true, // K-334: e-fatura/MEBBİS/BKDS yok
  mebEbaSaltOkunur: true, // K-331: ödevler ve içerik sadece çağrılır, yazılmaz
  kvkkYerelMaskeleme: true, // EBA UID'ler cihazda maskelenir, sunucuda açık metin yok
  telifiSifir: true, // Ölçekler/MEB müfredatı paket içinde yer almaz
  surum: 'v0.1.0',
} as const;

~~~~

### `data/mock.ts`

1646 B · SHA-256 `4c117c7929573cc5b030595ac27d19de6738660625ea7ddd065d45cbe1a99b8d`

~~~~tsx
// LEXIVA Scholaria (K-700 ÖÖG uyarlama) — Mock Veri (K-05 OGR-xxxx, gerçek veri yok)
import { Ogrenci, Sube, Gorev, SinifDurumu } from '../types';

export const SUBELER: Sube[] = [
  { id: 'SUB-2A', ad: '2. Sınıf A Şubesi', ogrenciSayisi: 24 },
  { id: 'SUB-2B', ad: '2. Sınıf B Şubesi', ogrenciSayisi: 22 },
  { id: 'SUB-4A', ad: '4. Sınıf A Şubesi', ogrenciSayisi: 25 },
];

export const GOREVLER: Gorev[] = [
  { id: 'PVC-101', baslik: 'Matematik: Sayı Blokları Eşleştirme', dersId: 'MAT-2', modul: 'M1' },
  { id: 'PVC-102', baslik: 'Hareket: Ritim ve Süre Tahmini', dersId: 'HKM-2', modul: 'M2' },
  { id: 'PVC-103', baslik: 'Türkçe: Hece Avcısı (Okuma)', dersId: 'TUR-2', modul: 'M3' },
];

export const OGRENCILER: Ogrenci[] = [
  { id: 'OGR-101', takmaAd: 'ARD-05', subeId: 'SUB-2A', katilim: 0.82, yorgunluk: 0.03, aktifGorev: 'PVC-101' },
  { id: 'OGR-102', takmaAd: 'ARD-06', subeId: 'SUB-2A', katilim: 0.75, yorgunluk: 0.05, aktifGorev: 'PVC-102' },
  { id: 'OGR-103', takmaAd: 'KRT-12', subeId: 'SUB-2B', katilim: 0.68, yorgunluk: 0.07, aktifGorev: 'PVC-103' },
  { id: 'OGR-104', takmaAd: 'SRY-22', subeId: 'SUB-4A', katilim: 0.81, yorgunluk: 0.04, aktifGorev: 'PVC-101' },
];

export const SINIF_DURUMU: SinifDurumu[] = [
  { sinifId: '2A', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-2A'), ortalamaYorgunluk: 0.04, sonAlarm: 'Yok' },
  { sinifId: '2B', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-2B'), ortalamaYorgunluk: 0.07, sonAlarm: 'Yorgunluk Uyarısı' },
  { sinifId: '4A', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-4A'), ortalamaYorgunluk: 0.04, sonAlarm: 'Yok' },
];

~~~~

### `data/mufredatYonerge.ts`

12979 B · SHA-256 `29449f8aa3a170fdc3ae6b179ff4717a16f3ad27d016da1c038a68c55935210f`

~~~~tsx
/**
 * MEB 2. SINIF KAZANIM-AĞACI + DERS-İŞLEME YÖNERGELERİ (K-555 · SCHOLARIA öğretmen-katmanı).
 * Hizalama: kod/ad kümesi disk-kuralına göre MUH-haritaları + MEB_K3-URETIM ile aynıdır
 * (MAT 25 + TR 37 = 62 — PERSONA cocukmoduVeri K3_LIST ile birebir).
 * Telif-çizgisi (K-08/YASA-M1-deseni): kazanım-ADLARI kılavuz-olgudur; YÖNERGELER VAMOLA-ÖZGÜN
 * kompozisyondur — MEB kitap/kılavuz cümlesi KOPYALANMAZ; bu liste resmî-kılavuz yerini TUTMAZ.
 * Dil (K-14): gözlemlenebilir-sayılabilir sınıf-eylemleri; ölçme/evaluation-yargısı yok (K-02).
 */
export interface MufredatKayit { kod: string; ad: string; ders: 'MAT' | 'TR'; yonerge: string }

export const MUFREDAT_2: MufredatKayit[] = [
  // ── MATEMATİK-2 (25) ──
  { kod: 'MAT.2.1.1', ad: 'Sayı postası: oku-yaz-eşle', ders: 'MAT', yonerge: 'Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.' },
  { kod: 'MAT.2.1.2', ad: 'Onluk-birlik çantası', ders: 'MAT', yonerge: 'Nesneleri 10\'luk torbalara koydurarak onluk-birlik ayrımını somutlaştırın; tahtadaki tabloya birlikte işleyin.' },
  { kod: 'MAT.2.1.3', ad: 'Sayı doğrusu düellosu', ders: 'MAT', yonerge: 'Yer-matında sayı doğrusu çizip komşu-sayılar arasında yürüyerek yer-değiştirme oyunu oynatın.' },
  { kod: 'MAT.2.1.4', ad: 'Yüzlük tablo zıplaş', ders: 'MAT', yonerge: 'Yüzlük tabloda 1\'er ve 10\'ar atlamaları renkli-kalemle boyattırın; kuralı öğrenciye sözlü teyit ettirin.' },
  { kod: 'MAT.2.1.5', ad: 'Örüntü treni: kural-kur-devam-et', ders: 'MAT', yonerge: 'Şekil/sayı-kartlarıyla 2\'şer-5\'er-10\'ar örüntüler kurdurtun; kuralı sözlutturup sıradaki-halkayı tahmin ettirin.' },
  { kod: 'MAT.2.1.6', ad: 'Tahmin kavanozu: grupla-tahmin et', ders: 'MAT', yonerge: 'Kavanozdaki nesneleri önce 10\'luk gruplatıp tahmin yazdırın; sonra saydırarak tahmini doğrulatın.' },
  { kod: 'MAT.2.1.7', ad: 'Bütün-yarım-çeyrek pizza', ders: 'MAT', yonerge: 'Kâğıt-daireleri katlatıp keserek yarım/çeyrek/bütün ilişkisini yapıştırma-panosunda kurun.' },
  { kod: 'MAT.2.1.8', ad: 'Kasaba para turu', ders: 'MAT', yonerge: 'Sınıf-mağazası dramatizasyonu kurun; TL-banknot kopyalarıyla alışveriş yaptırıp harcama-çizelgesi doldurtun.' },
  { kod: 'MAT.2.1.9', ad: 'Tam saat, yarım saat: saat-avcısı', ders: 'MAT', yonerge: 'Kart-saatlerle tam/yarım-saat ayırımı yaptırın; gün-içi rutini saat-bilgisiyle eşleştirme-turu kurun.' },
  { kod: 'MAT.2.1.10', ad: 'Karış mı, cetvel mi?', ders: 'MAT', yonerge: 'Aynı uzunluğu karış, adım ve cetvel ile ölçtürüp sonuçları karşılaştırın; standart-ölçü gereğini tartıştırın.' },
  { kod: 'MAT.2.1.11', ad: 'Tahmin çubuğu: ölç-karşılaştır', ders: 'MAT', yonerge: 'Uzunlukları önce tahmin ettirip yazdırın; sonra cetveliyle ölçtürüp tahmin-ölçü tablosunu doldurtun.' },
  { kod: 'MAT.2.2.1', ad: 'Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme', ders: 'MAT', yonerge: 'Sınıf-içi senaryolardan toplama-çıkarma problemleri kurdurtun; çözümü tek-cümleyle anlattırın.' },
  { kod: 'MAT.2.2.2', ad: 'Tahmin et, zihinden işle, tutarlılığı açıkla', ders: 'MAT', yonerge: 'İşlemi önce zihinden-tahmin ettirin; sonra yazıyla doğrulatıp tahminle-sonucu karşılaştırıp açıklattırın.' },
  { kod: 'MAT.2.2.3', ad: 'Toplama-çıkarma ters-ilişkisi', ders: 'MAT', yonerge: 'Toplamadan çıkarma ürettirtin (a+b=c → c−b=a); boşluklu-kartlarla eşleştirme-oyunuyla pekiştirin.' },
  { kod: 'MAT.2.2.4', ad: 'Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma', ders: 'MAT', yonerge: 'Eş-öbek dizilimleri kurdurtun; toplamanın-kısa-yolu olarak çarpma yazdırın (2+2+2 = 3×2).' },
  { kod: 'MAT.2.2.5', ad: 'Çarpan ve çarpım: bileşenler', ders: 'MAT', yonerge: '3×4 gibi işlemlerde parça-adlarını öğretin (çarpan-çarpan-çarpım); geriden-seçme oyunu oynatın.' },
  { kod: 'MAT.2.2.6', ad: 'Eşitliğin anlamları: denge', ders: 'MAT', yonerge: 'Terazi-deseninde boşluğa sayı yazdırarak eşitliği kurdurtun (5+3=□+2); dengeyi cümleyle açıklatın.' },
  { kod: 'MAT.2.3.1', ad: 'Geometri ayırma bandı', ders: 'MAT', yonerge: 'Şekil-kartlarını kenar ve köşe-özelliklerine göre sınıflandırma-bandına yerleştirtin; ayrımı sözlü gerekçelendirin.' },
  { kod: 'MAT.2.3.2', ad: 'Küp kule inşaatı', ders: 'MAT', yonerge: 'Küp-kule inşa ettirin; küp-sayısını önce-tahmin sonra-saydırarak karşılaştırma-satırı yazdırın.' },
  { kod: 'MAT.2.3.3', ad: 'Şekil mozaik atölyesi', ders: 'MAT', yonerge: 'Kare/üçgen mozaiklerle yeni-şekiller oluşturtun; hangi-şekillerden oluştuğunu anlattırın.' },
  { kod: 'MAT.2.3.4', ad: 'Döndür-karşılaştır: aynı mı, farklı mı?', ders: 'MAT', yonerge: 'Kesik-şekilleri döndürüp aynı/farklı ayırımı yaptırın; döndürünce adın-değişmediğini tartıştırın.' },
  { kod: 'MAT.2.3.5', ad: 'Bardak sorusu: tahmin-ölç', ders: 'MAT', yonerge: 'Aynı sıvıyı ince/geniş bardaklara döktürüp miktarın-değişmediğini gözlemletin (korunum-yargısı kurdurmadan).' },
  { kod: 'MAT.2.3.6', ad: 'Hedefe yol: planla-izle-analiz', ders: 'MAT', yonerge: 'Sınıf-planında A→B arası yolları çizdirtin; en-kısayı seçtirtin ve adım-adım plan-izle-analiz turu yapın.' },
  { kod: 'MAT.2.3.7', ad: 'Ayna avcısı', ders: 'MAT', yonerge: 'Harf ve şekil-kartlarını aynaya tutturtup simetrikleri avlattırın; simetri-çizgisini kendilerine bozdurtun.' },
  { kod: 'MAT.2.4.1', ad: 'İki grup, bir grafik', ders: 'MAT', yonerge: 'Basit sınıf-anketi yapılıp sonuçları resimli-grafiğe işlettirin; "kaç-fazla/kaç-az" soruları sordurtun.' },
  // ── TÜRKÇE-2 (37) ──
  { kod: 'T.D.1.1', ad: 'Dinleme/izlemeyi yönetebilme', ders: 'TR', yonerge: 'Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün.' },
  { kod: 'T.D.1.2', ad: 'Dinlediklerinden anlam kurma: ana-fikir avcısı', ders: 'TR', yonerge: 'Kısa-hikâye dinlettirin; ana-fikri tek-cümleyle tahmin ettirip sınıfça tartışın.' },
  { kod: 'T.D.1.3', ad: 'Dinlediklerini/izlediklerini çözümleyebilme', ders: 'TR', yonerge: 'Sebep-sonuç içeren masal dinlettirin; "neden-bekledi?" sorularıyla çözümleme-tartışması kurun.' },
  { kod: 'T.D.1.4', ad: 'Dinleme/izleme sürecini değerlendirebilme', ders: 'TR', yonerge: 'Dinleme-sonu "ne-anladım" paylaşım-çemberi yaptırın; kendi-dinlemesine bakan cümle kurdurtun.' },
  { kod: 'T.D.2.1', ad: 'Dinleme/izlemeyi yönetebilme (2)', ders: 'TR', yonerge: 'Haber/duyuru dinlettin; kim-ne-zaman ipuçlarını dinlerken resimli-not aldırtın.' },
  { kod: 'T.D.2.2', ad: 'Dinledikleri/izledikleri ile ilgili anlam oluşturabilme', ders: 'TR', yonerge: 'Kurallar-metni dinlettirip dinlediklerinden tek-cümlelik anlam-özeti ürettirin.' },
  { kod: 'T.D.2.3', ad: 'Dinlediklerini/izlediklerini çözümleyebilme (2)', ders: 'TR', yonerge: 'Sıralı-olay anlatımı dinlettin; önce/sonra kartlarını doğru-sıraya dizdirtin.' },
  { kod: 'T.D.2.4', ad: 'Dinleme/izleme sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Gürültülü ve sessiz ortamda kısa-dinleme karşılaştırması yaptırın; farkı birlikte tartıştırın.' },
  { kod: 'T.D.2.5', ad: 'Dinleme/izleme sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Dinlediği-hikâyeyi özetlettirin; güçlü-dinleme belirtilerini birlikte listelettirin.' },
  { kod: 'T.K.1.1', ad: 'Konuşmalarını yönetebilme', ders: 'TR', yonerge: 'Toplantı-çemberinde söz-sırası kuralıyla kısa-konuşmalar yaptırın; el-kaldırma rutinini pekiştirin.' },
  { kod: 'T.K.1.2', ad: 'Konuşmalarında içerik oluşturabilme', ders: 'TR', yonerge: 'Kim/zaman/yer/olay ipuçlarını içeren olay-anlatımı görevi verin; ipuçlarını kullanma-adımını gözlemleyin.' },
  { kod: 'T.K.1.3', ad: 'Konuşma kurallarını uygulayabilme', ders: 'TR', yonerge: 'Göz-teması ve ses-şiddeti hedefleriyle rol-oyunu konuşmaları kurdurun.' },
  { kod: 'T.K.1.4', ad: 'Konuşma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Konuşma-sonu "anlatabildim-mi" öz-tartışma çemberi yaptırın.' },
  { kod: 'T.K.2.1', ad: 'Konuşmalarını yönetebilme (2)', ders: 'TR', yonerge: 'Sınıf-tartışmasında sıra-alma kartları kullanın; dinle-söyle rutini kurun.' },
  { kod: 'T.K.2.2', ad: 'Konuşmalarında içerik oluşturabilme (2)', ders: 'TR', yonerge: 'Gezi/gün-anlatısında önce-sonra-en-son bağlaçlarını kullanma-hedefi verin.' },
  { kod: 'T.K.2.3', ad: 'Konuşma kurallarını uygulayabilme (2)', ders: 'TR', yonerge: 'Telefon-dramatizasyonu kurdurtun; selam-amaç-kapanış üçlüsünü denettirin.' },
  { kod: 'T.K.2.4', ad: 'Konuşma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Ortam-seçiminin anlaşılırlığa etkisini oyunla gözlemletip tartıştırın.' },
  { kod: 'T.K.2.5', ad: 'Konuşma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Konuşma-sonu iki-güçlü-yön bir-gelişim-alanı paylaşımı yaptırın.' },
  { kod: 'T.O.1.1', ad: 'Okuma sürecini yönetebilme', ders: 'TR', yonerge: 'Sessiz-okuma rutini kurun; satır-takip kartıyla odaklanma davranışını gözlem-notuyla izleyin.' },
  { kod: 'T.O.1.2', ad: 'Okuduklarından anlam kurma', ders: 'TR', yonerge: 'Kısa-metin okutturup yanıtı metinde-bulunur sorular sorun; işaretlettirin.' },
  { kod: 'T.O.1.3', ad: 'Okuduklarını çözümleyebilme', ders: 'TR', yonerge: 'Karakter/yer-bilgisi isteyen çözümleme-sorularıyla metin-tartışması kurun.' },
  { kod: 'T.O.1.4', ad: 'Okuma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Okuma-ortamını birlikte düzenlettirin; gürültünün anlamaya-etkisini gözlemletin.' },
  { kod: 'T.O.1.5', ad: 'Okuma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Okuduğunu-yeniden-anlatma çifti kurun; kendi-anlamasını kontrol-cümlesiyle bağdattırın.' },
  { kod: 'T.O.2.1', ad: 'Okuma sürecini yönetebilme (2)', ders: 'TR', yonerge: 'Satır-takip kartı kullanımını modelleyip her-okurda uygulattırın.' },
  { kod: 'T.O.2.2', ad: 'Okudukları ile ilgili anlam oluşturabilme', ders: 'TR', yonerge: 'Yanıtı metinde-olan sorular sorun; buldukları-satırı gösterdirtin.' },
  { kod: 'T.O.2.3', ad: 'Okuduklarını çözümleyebilme (2)', ders: 'TR', yonerge: 'İleti-bulma sorusuyla kısa-hikâye tartışması yaptırın ("bu-hikâye ne-öğretti?").' },
  { kod: 'T.O.2.4', ad: 'Okuma sürecine etki eden durumları gözden geçirebilme (2)', ders: 'TR', yonerge: 'Bilinmeyen-kelime sözlük-köşesi kurun; bakma-adımını modelleyip uygulattın.' },
  { kod: 'T.O.2.5', ad: 'Okuma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Hikâye-özetini kendi-kelimeleriyle anlattırın; anlamasını gözden-geçirtin.' },
  { kod: 'T.Y.1.1', ad: 'Yazılı anlatım becerilerini yönetebilme', ders: 'TR', yonerge: 'Oturuş ve kalem-tutuş kontrol-listesiyle yazma-hazırlığı yaptırın; listeyi öğrenciyle birlikte doldurun.' },
  { kod: 'T.Y.1.2', ad: 'Yazılarında içerik oluşturma', ders: 'TR', yonerge: 'Gün-içi olayı üç-cümleyle yazdirtin; önce-sonra kelimelerini kullanma-hedefi verin.' },
  { kod: 'T.Y.1.3', ad: 'Yazma kurallarını uygulayabilme', ders: 'TR', yonerge: 'Cümle-başı büyük-harf ve nokta-avcılığı yaptırın; yazısını kendine-tarattırın.' },
  { kod: 'T.Y.1.4', ad: 'Yazma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Yazıyı sesli-okuyarak-kontrol rutini kurup arkadaşa-okutma turu yapın.' },
  { kod: 'T.Y.2.1', ad: 'Yazılı anlatım becerilerini yönetebilme (2)', ders: 'TR', yonerge: 'Yazma-öncesi üç-kelimelik mini-plan yaptırıp taslağa geçirtin.' },
  { kod: 'T.Y.2.2', ad: 'Yazılarında içerik oluşturabilme (2)', ders: 'TR', yonerge: 'Tarih-hitap-ileti-imza şablonuyla sınıf-içi mektup yazdirtin.' },
  { kod: 'T.Y.2.3', ad: 'Yazma kurallarını uygulayabilme (2)', ders: 'TR', yonerge: 'Noktalama-kartlarıyla cümle-düzeltme yarışı kurun.' },
  { kod: 'T.Y.2.4', ad: 'Yazma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Kalem-tutuşu düzeltme egzersizlerini kısa-turlarla yaptırın; yorgunluk-belirtisini gözlemleyin.' },
  { kod: 'T.Y.2.5', ad: 'Yazma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Yazım-noktalama-anlam üçlü-kontrol listesini birlikte doldurtun.' },
];

export const MUFREDAT_SINIF = '2. sınıf';
export const MUFREDAT_KAYNAK_NOTU =
  'Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).';

~~~~

### `data/seriler.ts`

1194 B · SHA-256 `f9c9de9146e481c3d686ae059fc75da1bb266098e35b95096dcf2ec6323698bf`

~~~~tsx
// LEXIVA Scholaria (K-700 ÖÖG uyarlama) — Deterministik sentetik seriler (K-05 MOCK · K-554).
// Seed'li sin-dalga: her-açılışta-aynı; gerçek sensör-akışı DEĞİLDİR — yalnız gösterim-verisi (K-02).
export function seri(seed: number, n = 12, baz = 0.4, genlik = 0.14): number[] {
  return Array.from({ length: n }, (_, i) =>
    Math.round((baz + genlik * Math.sin(seed * 1.7 + i * 0.9) + (i / n) * 0.05) * 1000) / 1000
  );
}

export function ritimSeri(sinifId: string): number[] {  // sınıf ritim eğrisi (sentetik)
  const seed = sinifId.split('').reduce((a, c) => a + c.charCodeAt(0), 0);
  return seri(seed, 12, 0.38, 0.12);
}

export function yanitSeri(id: string): number[] {  // yanıt zamanı eğimi serisi (deterministik sentetik)
  const seed = parseInt(id.replace(/\D/g, ''), 10) || 7;
  return seri(seed, 12, 0.05, 0.035);
}

/** Seriyi SVG-polyline 'x,y' noktalarına çevirir. */
export function noktalar(vals: number[], w = 240, h = 48): string {
  const min = Math.min(...vals);
  const max = Math.max(...vals);
  const ar = max - min || 1;
  return vals.map((v, i) => `${(i / (vals.length - 1)) * w},${h - ((v - min) / ar) * (h - 6) - 3}`).join(' ');
}

~~~~

### `main.tsx`

236 B · SHA-256 `14a10dee4aaa2130d9f57c136db7f16f95f524d60d77146b17776e91c2ab626c`

~~~~tsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';
import './index.css';

ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);

~~~~

### `types/index.ts`

701 B · SHA-256 `aab7c4b22938dd7afa971f4daa98560035b052902328f63ababefcd2697a255f`

~~~~tsx
// LEXIVA Scholaria (K-700 ÖÖG uyarlama) — Tipler
export interface Ogrenci {
  id: string;
  takmaAd: string;
  subeId: string;
  katilim: number;   // görev katılım endeksi (0-1; sentetik)
  yorgunluk: number; // yorgunluk eğimi (0-0.1; sentetik)
  aktifGorev: string;
}

export interface Sube {
  id: string;
  ad: string;
  ogrenciSayisi: number;
}

export interface Gorev {
  id: string;
  baslik: string;
  dersId: string;
  modul: string;
}

export interface EBAAuth {
  accessToken: string;
  refreshToken: string;
  expiresIn: number;
  maskedUid: string;
}

export interface SinifDurumu {
  sinifId: string;
  ogrenciler: Ogrenci[];
  ortalamaYorgunluk: number;
  sonAlarm: string;
}

~~~~

### `types/surum.d.ts`

99 B · SHA-256 `c7816811300c1ea2de941d4302b67a45099395f33cd75e58c144efd668f4a381`

~~~~tsx
declare const __SURUM__: string;
declare const __TAM__: boolean;
declare const __PILOT__: boolean;

~~~~

# Ek C-SED — SCHOLARIA-SED bağımsız kanıt paketi

## C-SED-1 — 25 DOM durumu

Tarayıcı tarihi/saatleri test anını gösterir. ÖĞR/ARD ve benzeri kodlar üründeki sentetik örneklerdir; test notu gerçek öğrenciye ait değildir.

### SCH-SED-DOM-nav-pano

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf Özeti (Shared Evidence Akışı)

Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır.

2A Sınıfı
Yok
Öğr. Sayı: 2 · Ort. Fslope: 0.04
Gün-içi nabzı aç →
2B Sınıfı
Yorulma Uyarısı
Öğr. Sayı: 1 · Ort. Fslope: 0.07
Gün-içi nabzı aç →
4A Sınıfı
Yok
Öğr. Sayı: 1 · Ort. Fslope: 0.04
Gün-içi nabzı aç →

MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde.
~~~~

### SCH-SED-DOM-nav-sinif

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf (Dinamik Gating: G_contrast)

Ders esnasında sınıf içi gürültü/dikkat dengesi. Seçili sınıfın göstergeleri:

Hedef Sınıf:
SUB-2A
SUB-2B
SUB-4A
Aktif Parametre: Dynamic Gating Slope (Avg. G_contrast) — 0.31 · 2A · Öğrenci 2 · Ort. Fslope 0.04 [PRD §3.A deseninden MOCK]
G_contrast gün-içi eğrisi (sentetik-gösterim)
ARD-05
GFI 0.82 · Fslope 0.03 · görev PVC-101
ARD-06
GFI 0.75 · Fslope 0.05 · görev PVC-102
~~~~

### SCH-SED-DOM-nav-ogrenci

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğrenci (Cihaz & Olay Dinleyicileri)

Öğrenci Terminal UI. EventListener kilitleri (PRD §3.B) dürtüsel hataları engeller — mini-simülasyonda deneyin.

Görsel Dikkat: Renk Eşleştirme
MAT-2 | M1
Motivasyon: Zaman Farkındalığı
HKM-2 | M2
Bölünmüş Dikkat: Çift Görev
TUR-2 | M3
~~~~

### SCH-SED-DOM-nav-ogretmen

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Fslope ≥ 0.07 → Nefes Halkası.
Toplu Yorgunluk (Fslope) — 2A
ARD-05
Fslope 0.03
GFI 0.82
ARD-06
Fslope 0.05
GFI 0.75
d(SDRT)/dt sınıf-eğrisi (sentetik-gösterim)
Nefes Halkası (Breathing Circle)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
YZ Önerisi İste
~~~~

### SCH-SED-DOM-nav-transfer

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Transfer Gözlem Kartı

Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.

Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).

MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
Öğrenci (sentetik):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Gözlenen etkinlik:
Görsel Dikkat: Renk Eşleştirme
Motivasyon: Zaman Farkındalığı
Bölünmüş Dikkat: Çift Görev
Gözlenen davranışlar (işaretleyerek):
○ Göreve kendi başladı (yönlendirme olmadan)○ Zorlanınca ipucu istedi ve sürdürdü○ Mola verdi ve döndü (akışı korudu)○ Sözel yönerge tek başına yeterli oldu
Kısa not (isteğe bağlı):
Kaydet (yerel)
0 kayıt · yalnız bu tarayıcıda
~~~~

### SCH-SED-DOM-nav-ders

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Görsel Dikkat: Renk Eşleştirme
Motivasyon: Zaman Farkındalığı
Bölünmüş Dikkat: Çift Görev
Ders-işleme yönergesi (MAT.2.1.1): Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (0)

Defter boş — yukarıdan atama işleyin.

Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-SED-DOM-nav-veli

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Aile Bilgilendirme

Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.

Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).

Haftalık Aile Bülteni — TASLAK
2A
2B
4A
Bülten taslağı üret

Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.

Veli Görüşme — Randevu Defteri
Haftalık gözlem paylaşımı
H-c kart-turu değerlendirme paylaşımı
Gelişim-görüşmesi (gözlem-özetli)
Diğer
Randevu kaydet

Defter boş — randevu kaydedin.

Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.
~~~~

### SCH-SED-DOM-nav-bep

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
BEP Hazırlık

Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.

Sınır-şerhi: Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
Hedef-şablonu üretimi
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Hedef-şablonunu deftere ekle

Defter boş — yukarıdan hedef-şablonu üretin.
~~~~

### SCH-SED-DOM-nav-eba

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
MEB EBA Entegrasyonu

Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.

Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:

1 · Cihaz (Terminal)
EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
2 · daily-insight TASLAĞI
Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
3 · [EBA POST] /api/v1/report/daily-insight
PLANLI ENTEGRASYON — bu önizlemede gönderim YOK
K-331: salt-okunur çağrı — ödev/içerik yazılmaz
e-sınav girişi YOK
K-334: idari-mali otomasyon dışarı
Başarı Notu Yazılmaz · Maskeli UID
Insight Taslağı Üret (yerel)

OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
~~~~

### SCH-SED-DOM-nav-izleme

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Gelişim Takibi

Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin.

MOCK: seriler sentetik-gösterimdir (K-05); XR/Control-Task Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
d(SDRT)/dt — ARD-05 (12 gözlem-noktası)
Gaze-Lock etkileşim-oranı: %88.4 (sentetik-sabit · Faz-3 Control Task-M11)
Aktif görev: PVC-101 · GFI: 0.82 · Fslope: 0.03
K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.
Gelişim-takibi (gözlem-çizelgesi) — ARD-05
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
GFI/Fslope serisi (MOCK-gösterim)
Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04).
H-c gözlem-zaman-çizelgesi (0 kayıt)

Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun.
~~~~

### SCH-SED-DOM-nav-ses

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sınıf İçi Ses Yönetimi

Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın.

PLANLI-KATMAN şerhi: donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü ayrımının görsel-simülasyonu vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik).
Ana Sinyal İzolasyonu — 60%
ana-sinyal
ortam-gürültüsü (izolasyon-arttıkça söner)
Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır)
~~~~

### SCH-SED-DOM-nav-rapor

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

### SCH-SED-DOM-nav-ayarlar

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ayarlar

Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır.

2. Sınıf A Şubesi (24 slot)
2. Sınıf B Şubesi (22 slot)
4. Sınıf A Şubesi (25 slot)

MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda.
~~~~

### SCH-SED-DOM-nav-yardim

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Sistem Kılavuzu ve Terimler

Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu.

K-05: Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır.
K-02: Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil.
K-331: MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok.
K-334: Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok).
K-05/MOCK: ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez.
MOCK-değerleri: {"idariMaliKapsamDisi":true,"mebEbaSaltOkunur":true,"kvkkYerelMaskeleme":true,"telifiSifir":true,"surum":"v0.1.0"}
~~~~

### SCH-SED-DOM-ogrenci-gorev-detay

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğrenci (Cihaz & Olay Dinleyicileri)

Öğrenci Terminal UI. EventListener kilitleri (PRD §3.B) dürtüsel hataları engeller — mini-simülasyonda deneyin.

Görsel Dikkat: Renk Eşleştirme
MAT-2 | M1
Motivasyon: Zaman Farkındalığı
HKM-2 | M2
Bölünmüş Dikkat: Çift Görev
TUR-2 | M3
Görsel Dikkat: Renk Eşleştirme — Terminal önizlemesi (MOCK)

Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): dürtüsel-tık engellenir.

Göreve Başla (kilit-demosu)Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir.
~~~~

### SCH-SED-DOM-transfer-kayitli

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Transfer Gözlem Kartı

Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.

Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).

MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
Öğrenci (sentetik):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Gözlenen etkinlik:
Görsel Dikkat: Renk Eşleştirme
Motivasyon: Zaman Farkındalığı
Bölünmüş Dikkat: Çift Görev
Gözlenen davranışlar (işaretleyerek):
○ Göreve kendi başladı (yönlendirme olmadan)○ Zorlanınca ipucu istedi ve sürdürdü○ Mola verdi ve döndü (akışı korudu)○ Sözel yönerge tek başına yeterli oldu
Kısa not (isteğe bağlı):
Kaydet (yerel)
1 kayıt · yalnız bu tarayıcıda
Son kayıtlar:
hepsini temizle
ARD-05 · Görsel Dikkat: Renk Eşleştirme · 1 davranış · “SENTETIK BRIEF TESTI — gerçek öğrenci değildir.” (10.09.2026 23:27:41)
~~~~

### SCH-SED-DOM-rapor-kayitli

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

### SCH-SED-DOM-eba-taslak

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
MEB EBA Entegrasyonu

Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.

Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:

1 · Cihaz (Terminal)
EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
2 · daily-insight TASLAĞI
Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
3 · [EBA POST] /api/v1/report/daily-insight
PLANLI ENTEGRASYON — bu önizlemede gönderim YOK
K-331: salt-okunur çağrı — ödev/içerik yazılmaz
e-sınav girişi YOK
K-334: idari-mali otomasyon dışarı
Başarı Notu Yazılmaz · Maskeli UID
Insight Taslağı Üret (yerel)

OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
~~~~

Alan `eba-taslagi` · readOnly=True

~~~~text
GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez)
Tarih: 2026-09-10 · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02)

• ••• (maske-UID ÖĞR-•••) — görev: 1 davranış-gözlemi; ör. "Göreve kendi başladı (yönlendirme olmadan)" (gözlemlenebilir-sayılabilir dil).

[Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA'ya yazma-yok]
~~~~

### SCH-SED-DOM-veli-kayitli

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Aile Bilgilendirme

Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.

Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).

Haftalık Aile Bülteni — TASLAK
2A
2B
4A
Bülten taslağı üret

Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.

Veli Görüşme — Randevu Defteri
Haftalık gözlem paylaşımı
H-c kart-turu değerlendirme paylaşımı
Gelişim-görüşmesi (gözlem-özetli)
Diğer
Randevu kaydet

Defter boş — randevu kaydedin.

Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.
~~~~

### SCH-SED-DOM-yz-oneri

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Fslope ≥ 0.07 → Nefes Halkası.
Toplu Yorgunluk (Fslope) — 2A
ARD-05
Fslope 0.03
GFI 0.82
ARD-06
Fslope 0.05
GFI 0.75
d(SDRT)/dt sınıf-eğrisi (sentetik-gösterim)
Nefes Halkası (Breathing Circle)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı)

Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin.

Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.
İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma.
Nefes Halkası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.
Yer-seçimi: dikkat-dağınıklığı-anında öne-yakın sessiz-masa önerin.
Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin.
✓ Onayla ve Yürürlüğe Al
✕ Reddet ve Gerekçelendir
~~~~

Alan `oneri-notu` · readOnly=True

~~~~text
EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · ARD-05 · 2A):
• Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.
• Nefes Halkası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.

⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer.
~~~~

### SCH-SED-DOM-yz-reddet

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Öğretmen Paneli (Teacher Cockpit)
MOCK: tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için yönlendirme-desteğidir (K-02) · eşik-önerisi: Fslope ≥ 0.07 → Nefes Halkası.
Toplu Yorgunluk (Fslope) — 2A
ARD-05
Fslope 0.03
GFI 0.82
ARD-06
Fslope 0.05
GFI 0.75
d(SDRT)/dt sınıf-eğrisi (sentetik-gösterim)
Nefes Halkası (Breathing Circle)
Kılavuz-tempo: 4 sn al — 4 sn tut — 4 sn ver · sınıf-öncesi/arası 2 tur.
Eşik-üstü öğrenci yok.
Yönlendirme-kartı üret
Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri

YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.

Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)

YZ Önerisi Öğretmen Tarafından Reddedildi

Kaydet
~~~~

### SCH-SED-DOM-bep-taslak-probe

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
BEP Hazırlık

Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.

Sınır-şerhi: Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
Hedef-şablonu üretimi
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Hedef-şablonunu deftere ekle
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
sil
Haftalık gözlem-probu izgarası (1/4):
H1 · 2026-09-10 · yok
+ haftalık-probe ekle

İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14).
~~~~

Alan `bep-sablon-metin` · readOnly=True

~~~~text
GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir)
Öğrenci: ARD-05 (maske-ÖĞR) · Kazanım: MAT.2.1.1 — Sayı postası: oku-yaz-eşle

Hedef-cümlesi (gözlemlenebilir-dil, K-14): ARD-05, sayı postası: oku-yaz-eşle kazanımına bağlı sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.

İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara.
Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır.
~~~~

### SCH-SED-DOM-ders-atamali

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
MAT.2.1.1 — Sayı postası: oku-yaz-eşle
MAT.2.1.2 — Onluk-birlik çantası
MAT.2.1.3 — Sayı doğrusu düellosu
MAT.2.1.4 — Yüzlük tablo zıplaş
MAT.2.1.5 — Örüntü treni: kural-kur-devam-et
MAT.2.1.6 — Tahmin kavanozu: grupla-tahmin et
MAT.2.1.7 — Bütün-yarım-çeyrek pizza
MAT.2.1.8 — Kasaba para turu
MAT.2.1.9 — Tam saat, yarım saat: saat-avcısı
MAT.2.1.10 — Karış mı, cetvel mi?
MAT.2.1.11 — Tahmin çubuğu: ölç-karşılaştır
MAT.2.2.1 — Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme
MAT.2.2.2 — Tahmin et, zihinden işle, tutarlılığı açıkla
MAT.2.2.3 — Toplama-çıkarma ters-ilişkisi
MAT.2.2.4 — Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma
MAT.2.2.5 — Çarpan ve çarpım: bileşenler
MAT.2.2.6 — Eşitliğin anlamları: denge
MAT.2.3.1 — Geometri ayırma bandı
MAT.2.3.2 — Küp kule inşaatı
MAT.2.3.3 — Şekil mozaik atölyesi
MAT.2.3.4 — Döndür-karşılaştır: aynı mı, farklı mı?
MAT.2.3.5 — Bardak sorusu: tahmin-ölç
MAT.2.3.6 — Hedefe yol: planla-izle-analiz
MAT.2.3.7 — Ayna avcısı
MAT.2.4.1 — İki grup, bir grafik
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Görsel Dikkat: Renk Eşleştirme
Motivasyon: Zaman Farkındalığı
Bölünmüş Dikkat: Çift Görev
Ders-işleme yönergesi (MAT.2.1.1): Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (1)
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
Görsel Dikkat: Renk Eşleştirme · 2026-09-10
sil
Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-SED-DOM-ders-turkce

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Ders & Görev

2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).

2. sınıf kazanım-ağacı · 62 kazanım (Matematik 25 + Türkçe 37). Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).
Ders:
Matematik (25)
Türkçe (37)
Kazanım:
T.D.1.1 — Dinleme/izlemeyi yönetebilme
T.D.1.2 — Dinlediklerinden anlam kurma: ana-fikir avcısı
T.D.1.3 — Dinlediklerini/izlediklerini çözümleyebilme
T.D.1.4 — Dinleme/izleme sürecini değerlendirebilme
T.D.2.1 — Dinleme/izlemeyi yönetebilme (2)
T.D.2.2 — Dinledikleri/izledikleri ile ilgili anlam oluşturabilme
T.D.2.3 — Dinlediklerini/izlediklerini çözümleyebilme (2)
T.D.2.4 — Dinleme/izleme sürecine etki eden durumları gözden geçirebilme
T.D.2.5 — Dinleme/izleme sürecini değerlendirebilme (2)
T.K.1.1 — Konuşmalarını yönetebilme
T.K.1.2 — Konuşmalarında içerik oluşturabilme
T.K.1.3 — Konuşma kurallarını uygulayabilme
T.K.1.4 — Konuşma sürecini değerlendirebilme
T.K.2.1 — Konuşmalarını yönetebilme (2)
T.K.2.2 — Konuşmalarında içerik oluşturabilme (2)
T.K.2.3 — Konuşma kurallarını uygulayabilme (2)
T.K.2.4 — Konuşma sürecine etki eden durumları gözden geçirebilme
T.K.2.5 — Konuşma sürecini değerlendirebilme (2)
T.O.1.1 — Okuma sürecini yönetebilme
T.O.1.2 — Okuduklarından anlam kurma
T.O.1.3 — Okuduklarını çözümleyebilme
T.O.1.4 — Okuma sürecine etki eden durumları gözden geçirebilme
T.O.1.5 — Okuma sürecini değerlendirebilme
T.O.2.1 — Okuma sürecini yönetebilme (2)
T.O.2.2 — Okudukları ile ilgili anlam oluşturabilme
T.O.2.3 — Okuduklarını çözümleyebilme (2)
T.O.2.4 — Okuma sürecine etki eden durumları gözden geçirebilme (2)
T.O.2.5 — Okuma sürecini değerlendirebilme (2)
T.Y.1.1 — Yazılı anlatım becerilerini yönetebilme
T.Y.1.2 — Yazılarında içerik oluşturma
T.Y.1.3 — Yazma kurallarını uygulayabilme
T.Y.1.4 — Yazma sürecini değerlendirebilme
T.Y.2.1 — Yazılı anlatım becerilerini yönetebilme (2)
T.Y.2.2 — Yazılarında içerik oluşturabilme (2)
T.Y.2.3 — Yazma kurallarını uygulayabilme (2)
T.Y.2.4 — Yazma sürecine etki eden durumları gözden geçirebilme
T.Y.2.5 — Yazma sürecini değerlendirebilme (2)
Öğrenci (maskeli):
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Etkinlik:
Görsel Dikkat: Renk Eşleştirme
Motivasyon: Zaman Farkındalığı
Bölünmüş Dikkat: Çift Görev
Ders-işleme yönergesi (T.D.1.1): Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün.
Atamayı deftere işle

Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.

Atama-defteri (1)
ARD-05
MAT.2.1.1 · Sayı postası: oku-yaz-eşle
Görsel Dikkat: Renk Eşleştirme · 2026-09-10
sil
Sınav/gözlem Sonuç-Notu Defteri (sınırlı)

Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.

Deftere yaz

Defter boş.
~~~~

### SCH-SED-DOM-portfoy-atamali

~~~~text
SEDUVA Scholaria: Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).

v0.2.7 · VAMOLA Scholaria - Öğretmen Sınıf Panosu
Rapor
Görev-H deseni: "40 dk derste 3 kez yerinden kalktı" tipi gözlemlenebilir-sayılabilir dil. Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
Günün Ev–Okul Notu Taslağı (H-c kaynaklı)

Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.

Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.

Öğrenci Defteri — yazılı-portfolyo
Öğrenci:
ARD-05 (OGR-101)
ARD-06 (OGR-102)
KRT-12 (OGR-103)
SRY-22 (OGR-104)
Defterleri tara
0 kayıt · 4-defter salt-okunur

Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.

Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
~~~~

## C-SED-2 — Kaynak metin adayları

ID kaynağın bu tarihteki satırına bağlıdır; refactor sonrası satır kayabilir. JSX/template parçası birebir tam cümle değildir.

| ID | Kaynak:satır | Tür | Ham parça (↵=satır sonu) | Görünürlük sınıfı |
|---|---|---|---|---|
| SCH-SED-0001 | `App.tsx:42` | StringLiteral | B2B Yönetici | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0002 | `App.tsx:44` | JsxText | · VAMOLA Scholaria - Öğretmen Sınıf Panosu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0003 | `App.tsx:49` | JsxText | Sınıf Özeti (Shared Evidence Akışı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0004 | `App.tsx:50` | JsxText | Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0005 | `App.tsx:57` | JsxText | Sınıfı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0006 | `App.tsx:60` | JsxText | Öğr. Sayı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0007 | `App.tsx:60` | JsxText | · Ort. Fslope: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0008 | `App.tsx:61` | JsxText | Gün-içi nabzı aç → | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0009 | `App.tsx:65` | JsxText | MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0010 | `App.tsx:71` | JsxText | Sınıf (Dinamik Gating: G_contrast) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0011 | `App.tsx:72` | JsxText | Ders esnasında sınıf içi gürültü/dikkat dengesi. Seçili sınıfın göstergeleri: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0012 | `App.tsx:74` | JsxText | Hedef Sınıf: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0013 | `App.tsx:85` | JsxText | Aktif Parametre: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0014 | `App.tsx:85` | JsxText | Dynamic Gating Slope (Avg. G_contrast) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0015 | `App.tsx:85` | TemplateHead | Öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0016 | `App.tsx:85` | TemplateMiddle | · Ort. Fslope | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0017 | `App.tsx:85` | JsxText | [PRD §3.A deseninden MOCK] | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0018 | `App.tsx:87` | JsxText | G_contrast gün-içi eğrisi (sentetik-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0019 | `App.tsx:95` | JsxText | GFI | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0020 | `App.tsx:95` | JsxText | · Fslope | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0021 | `App.tsx:95` | JsxText | · görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0022 | `App.tsx:107` | JsxText | Gelişim Takibi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0023 | `App.tsx:108` | JsxText | Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0024 | `App.tsx:116` | JsxText | Öğrenci (Cihaz & Olay Dinleyicileri) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0025 | `App.tsx:117` | JsxText | Öğrenci Terminal UI. EventListener kilitleri (PRD §3.B) dürtüsel hataları engeller — mini-simülasyonda deneyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0026 | `App.tsx:132` | JsxText | — Terminal önizlemesi (MOCK) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0027 | `App.tsx:133` | JsxText | Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): dürtüsel-tık engellenir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0028 | `App.tsx:137` | TemplateHead | Kilit — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0029 | `App.tsx:137` | StringLiteral | Göreve Başla (kilit-demosu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0030 | `App.tsx:139` | JsxText | Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0031 | `App.tsx:148` | JsxText | Öğretmen Paneli (Teacher Cockpit) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0032 | `App.tsx:158` | JsxText | Ders & Görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0033 | `App.tsx:159` | JsxText | 2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0034 | `App.tsx:167` | JsxText | BEP Hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0035 | `App.tsx:168` | JsxText | Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0036 | `App.tsx:175` | JsxText | Aile Bilgilendirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0037 | `App.tsx:176` | JsxText | Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0038 | `App.tsx:177` | JsxText | Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0039 | `App.tsx:184` | JsxText | MEB EBA Entegrasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0040 | `App.tsx:185` | JsxText | Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0041 | `App.tsx:186` | JsxText | Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0042 | `App.tsx:193` | JsxText | Sınıf İçi Ses Yönetimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0043 | `App.tsx:194` | JsxText | Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0044 | `App.tsx:201` | JsxText | Rapor | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0045 | `App.tsx:209` | JsxText | Ayarlar | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0046 | `App.tsx:210` | JsxText | Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0047 | `App.tsx:213` | JsxText | slot) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0048 | `App.tsx:216` | JsxText | MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0049 | `App.tsx:222` | JsxText | Sistem Kılavuzu ve Terimler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0050 | `App.tsx:223` | JsxText | Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0051 | `App.tsx:225` | JsxText | K-05: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0052 | `App.tsx:225` | JsxText | Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0053 | `App.tsx:226` | JsxText | K-02: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0054 | `App.tsx:226` | JsxText | Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0055 | `App.tsx:227` | JsxText | K-331: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0056 | `App.tsx:227` | JsxText | MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0057 | `App.tsx:228` | JsxText | K-334: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0058 | `App.tsx:228` | JsxText | Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0059 | `App.tsx:229` | JsxText | K-05/MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0060 | `App.tsx:229` | JsxText | ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0061 | `App.tsx:230` | JsxText | MOCK-değerleri: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0062 | `components/bep/BepHedef.tsx:20` | StringLiteral | kısmen | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0063 | `components/bep/BepHedef.tsx:20` | StringLiteral | gözlemlendi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0064 | `components/bep/BepHedef.tsx:31` | FirstTemplateToken | GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0065 | `components/bep/BepHedef.tsx:32` | TemplateHead | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0066 | `components/bep/BepHedef.tsx:32` | TemplateMiddle | (maske-ÖĞR) · Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0067 | `components/bep/BepHedef.tsx:33` | TemplateHead | Hedef-cümlesi (gözlemlenebilir-dil, K-14): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0068 | `components/bep/BepHedef.tsx:33` | LastTemplateToken | kazanımına bağlı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0069 | `components/bep/BepHedef.tsx:34` | TemplateHead | sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0070 | `components/bep/BepHedef.tsx:35` | FirstTemplateToken | İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0071 | `components/bep/BepHedef.tsx:36` | FirstTemplateToken | Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0072 | `components/bep/BepHedef.tsx:59` | JsxText | Sınır-şerhi: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0073 | `components/bep/BepHedef.tsx:59` | JsxText | Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu ↵         taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0074 | `components/bep/BepHedef.tsx:64` | JsxText | Hedef-şablonu üretimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0075 | `components/bep/BepHedef.tsx:66` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0076 | `components/bep/BepHedef.tsx:71` | JsxText | Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0077 | `components/bep/BepHedef.tsx:79` | JsxText | Hedef-şablonunu deftere ekle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0078 | `components/bep/BepHedef.tsx:85` | JsxText | Defter boş — yukarıdan hedef-şablonu üretin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0079 | `components/bep/BepHedef.tsx:94` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0080 | `components/bep/BepHedef.tsx:99` | JsxText | Haftalık gözlem-probu izgarası ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0081 | `components/bep/BepHedef.tsx:102` | StringLiteral | tıkla: durum değişir (yok→kısmen→gözlemlendi) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0082 | `components/bep/BepHedef.tsx:109` | JsxText | + haftalık-probe ekle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0083 | `components/bep/BepHedef.tsx:113` | JsxText | İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0084 | `components/defter/SonucNotu.tsx:31` | JsxText | Sınav/gözlem Sonuç-Notu Defteri (sınırlı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0085 | `components/defter/SonucNotu.tsx:33` | JsxText | Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız. ↵         Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0086 | `components/defter/SonucNotu.tsx:38` | StringLiteral | ör. "Pazartesi kısa-sayma-yazılısı — sınıf-geneli notu defterimde" (kategori-yazmayın) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0087 | `components/defter/SonucNotu.tsx:40` | JsxText | Deftere yaz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0088 | `components/defter/SonucNotu.tsx:44` | JsxText | Defter boş. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0089 | `components/defter/SonucNotu.tsx:48` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0090 | `components/ders/GorevAtama.tsx:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0091 | `components/ders/GorevAtama.tsx:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0092 | `components/ders/GorevAtama.tsx:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0093 | `components/ders/GorevAtama.tsx:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0094 | `components/ders/GorevAtama.tsx:40` | JsxText | kazanım-ağacı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0095 | `components/ders/GorevAtama.tsx:40` | JsxText | kazanım (Matematik 25 + Türkçe 37). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0096 | `components/ders/GorevAtama.tsx:45` | JsxText | Ders: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0097 | `components/ders/GorevAtama.tsx:46` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0098 | `components/ders/GorevAtama.tsx:47` | JsxText | Matematik (25) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0099 | `components/ders/GorevAtama.tsx:49` | JsxText | Türkçe (37) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0100 | `components/ders/GorevAtama.tsx:53` | JsxText | Kazanım: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0101 | `components/ders/GorevAtama.tsx:58` | JsxText | Öğrenci (maskeli): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0102 | `components/ders/GorevAtama.tsx:63` | JsxText | Etkinlik: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0103 | `components/ders/GorevAtama.tsx:71` | JsxText | Ders-işleme yönergesi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0104 | `components/ders/GorevAtama.tsx:76` | JsxText | Atamayı deftere işle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0105 | `components/ders/GorevAtama.tsx:79` | JsxText | Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması ↵           PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0106 | `components/ders/GorevAtama.tsx:85` | JsxText | Atama-defteri ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0107 | `components/ders/GorevAtama.tsx:87` | JsxText | Defter boş — yukarıdan atama işleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0108 | `components/ders/GorevAtama.tsx:99` | JsxText | sil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0109 | `components/ders/OneriSablonlari.tsx:10` | StringLiteral | Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0110 | `components/ders/OneriSablonlari.tsx:11` | StringLiteral | İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0111 | `components/ders/OneriSablonlari.tsx:12` | StringLiteral | Nefes Halkası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0112 | `components/ders/OneriSablonlari.tsx:13` | StringLiteral | Yer-seçimi: dikkat-dağınıklığı-anında öne-yakın sessiz-masa önerin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0113 | `components/ders/OneriSablonlari.tsx:14` | StringLiteral | Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0114 | `components/ders/OneriSablonlari.tsx:26` | TemplateHead | EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0115 | `components/ders/OneriSablonlari.tsx:28` | FirstTemplateToken | ⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0116 | `components/ders/OneriSablonlari.tsx:32` | JsxText | Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0117 | `components/ders/OneriSablonlari.tsx:33` | JsxText | YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0118 | `components/ders/OneriSablonlari.tsx:36` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0119 | `components/ders/OneriSablonlari.tsx:40` | JsxText | YZ Önerisi İste | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0120 | `components/ders/OneriSablonlari.tsx:46` | JsxText | BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0121 | `components/ders/OneriSablonlari.tsx:47` | JsxText | Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0122 | `components/ders/OneriSablonlari.tsx:61` | JsxText | ✓ Onayla ve Yürürlüğe Al | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0123 | `components/ders/OneriSablonlari.tsx:62` | JsxText | ✕ Reddet ve Gerekçelendir | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0124 | `components/ders/OneriSablonlari.tsx:69` | JsxText | YZ Önerisi Öğretmen Tarafından Reddedildi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0125 | `components/ders/OneriSablonlari.tsx:70` | StringLiteral | Gerekçe (Örn: Sınıf dinamiklerine bugün uygun değil) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0126 | `components/ders/OneriSablonlari.tsx:71` | JsxText | Kaydet | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0127 | `components/eba/EbaPaneli.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0128 | `components/eba/EbaPaneli.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0129 | `components/eba/EbaPaneli.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0130 | `components/eba/EbaPaneli.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0131 | `components/eba/EbaPaneli.tsx:28` | StringLiteral | gözlem-girişi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0132 | `components/eba/EbaPaneli.tsx:29` | TemplateMiddle | (maske-UID ÖĞR-•••) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0133 | `components/eba/EbaPaneli.tsx:29` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0134 | `components/eba/EbaPaneli.tsx:29` | TemplateMiddle | davranış-gözlemi; ör. " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0135 | `components/eba/EbaPaneli.tsx:29` | LastTemplateToken | " (gözlemlenebilir-sayılabilir dil). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0136 | `components/eba/EbaPaneli.tsx:33` | StringLiteral | • Bugün H-c kaydı yok — örnek-desen (sentetik): "ARD-05, Renk Eşleştirme görevi sırasında 2 kez kendi başladı; 1 kez ipucu istedi ve sürdürdü." | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0137 | `components/eba/EbaPaneli.tsx:35` | StringLiteral | GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0138 | `components/eba/EbaPaneli.tsx:36` | TemplateHead | Tarih: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0139 | `components/eba/EbaPaneli.tsx:36` | LastTemplateToken | · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0140 | `components/eba/EbaPaneli.tsx:38` | StringLiteral | [Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA'ya yazma-yok] | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0141 | `components/eba/EbaPaneli.tsx:45` | JsxText | 1 · Cihaz (Terminal) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0142 | `components/eba/EbaPaneli.tsx:45` | JsxText | EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0143 | `components/eba/EbaPaneli.tsx:48` | JsxText | 2 · daily-insight TASLAĞI | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0144 | `components/eba/EbaPaneli.tsx:48` | JsxText | Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0145 | `components/eba/EbaPaneli.tsx:51` | JsxText | 3 · [EBA POST] /api/v1/report/daily-insight | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0146 | `components/eba/EbaPaneli.tsx:52` | JsxText | PLANLI ENTEGRASYON — bu önizlemede gönderim YOK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0147 | `components/eba/EbaPaneli.tsx:57` | JsxText | K-331: salt-okunur çağrı — ödev/içerik yazılmaz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0148 | `components/eba/EbaPaneli.tsx:58` | JsxText | e-sınav girişi YOK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0149 | `components/eba/EbaPaneli.tsx:59` | JsxText | K-334: idari-mali otomasyon dışarı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0150 | `components/eba/EbaPaneli.tsx:60` | JsxText | Başarı Notu Yazılmaz · Maskeli UID | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0151 | `components/eba/EbaPaneli.tsx:65` | JsxText | Insight Taslağı Üret (yerel) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0152 | `components/eba/EbaPaneli.tsx:72` | JsxText | OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur; ↵         bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0153 | `components/izleme/FrictionMap.tsx:18` | StringLiteral | Ali Y. | Bağlı değil: kaynak rezervi |
| SCH-SED-0154 | `components/izleme/FrictionMap.tsx:19` | StringLiteral | Ayşe T. | Bağlı değil: kaynak rezervi |
| SCH-SED-0155 | `components/izleme/FrictionMap.tsx:20` | StringLiteral | Can B. | Bağlı değil: kaynak rezervi |
| SCH-SED-0156 | `components/izleme/FrictionMap.tsx:36` | JsxText | Öğrenme Sürtünme Haritası (Friction Map) | Bağlı değil: kaynak rezervi |
| SCH-SED-0157 | `components/izleme/FrictionMap.tsx:37` | JsxText | Öğrencilerin görev aşamalarındaki bilişsel dirençlerini ve kopma noktalarını gösterir. | Bağlı değil: kaynak rezervi |
| SCH-SED-0158 | `components/izleme/FrictionMap.tsx:44` | JsxText | Öğrenci | Bağlı değil: kaynak rezervi |
| SCH-SED-0159 | `components/izleme/FrictionMap.tsx:45` | JsxText | Görev | Bağlı değil: kaynak rezervi |
| SCH-SED-0160 | `components/izleme/FrictionMap.tsx:46` | JsxText | Başlama Direnci | Bağlı değil: kaynak rezervi |
| SCH-SED-0161 | `components/izleme/FrictionMap.tsx:47` | JsxText | Görev Sürdürme | Bağlı değil: kaynak rezervi |
| SCH-SED-0162 | `components/izleme/FrictionMap.tsx:48` | JsxText | Geçiş / Sonlandırma | Bağlı değil: kaynak rezervi |
| SCH-SED-0163 | `components/izleme/FrictionMap.tsx:78` | JsxText | Eğitsel Çıkarım Örneği: | Bağlı değil: kaynak rezervi |
| SCH-SED-0164 | `components/izleme/FrictionMap.tsx:78` | JsxText | Ali'nin MAT-02 görevine başlaması çok zor (Yüksek Direnç) ancak başladıktan sonra akıcı bir şekilde bitiriyor (Düşük Sürdürme Direnci). Ali'ye göreve başlarken kısa bir görsel tetikleyici vermek sürtünmeyi (friction) kırabilir. | Bağlı değil: kaynak rezervi |
| SCH-SED-0165 | `components/izleme/IzlemePaneli.tsx:16` | JsxText | MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0166 | `components/izleme/IzlemePaneli.tsx:16` | JsxText | seriler sentetik-gösterimdir (K-05); XR/Control-Task Faz-3 PLANLI-katmandır — bu ekranda koşmaz. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0167 | `components/izleme/IzlemePaneli.tsx:20` | JsxText | Öğrenci (maskeli): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0168 | `components/izleme/IzlemePaneli.tsx:28` | JsxText | d(SDRT)/dt — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0169 | `components/izleme/IzlemePaneli.tsx:28` | JsxText | (12 gözlem-noktası) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0170 | `components/izleme/IzlemePaneli.tsx:35` | JsxText | Gaze-Lock etkileşim-oranı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0171 | `components/izleme/IzlemePaneli.tsx:35` | JsxText | (sentetik-sabit · Faz-3 Control Task-M11) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0172 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | Aktif görev: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0173 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | GFI: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0174 | `components/izleme/IzlemePaneli.tsx:38` | JsxText | Fslope: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0175 | `components/izleme/IzlemePaneli.tsx:40` | JsxText | K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0176 | `components/ogretmen/Cockpit.tsx:17` | StringLiteral | SNF | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0177 | `components/ogretmen/Cockpit.tsx:22` | JsxText | MOCK: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0178 | `components/ogretmen/Cockpit.tsx:22` | JsxText | tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için ↵         yönlendirme-desteğidir (K-02) · eşik-önerisi: Fslope ≥ 0.07 → Nefes Halkası. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0179 | `components/ogretmen/Cockpit.tsx:27` | JsxText | Toplu Yorgunluk (Fslope) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0180 | `components/ogretmen/Cockpit.tsx:35` | JsxText | Fslope | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0181 | `components/ogretmen/Cockpit.tsx:36` | JsxText | GFI | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0182 | `components/ogretmen/Cockpit.tsx:37` | JsxText | yorgunluk-uyarısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0183 | `components/ogretmen/Cockpit.tsx:42` | JsxText | d(SDRT)/dt sınıf-eğrisi (sentetik-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0184 | `components/ogretmen/Cockpit.tsx:50` | JsxText | Nefes Halkası (Breathing Circle) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0185 | `components/ogretmen/Cockpit.tsx:57` | JsxText | Kılavuz-tempo: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0186 | `components/ogretmen/Cockpit.tsx:57` | JsxText | 4 sn al — 4 sn tut — 4 sn ver | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0187 | `components/ogretmen/Cockpit.tsx:57` | JsxText | · sınıf-öncesi/arası 2 tur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0188 | `components/ogretmen/Cockpit.tsx:59` | JsxText | öğrenci eşik-üstü → yönlendirme-önerisi hazır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0189 | `components/ogretmen/Cockpit.tsx:60` | StringLiteral | Eşik-üstü öğrenci yok. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0190 | `components/ogretmen/Cockpit.tsx:65` | JsxText | Yönlendirme-kartı üret | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0191 | `components/ogretmen/Cockpit.tsx:69` | JsxText | — gözlem-notu (MOCK): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0192 | `components/ogretmen/Cockpit.tsx:69` | StringLiteral | sınıf-geneli | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0193 | `components/ogretmen/Cockpit.tsx:69` | JsxText | için ↵             Nefes Halkası-tempo (4-4-4) denenebilir. Bu kart cihaza komut GÖNDERMEZ; öğretmen-sözüyle yürütülür. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0194 | `components/ogretmen/TransferGozlemKarti.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0195 | `components/ogretmen/TransferGozlemKarti.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0196 | `components/ogretmen/TransferGozlemKarti.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0197 | `components/ogretmen/TransferGozlemKarti.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0198 | `components/ogretmen/TransferGozlemKarti.tsx:79` | JsxText | Transfer Gözlem Kartı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0199 | `components/ogretmen/TransferGozlemKarti.tsx:80` | JsxText | Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0200 | `components/ogretmen/TransferGozlemKarti.tsx:82` | JsxText | Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı. ↵             Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0201 | `components/ogretmen/TransferGozlemKarti.tsx:89` | JsxText | MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0202 | `components/ogretmen/TransferGozlemKarti.tsx:94` | JsxText | Öğrenci (sentetik): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0203 | `components/ogretmen/TransferGozlemKarti.tsx:101` | JsxText | Gözlenen etkinlik: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0204 | `components/ogretmen/TransferGozlemKarti.tsx:110` | JsxText | Gözlenen davranışlar (işaretleyerek): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0205 | `components/ogretmen/TransferGozlemKarti.tsx:125` | JsxText | Kısa not (isteğe bağlı): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0206 | `components/ogretmen/TransferGozlemKarti.tsx:127` | StringLiteral | Örn. tahta örneğinden sonra kendi uygulamasına geçti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0207 | `components/ogretmen/TransferGozlemKarti.tsx:134` | JsxText | Kaydet (yerel) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0208 | `components/ogretmen/TransferGozlemKarti.tsx:137` | JsxText | kayıt · yalnız bu tarayıcıda | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0209 | `components/ogretmen/TransferGozlemKarti.tsx:144` | JsxText | Son kayıtlar: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0210 | `components/ogretmen/TransferGozlemKarti.tsx:147` | JsxText | hepsini temizle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0211 | `components/ogretmen/TransferGozlemKarti.tsx:153` | JsxText | davranış | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0212 | `components/portfoy/Portfoy.tsx:12` | StringLiteral | Gözlem-kartı (H-c) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0213 | `components/portfoy/Portfoy.tsx:13` | StringLiteral | Görev-ataması | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0214 | `components/portfoy/Portfoy.tsx:14` | StringLiteral | BEP-hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0215 | `components/portfoy/Portfoy.tsx:15` | StringLiteral | Sonuç-notu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0216 | `components/portfoy/Portfoy.tsx:32` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0217 | `components/portfoy/Portfoy.tsx:32` | TemplateMiddle | davranış-gözlemi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0218 | `components/portfoy/Portfoy.tsx:35` | TemplateHead | etkinlik atandı: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0219 | `components/portfoy/Portfoy.tsx:35` | TemplateMiddle | · kazanım | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0220 | `components/portfoy/Portfoy.tsx:38` | TemplateHead | BEP-hazırlık hedefi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0221 | `components/portfoy/Portfoy.tsx:38` | LastTemplateToken | haftalık-probu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0222 | `components/portfoy/Portfoy.tsx:41` | TemplateHead | sonuç-notu: " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0223 | `components/portfoy/Portfoy.tsx:54` | JsxText | Öğrenci Defteri — yazılı-portfolyo | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0224 | `components/portfoy/Portfoy.tsx:56` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0225 | `components/portfoy/Portfoy.tsx:61` | JsxText | Defterleri tara | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0226 | `components/portfoy/Portfoy.tsx:62` | JsxText | kayıt · 4-defter salt-okunur | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0227 | `components/portfoy/Portfoy.tsx:65` | JsxText | Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0228 | `components/portfoy/Portfoy.tsx:78` | JsxText | Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla ↵         bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0229 | `components/rapor/RaporOzeti.tsx:14` | StringLiteral | Göreve kendi başladı (yönlendirme olmadan) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0230 | `components/rapor/RaporOzeti.tsx:15` | StringLiteral | Zorlanınca ipucu istedi ve sürdürdü | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0231 | `components/rapor/RaporOzeti.tsx:16` | StringLiteral | Mola verdi ve döndü (akışı korudu) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0232 | `components/rapor/RaporOzeti.tsx:17` | StringLiteral | Sözel yönerge tek başına yeterli oldu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0233 | `components/rapor/RaporOzeti.tsx:28` | StringLiteral | gözlem | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0234 | `components/rapor/RaporOzeti.tsx:29` | StringLiteral | görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0235 | `components/rapor/RaporOzeti.tsx:29` | StringLiteral | gözlem-girişi yok | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0236 | `components/rapor/RaporOzeti.tsx:29` | TemplateHead | ; öğretmen-notu: " | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0237 | `components/rapor/RaporOzeti.tsx:34` | JsxText | Görev-H deseni: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0238 | `components/rapor/RaporOzeti.tsx:34` | JsxText | "40 dk derste 3 kez yerinden kalktı" tipi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0239 | `components/rapor/RaporOzeti.tsx:34` | JsxText | gözlemlenebilir-sayılabilir dil | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0240 | `components/rapor/RaporOzeti.tsx:34` | JsxText | . ↵         Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0241 | `components/rapor/RaporOzeti.tsx:38` | JsxText | Günün Ev–Okul Notu Taslağı (H-c kaynaklı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0242 | `components/rapor/RaporOzeti.tsx:41` | JsxText | Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0243 | `components/rapor/RaporOzeti.tsx:48` | JsxText | Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0244 | `components/ses/SesPaneli.tsx:16` | JsxText | PLANLI-KATMAN şerhi: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0245 | `components/ses/SesPaneli.tsx:16` | JsxText | donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü ↵         ayrımının | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0246 | `components/ses/SesPaneli.tsx:17` | JsxText | görsel-simülasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0247 | `components/ses/SesPaneli.tsx:17` | JsxText | vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0248 | `components/ses/SesPaneli.tsx:21` | JsxText | Ana Sinyal İzolasyonu — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0249 | `components/ses/SesPaneli.tsx:29` | JsxText | ana-sinyal | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0250 | `components/ses/SesPaneli.tsx:30` | JsxText | ortam-gürültüsü (izolasyon-arttıkça söner) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0251 | `components/ses/SesPaneli.tsx:35` | JsxText | Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0252 | `components/shell/Kabuk.tsx:6` | StringLiteral | Sınıf Özeti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0253 | `components/shell/Kabuk.tsx:7` | StringLiteral | Sınıf | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0254 | `components/shell/Kabuk.tsx:8` | StringLiteral | Öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0255 | `components/shell/Kabuk.tsx:9` | StringLiteral | Öğretmen | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0256 | `components/shell/Kabuk.tsx:10` | StringLiteral | Transfer Gözlem Kartı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0257 | `components/shell/Kabuk.tsx:11` | StringLiteral | Ders & Görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0258 | `components/shell/Kabuk.tsx:12` | StringLiteral | Aile Bilgilendirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0259 | `components/shell/Kabuk.tsx:13` | StringLiteral | BEP Hazırlık | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0260 | `components/shell/Kabuk.tsx:14` | StringLiteral | MEB EBA Entegrasyonu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0261 | `components/shell/Kabuk.tsx:15` | StringLiteral | Gelişim Takibi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0262 | `components/shell/Kabuk.tsx:16` | StringLiteral | Sınıf İçi Ses Yönetimi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0263 | `components/shell/Kabuk.tsx:19` | StringLiteral | Sistem Kılavuzu ve Terimler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0264 | `components/shell/Kabuk.tsx:32` | JsxText | SEDUVA Scholaria™ | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0265 | `components/shell/Kabuk.tsx:33` | JsxText | School Node · v | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0266 | `components/shell/Kabuk.tsx:50` | JsxText | Rol: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0267 | `components/shell/Kabuk.tsx:50` | JsxText | · B2B Sınıf Düğümü (School Node) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0268 | `components/shell/Kabuk.tsx:55` | JsxText | SEDUVA Scholaria: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0269 | `components/shell/Kabuk.tsx:55` | JsxText | Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0270 | `components/takip/GelisimTakibi.tsx:24` | JsxText | Gelişim-takibi (gözlem-çizelgesi) — | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0271 | `components/takip/GelisimTakibi.tsx:26` | JsxText | Öğrenci: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0272 | `components/takip/GelisimTakibi.tsx:33` | JsxText | GFI/Fslope serisi (MOCK-gösterim) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0273 | `components/takip/GelisimTakibi.tsx:37` | JsxText | Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0274 | `components/takip/GelisimTakibi.tsx:40` | JsxText | H-c gözlem-zaman-çizelgesi ( | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0275 | `components/takip/GelisimTakibi.tsx:40` | JsxText | kayıt) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0276 | `components/takip/GelisimTakibi.tsx:42` | JsxText | Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0277 | `components/takip/GelisimTakibi.tsx:47` | JsxText | davranış-gözlemi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0278 | `components/veli/VeliKoprusu.tsx:12` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0279 | `components/veli/VeliKoprusu.tsx:12` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0280 | `components/veli/VeliKoprusu.tsx:15` | StringLiteral | Eve dönüşte gün-içi bir gözlemi tek-cümleyle paylaşın ("bugün görevine kendi başladı"). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0281 | `components/veli/VeliKoprusu.tsx:16` | StringLiteral | Ödevi tek-seferde değil, 10 dakikalık iki-bölüm olarak planlayın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0282 | `components/veli/VeliKoprusu.tsx:17` | StringLiteral | Ekran-öncesi kısa nefes-rutini (4-4-4) birlikte deneyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0283 | `components/veli/VeliKoprusu.tsx:18` | StringLiteral | Talimatları tek-tek ve sırayla verin; tamamlanınca sözel takdir edin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0284 | `components/veli/VeliKoprusu.tsx:19` | StringLiteral | Uyku ve oyun-düzeni gözlem-notlarını hafta-sonu karşılaştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0285 | `components/veli/VeliKoprusu.tsx:30` | StringLiteral | Haftalık gözlem paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0286 | `components/veli/VeliKoprusu.tsx:39` | TemplateHead | HAFTALIK SINIF BÜLTENİ — TASLAK (yerel-üretim; gönderilmez) ↵ Sınıf: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0287 | `components/veli/VeliKoprusu.tsx:39` | TemplateMiddle | · Tarih: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0288 | `components/veli/VeliKoprusu.tsx:40` | TemplateHead | Sınıf-gözlemi (MOCK): öğrenci | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0289 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · ort. Fslope | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0290 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · son-alarm: | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0291 | `components/veli/VeliKoprusu.tsx:40` | TemplateMiddle | · bu-hafta | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0292 | `components/veli/VeliKoprusu.tsx:40` | LastTemplateToken | gözlem-kartı (H-c). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0293 | `components/veli/VeliKoprusu.tsx:41` | FirstTemplateToken | Bu haftanın genel-önerileri (sınıf-geneli; kişi-değerlendirmesi yok — K-02): | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0294 | `components/veli/VeliKoprusu.tsx:43` | FirstTemplateToken | Aile-EĞİTİMİ programı ve kişiye-özel içerik SUPPORTA ürünündedir; bu bülten yalnız bilgilendirme-notudur. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0295 | `components/veli/VeliKoprusu.tsx:48` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0296 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0297 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0298 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | gerçekleşti | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0299 | `components/veli/VeliKoprusu.tsx:52` | StringLiteral | planlandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0300 | `components/veli/VeliKoprusu.tsx:58` | JsxText | Haftalık Aile Bülteni — TASLAK | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0301 | `components/veli/VeliKoprusu.tsx:63` | JsxText | Bülten taslağı üret | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0302 | `components/veli/VeliKoprusu.tsx:66` | JsxText | Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0303 | `components/veli/VeliKoprusu.tsx:70` | JsxText | Veli Görüşme — Randevu Defteri | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0304 | `components/veli/VeliKoprusu.tsx:75` | JsxText | Haftalık gözlem paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0305 | `components/veli/VeliKoprusu.tsx:76` | JsxText | H-c kart-turu değerlendirme paylaşımı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0306 | `components/veli/VeliKoprusu.tsx:77` | JsxText | Gelişim-görüşmesi (gözlem-özetli) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0307 | `components/veli/VeliKoprusu.tsx:78` | JsxText | Diğer | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0308 | `components/veli/VeliKoprusu.tsx:80` | StringLiteral | görüşme-notu (isteğe bağlı) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0309 | `components/veli/VeliKoprusu.tsx:82` | JsxText | Randevu kaydet | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0310 | `components/veli/VeliKoprusu.tsx:85` | JsxText | Defter boş — randevu kaydedin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0311 | `components/veli/VeliKoprusu.tsx:98` | JsxText | Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0312 | `data/mock.ts:5` | StringLiteral | 2. Sınıf A Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0313 | `data/mock.ts:6` | StringLiteral | 2. Sınıf B Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0314 | `data/mock.ts:7` | StringLiteral | 4. Sınıf A Şubesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0315 | `data/mock.ts:11` | StringLiteral | Görsel Dikkat: Renk Eşleştirme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0316 | `data/mock.ts:12` | StringLiteral | Motivasyon: Zaman Farkındalığı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0317 | `data/mock.ts:13` | StringLiteral | Bölünmüş Dikkat: Çift Görev | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0318 | `data/mock.ts:25` | StringLiteral | Yorulma Uyarısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0319 | `data/mufredatYonerge.ts:9` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0320 | `data/mufredatYonerge.ts:13` | StringLiteral | Sayı postası: oku-yaz-eşle | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0321 | `data/mufredatYonerge.ts:13` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0322 | `data/mufredatYonerge.ts:13` | StringLiteral | Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0323 | `data/mufredatYonerge.ts:14` | StringLiteral | Onluk-birlik çantası | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0324 | `data/mufredatYonerge.ts:14` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0325 | `data/mufredatYonerge.ts:14` | StringLiteral | Nesneleri 10'luk torbalara koydurarak onluk-birlik ayrımını somutlaştırın; tahtadaki tabloya birlikte işleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0326 | `data/mufredatYonerge.ts:15` | StringLiteral | Sayı doğrusu düellosu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0327 | `data/mufredatYonerge.ts:15` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0328 | `data/mufredatYonerge.ts:15` | StringLiteral | Yer-matında sayı doğrusu çizip komşu-sayılar arasında yürüyerek yer-değiştirme oyunu oynatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0329 | `data/mufredatYonerge.ts:16` | StringLiteral | Yüzlük tablo zıplaş | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0330 | `data/mufredatYonerge.ts:16` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0331 | `data/mufredatYonerge.ts:16` | StringLiteral | Yüzlük tabloda 1'er ve 10'ar atlamaları renkli-kalemle boyattırın; kuralı öğrenciye sözlü teyit ettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0332 | `data/mufredatYonerge.ts:17` | StringLiteral | Örüntü treni: kural-kur-devam-et | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0333 | `data/mufredatYonerge.ts:17` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0334 | `data/mufredatYonerge.ts:17` | StringLiteral | Şekil/sayı-kartlarıyla 2'şer-5'er-10'ar örüntüler kurdurtun; kuralı sözlutturup sıradaki-halkayı tahmin ettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0335 | `data/mufredatYonerge.ts:18` | StringLiteral | Tahmin kavanozu: grupla-tahmin et | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0336 | `data/mufredatYonerge.ts:18` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0337 | `data/mufredatYonerge.ts:18` | StringLiteral | Kavanozdaki nesneleri önce 10'luk gruplatıp tahmin yazdırın; sonra saydırarak tahmini doğrulatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0338 | `data/mufredatYonerge.ts:19` | StringLiteral | Bütün-yarım-çeyrek pizza | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0339 | `data/mufredatYonerge.ts:19` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0340 | `data/mufredatYonerge.ts:19` | StringLiteral | Kâğıt-daireleri katlatıp keserek yarım/çeyrek/bütün ilişkisini yapıştırma-panosunda kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0341 | `data/mufredatYonerge.ts:20` | StringLiteral | Kasaba para turu | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0342 | `data/mufredatYonerge.ts:20` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0343 | `data/mufredatYonerge.ts:20` | StringLiteral | Sınıf-mağazası dramatizasyonu kurun; TL-banknot kopyalarıyla alışveriş yaptırıp harcama-çizelgesi doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0344 | `data/mufredatYonerge.ts:21` | StringLiteral | Tam saat, yarım saat: saat-avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0345 | `data/mufredatYonerge.ts:21` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0346 | `data/mufredatYonerge.ts:21` | StringLiteral | Kart-saatlerle tam/yarım-saat ayırımı yaptırın; gün-içi rutini saat-bilgisiyle eşleştirme-turu kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0347 | `data/mufredatYonerge.ts:22` | StringLiteral | Karış mı, cetvel mi? | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0348 | `data/mufredatYonerge.ts:22` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0349 | `data/mufredatYonerge.ts:22` | StringLiteral | Aynı uzunluğu karış, adım ve cetvel ile ölçtürüp sonuçları karşılaştırın; standart-ölçü gereğini tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0350 | `data/mufredatYonerge.ts:23` | StringLiteral | Tahmin çubuğu: ölç-karşılaştır | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0351 | `data/mufredatYonerge.ts:23` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0352 | `data/mufredatYonerge.ts:23` | StringLiteral | Uzunlukları önce tahmin ettirip yazdırın; sonra cetveliyle ölçtürüp tahmin-ölçü tablosunu doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0353 | `data/mufredatYonerge.ts:24` | StringLiteral | Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0354 | `data/mufredatYonerge.ts:24` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0355 | `data/mufredatYonerge.ts:24` | StringLiteral | Sınıf-içi senaryolardan toplama-çıkarma problemleri kurdurtun; çözümü tek-cümleyle anlattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0356 | `data/mufredatYonerge.ts:25` | StringLiteral | Tahmin et, zihinden işle, tutarlılığı açıkla | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0357 | `data/mufredatYonerge.ts:25` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0358 | `data/mufredatYonerge.ts:25` | StringLiteral | İşlemi önce zihinden-tahmin ettirin; sonra yazıyla doğrulatıp tahminle-sonucu karşılaştırıp açıklattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0359 | `data/mufredatYonerge.ts:26` | StringLiteral | Toplama-çıkarma ters-ilişkisi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0360 | `data/mufredatYonerge.ts:26` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0361 | `data/mufredatYonerge.ts:26` | StringLiteral | Toplamadan çıkarma ürettirtin (a+b=c → c−b=a); boşluklu-kartlarla eşleştirme-oyunuyla pekiştirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0362 | `data/mufredatYonerge.ts:27` | StringLiteral | Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0363 | `data/mufredatYonerge.ts:27` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0364 | `data/mufredatYonerge.ts:27` | StringLiteral | Eş-öbek dizilimleri kurdurtun; toplamanın-kısa-yolu olarak çarpma yazdırın (2+2+2 = 3×2). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0365 | `data/mufredatYonerge.ts:28` | StringLiteral | Çarpan ve çarpım: bileşenler | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0366 | `data/mufredatYonerge.ts:28` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0367 | `data/mufredatYonerge.ts:28` | StringLiteral | 3×4 gibi işlemlerde parça-adlarını öğretin (çarpan-çarpan-çarpım); geriden-seçme oyunu oynatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0368 | `data/mufredatYonerge.ts:29` | StringLiteral | Eşitliğin anlamları: denge | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0369 | `data/mufredatYonerge.ts:29` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0370 | `data/mufredatYonerge.ts:29` | StringLiteral | Terazi-deseninde boşluğa sayı yazdırarak eşitliği kurdurtun (5+3=□+2); dengeyi cümleyle açıklatın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0371 | `data/mufredatYonerge.ts:30` | StringLiteral | Geometri ayırma bandı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0372 | `data/mufredatYonerge.ts:30` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0373 | `data/mufredatYonerge.ts:30` | StringLiteral | Şekil-kartlarını kenar ve köşe-özelliklerine göre sınıflandırma-bandına yerleştirtin; ayrımı sözlü gerekçelendirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0374 | `data/mufredatYonerge.ts:31` | StringLiteral | Küp kule inşaatı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0375 | `data/mufredatYonerge.ts:31` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0376 | `data/mufredatYonerge.ts:31` | StringLiteral | Küp-kule inşa ettirin; küp-sayısını önce-tahmin sonra-saydırarak karşılaştırma-satırı yazdırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0377 | `data/mufredatYonerge.ts:32` | StringLiteral | Şekil mozaik atölyesi | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0378 | `data/mufredatYonerge.ts:32` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0379 | `data/mufredatYonerge.ts:32` | StringLiteral | Kare/üçgen mozaiklerle yeni-şekiller oluşturtun; hangi-şekillerden oluştuğunu anlattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0380 | `data/mufredatYonerge.ts:33` | StringLiteral | Döndür-karşılaştır: aynı mı, farklı mı? | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0381 | `data/mufredatYonerge.ts:33` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0382 | `data/mufredatYonerge.ts:33` | StringLiteral | Kesik-şekilleri döndürüp aynı/farklı ayırımı yaptırın; döndürünce adın-değişmediğini tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0383 | `data/mufredatYonerge.ts:34` | StringLiteral | Bardak sorusu: tahmin-ölç | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0384 | `data/mufredatYonerge.ts:34` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0385 | `data/mufredatYonerge.ts:34` | StringLiteral | Aynı sıvıyı ince/geniş bardaklara döktürüp miktarın-değişmediğini gözlemletin (korunum-yargısı kurdurmadan). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0386 | `data/mufredatYonerge.ts:35` | StringLiteral | Hedefe yol: planla-izle-analiz | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0387 | `data/mufredatYonerge.ts:35` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0388 | `data/mufredatYonerge.ts:35` | StringLiteral | Sınıf-planında A→B arası yolları çizdirtin; en-kısayı seçtirtin ve adım-adım plan-izle-analiz turu yapın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0389 | `data/mufredatYonerge.ts:36` | StringLiteral | Ayna avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0390 | `data/mufredatYonerge.ts:36` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0391 | `data/mufredatYonerge.ts:36` | StringLiteral | Harf ve şekil-kartlarını aynaya tutturtup simetrikleri avlattırın; simetri-çizgisini kendilerine bozdurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0392 | `data/mufredatYonerge.ts:37` | StringLiteral | İki grup, bir grafik | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0393 | `data/mufredatYonerge.ts:37` | StringLiteral | MAT | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0394 | `data/mufredatYonerge.ts:37` | StringLiteral | Basit sınıf-anketi yapılıp sonuçları resimli-grafiğe işlettirin; "kaç-fazla/kaç-az" soruları sordurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0395 | `data/mufredatYonerge.ts:39` | StringLiteral | Dinleme/izlemeyi yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0396 | `data/mufredatYonerge.ts:39` | StringLiteral | Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0397 | `data/mufredatYonerge.ts:40` | StringLiteral | Dinlediklerinden anlam kurma: ana-fikir avcısı | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0398 | `data/mufredatYonerge.ts:40` | StringLiteral | Kısa-hikâye dinlettirin; ana-fikri tek-cümleyle tahmin ettirip sınıfça tartışın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0399 | `data/mufredatYonerge.ts:41` | StringLiteral | Dinlediklerini/izlediklerini çözümleyebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0400 | `data/mufredatYonerge.ts:41` | StringLiteral | Sebep-sonuç içeren masal dinlettirin; "neden-bekledi?" sorularıyla çözümleme-tartışması kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0401 | `data/mufredatYonerge.ts:42` | StringLiteral | Dinleme/izleme sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0402 | `data/mufredatYonerge.ts:42` | StringLiteral | Dinleme-sonu "ne-anladım" paylaşım-çemberi yaptırın; kendi-dinlemesine bakan cümle kurdurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0403 | `data/mufredatYonerge.ts:43` | StringLiteral | Dinleme/izlemeyi yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0404 | `data/mufredatYonerge.ts:43` | StringLiteral | Haber/duyuru dinlettin; kim-ne-zaman ipuçlarını dinlerken resimli-not aldırtın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0405 | `data/mufredatYonerge.ts:44` | StringLiteral | Dinledikleri/izledikleri ile ilgili anlam oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0406 | `data/mufredatYonerge.ts:44` | StringLiteral | Kurallar-metni dinlettirip dinlediklerinden tek-cümlelik anlam-özeti ürettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0407 | `data/mufredatYonerge.ts:45` | StringLiteral | Dinlediklerini/izlediklerini çözümleyebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0408 | `data/mufredatYonerge.ts:45` | StringLiteral | Sıralı-olay anlatımı dinlettin; önce/sonra kartlarını doğru-sıraya dizdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0409 | `data/mufredatYonerge.ts:46` | StringLiteral | Dinleme/izleme sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0410 | `data/mufredatYonerge.ts:46` | StringLiteral | Gürültülü ve sessiz ortamda kısa-dinleme karşılaştırması yaptırın; farkı birlikte tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0411 | `data/mufredatYonerge.ts:47` | StringLiteral | Dinleme/izleme sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0412 | `data/mufredatYonerge.ts:47` | StringLiteral | Dinlediği-hikâyeyi özetlettirin; güçlü-dinleme belirtilerini birlikte listelettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0413 | `data/mufredatYonerge.ts:48` | StringLiteral | Konuşmalarını yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0414 | `data/mufredatYonerge.ts:48` | StringLiteral | Toplantı-çemberinde söz-sırası kuralıyla kısa-konuşmalar yaptırın; el-kaldırma rutinini pekiştirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0415 | `data/mufredatYonerge.ts:49` | StringLiteral | Konuşmalarında içerik oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0416 | `data/mufredatYonerge.ts:49` | StringLiteral | Kim/zaman/yer/olay ipuçlarını içeren olay-anlatımı görevi verin; ipuçlarını kullanma-adımını gözlemleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0417 | `data/mufredatYonerge.ts:50` | StringLiteral | Konuşma kurallarını uygulayabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0418 | `data/mufredatYonerge.ts:50` | StringLiteral | Göz-teması ve ses-şiddeti hedefleriyle rol-oyunu konuşmaları kurdurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0419 | `data/mufredatYonerge.ts:51` | StringLiteral | Konuşma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0420 | `data/mufredatYonerge.ts:51` | StringLiteral | Konuşma-sonu "anlatabildim-mi" öz-tartışma çemberi yaptırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0421 | `data/mufredatYonerge.ts:52` | StringLiteral | Konuşmalarını yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0422 | `data/mufredatYonerge.ts:52` | StringLiteral | Sınıf-tartışmasında sıra-alma kartları kullanın; dinle-söyle rutini kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0423 | `data/mufredatYonerge.ts:53` | StringLiteral | Konuşmalarında içerik oluşturabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0424 | `data/mufredatYonerge.ts:53` | StringLiteral | Gezi/gün-anlatısında önce-sonra-en-son bağlaçlarını kullanma-hedefi verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0425 | `data/mufredatYonerge.ts:54` | StringLiteral | Konuşma kurallarını uygulayabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0426 | `data/mufredatYonerge.ts:54` | StringLiteral | Telefon-dramatizasyonu kurdurtun; selam-amaç-kapanış üçlüsünü denettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0427 | `data/mufredatYonerge.ts:55` | StringLiteral | Konuşma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0428 | `data/mufredatYonerge.ts:55` | StringLiteral | Ortam-seçiminin anlaşılırlığa etkisini oyunla gözlemletip tartıştırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0429 | `data/mufredatYonerge.ts:56` | StringLiteral | Konuşma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0430 | `data/mufredatYonerge.ts:56` | StringLiteral | Konuşma-sonu iki-güçlü-yön bir-gelişim-alanı paylaşımı yaptırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0431 | `data/mufredatYonerge.ts:57` | StringLiteral | Okuma sürecini yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0432 | `data/mufredatYonerge.ts:57` | StringLiteral | Sessiz-okuma rutini kurun; satır-takip kartıyla odaklanma davranışını gözlem-notuyla izleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0433 | `data/mufredatYonerge.ts:58` | StringLiteral | Okuduklarından anlam kurma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0434 | `data/mufredatYonerge.ts:58` | StringLiteral | Kısa-metin okutturup yanıtı metinde-bulunur sorular sorun; işaretlettirin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0435 | `data/mufredatYonerge.ts:59` | StringLiteral | Okuduklarını çözümleyebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0436 | `data/mufredatYonerge.ts:59` | StringLiteral | Karakter/yer-bilgisi isteyen çözümleme-sorularıyla metin-tartışması kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0437 | `data/mufredatYonerge.ts:60` | StringLiteral | Okuma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0438 | `data/mufredatYonerge.ts:60` | StringLiteral | Okuma-ortamını birlikte düzenlettirin; gürültünün anlamaya-etkisini gözlemletin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0439 | `data/mufredatYonerge.ts:61` | StringLiteral | Okuma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0440 | `data/mufredatYonerge.ts:61` | StringLiteral | Okuduğunu-yeniden-anlatma çifti kurun; kendi-anlamasını kontrol-cümlesiyle bağdattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0441 | `data/mufredatYonerge.ts:62` | StringLiteral | Okuma sürecini yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0442 | `data/mufredatYonerge.ts:62` | StringLiteral | Satır-takip kartı kullanımını modelleyip her-okurda uygulattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0443 | `data/mufredatYonerge.ts:63` | StringLiteral | Okudukları ile ilgili anlam oluşturabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0444 | `data/mufredatYonerge.ts:63` | StringLiteral | Yanıtı metinde-olan sorular sorun; buldukları-satırı gösterdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0445 | `data/mufredatYonerge.ts:64` | StringLiteral | Okuduklarını çözümleyebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0446 | `data/mufredatYonerge.ts:64` | StringLiteral | İleti-bulma sorusuyla kısa-hikâye tartışması yaptırın ("bu-hikâye ne-öğretti?"). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0447 | `data/mufredatYonerge.ts:65` | StringLiteral | Okuma sürecine etki eden durumları gözden geçirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0448 | `data/mufredatYonerge.ts:65` | StringLiteral | Bilinmeyen-kelime sözlük-köşesi kurun; bakma-adımını modelleyip uygulattın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0449 | `data/mufredatYonerge.ts:66` | StringLiteral | Okuma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0450 | `data/mufredatYonerge.ts:66` | StringLiteral | Hikâye-özetini kendi-kelimeleriyle anlattırın; anlamasını gözden-geçirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0451 | `data/mufredatYonerge.ts:67` | StringLiteral | Yazılı anlatım becerilerini yönetebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0452 | `data/mufredatYonerge.ts:67` | StringLiteral | Oturuş ve kalem-tutuş kontrol-listesiyle yazma-hazırlığı yaptırın; listeyi öğrenciyle birlikte doldurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0453 | `data/mufredatYonerge.ts:68` | StringLiteral | Yazılarında içerik oluşturma | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0454 | `data/mufredatYonerge.ts:68` | StringLiteral | Gün-içi olayı üç-cümleyle yazdirtin; önce-sonra kelimelerini kullanma-hedefi verin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0455 | `data/mufredatYonerge.ts:69` | StringLiteral | Yazma kurallarını uygulayabilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0456 | `data/mufredatYonerge.ts:69` | StringLiteral | Cümle-başı büyük-harf ve nokta-avcılığı yaptırın; yazısını kendine-tarattırın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0457 | `data/mufredatYonerge.ts:70` | StringLiteral | Yazma sürecini değerlendirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0458 | `data/mufredatYonerge.ts:70` | StringLiteral | Yazıyı sesli-okuyarak-kontrol rutini kurup arkadaşa-okutma turu yapın. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0459 | `data/mufredatYonerge.ts:71` | StringLiteral | Yazılı anlatım becerilerini yönetebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0460 | `data/mufredatYonerge.ts:71` | StringLiteral | Yazma-öncesi üç-kelimelik mini-plan yaptırıp taslağa geçirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0461 | `data/mufredatYonerge.ts:72` | StringLiteral | Yazılarında içerik oluşturabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0462 | `data/mufredatYonerge.ts:72` | StringLiteral | Tarih-hitap-ileti-imza şablonuyla sınıf-içi mektup yazdirtin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0463 | `data/mufredatYonerge.ts:73` | StringLiteral | Yazma kurallarını uygulayabilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0464 | `data/mufredatYonerge.ts:73` | StringLiteral | Noktalama-kartlarıyla cümle-düzeltme yarışı kurun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0465 | `data/mufredatYonerge.ts:74` | StringLiteral | Yazma sürecine etki eden durumları gözden geçirebilme | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0466 | `data/mufredatYonerge.ts:74` | StringLiteral | Kalem-tutuşu düzeltme egzersizlerini kısa-turlarla yaptırın; yorgunluk-belirtisini gözlemleyin. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0467 | `data/mufredatYonerge.ts:75` | StringLiteral | Yazma sürecini değerlendirebilme (2) | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0468 | `data/mufredatYonerge.ts:75` | StringLiteral | Yazım-noktalama-anlam üçlü-kontrol listesini birlikte doldurtun. | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0469 | `data/mufredatYonerge.ts:78` | StringLiteral | 2. sınıf | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |
| SCH-SED-0470 | `data/mufredatYonerge.ts:80` | StringLiteral | Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08). | App/import bağlamında; koşullu görünürlük ayrıca DOM’da |

## C-SED-3 — Tam TS/TSX kaynak bağlamı

Ürün kodu değiştirilmeden kopyalandı; bu bölüm UI listesi değildir. Teknik alanlar/yorumlar/bağlı olmayan bileşenler görünür metinden ayrı okunur. Satır sayımı aşağıdaki blokların ilk satırından başlar.

### `App.tsx`

13560 B · SHA-256 `ca20837b65e8b3aeb4da6960fb16af7a380b33fa084a9e5318208c89694009bc`

~~~~tsx
/**
 * SCHOLARIA App — K-554 CANLI-EKRAN-TURU (9/11 ekran artık etkileşimli; v0.2.2).
 * Canlı: Pano (tıklanır sınıf-nabız) · Sınıf (seçici↔veri + G_contrast eğrisi) · Öğrenci (görev-detay +
 * dürtü-kilidi mini-simülasyon) · Öğretmen-Cockpit · EBA (salt-okunur akış + yerel insight-taslağı) ·
 * İzleme (öğrenci-eğrisi) · Ses (görsel-simülasyon) · Rapor (görev-H özeti) · Yardım (şerh-sözlüğü).
 * Statik-kalan: Ayarlar (K-334 idari-mali dışarı). Transfer Gözlem (H-c): v0.2.0'dan beri canlı (K-451).
 * Tüm veriler sentetik/mock (K-05); "ölçen değil, gözlemleyen" (K-02); sunucusuz (K-05).
 */
import { useEffect, useState } from 'react';
import Kabuk, { type EkranId } from './components/shell/Kabuk';
import { SINIF_DURUMU, GOREVLER, SUBELER } from './data/mock';
import { gContrastSeri, noktalar } from './data/seriler';
import { KISITLAR } from './data/kisitlar';
import TransferGozlemKarti from './components/ogretmen/TransferGozlemKarti';
import Cockpit from './components/ogretmen/Cockpit';
import EbaPaneli from './components/eba/EbaPaneli';
import SesPaneli from './components/ses/SesPaneli';
import IzlemePaneli from './components/izleme/IzlemePaneli';
import RaporOzeti from './components/rapor/RaporOzeti';
import GorevAtama from './components/ders/GorevAtama';
import VeliKoprusu from './components/veli/VeliKoprusu';
import GelisimTakibi from './components/takip/GelisimTakibi';
import OneriSablonlari from './components/ders/OneriSablonlari';
import SonucNotu from './components/defter/SonucNotu';
import BepHedef from './components/bep/BepHedef';
import Portfoy from './components/portfoy/Portfoy';

export default function App() {
  const [ekran, setEkran] = useState<EkranId>('pano');
  const [secSinif, setSecSinif] = useState<string>('2A');
  const [secGorev, setSecGorev] = useState<string | null>(null);
  const [geriSay, setGeriSay] = useState<number | null>(null);

  useEffect(() => {
    if (geriSay === null) return;
    if (geriSay === 0) { setGeriSay(null); return; }
    const t = setTimeout(() => setGeriSay((g) => (g === null ? null : g - 1)), 1000);
    return () => clearTimeout(t);
  }, [geriSay]);

  return (
    <Kabuk ekran={ekran} setEkran={setEkran} rol="B2B Yönetici">
      <div data-testid="surum-modu" className="mb-3 flex flex-wrap gap-2 items-center justify-center rounded-xl border px-3 py-2 text-[11px] font-semibold bg-slate-50 border-slate-200 text-slate-700">
        <span>v{__SURUM__} · VAMOLA Scholaria - Öğretmen Sınıf Panosu</span>
      </div>

      {ekran === 'pano' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf Özeti (Shared Evidence Akışı)</h2>
          <p className="text-sm text-slate-600">Şube, sınıf ve cihaz envanteri için B2B kurumsal özet paneli. Sınıf-kartına tıklayınca gün-içi nabız (Sınıf ekranı) açılır.</p>
          <div className="grid md:grid-cols-3 gap-3">
            {SINIF_DURUMU.map((s) => (
              <button key={s.sinifId} type="button" data-testid={`pano-sinif-${s.sinifId}`}
                onClick={() => { setSecSinif(s.sinifId); setEkran('sinif'); }}
                className="text-left border border-slate-200 p-4 rounded-xl space-y-1 bg-white hover:border-indigo-300 cursor-pointer">
                <div className="flex items-center justify-between">
                  <span className="font-bold">{s.sinifId} Sınıfı</span>
                  <span className={`text-[10px] px-1.5 py-0.5 rounded-full font-bold ${s.sonAlarm === 'Yok' ? 'bg-emerald-100 text-emerald-700' : 'bg-amber-100 text-amber-700'}`}>{s.sonAlarm}</span>
                </div>
                <div className="text-xs text-slate-500">Öğr. Sayı: {s.ogrenciler.length} · Ort. Fslope: {s.ortalamaFslope.toFixed(2)}</div>
                <div className="text-[10px] text-indigo-600">Gün-içi nabzı aç →</div>
              </button>
            ))}
          </div>
          <p className="text-[11px] text-slate-500">MOCK (K-05): sınıf-değerleri sentetiktir; pedagojik detay Sınıf menüsünde.</p>
        </div>
      )}

      {ekran === 'sinif' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf (Dinamik Gating: G_contrast)</h2>
          <p className="text-sm text-slate-600">Ders esnasında sınıf içi gürültü/dikkat dengesi. Seçili sınıfın göstergeleri:</p>
          <label className="inline-flex items-center gap-2 text-xs font-semibold text-slate-700">
            Hedef Sınıf:
            <select data-testid="sinif-secici" value={secSinif} onChange={(e) => setSecSinif(e.target.value)} className="rounded-lg border border-slate-200 bg-white px-2 py-1 text-xs">
              {SUBELER.map((s) => <option key={s.id} value={s.id.replace('SUB-', '')}>{s.id}</option>)}
            </select>
          </label>
          {(() => {
            const d = SINIF_DURUMU.find((x) => x.sinifId === secSinif);
            const seri = gContrastSeri(secSinif);
            return (
              <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="sinif-paneli">
                <div className="p-3 bg-amber-50 border border-amber-200 rounded-xl text-xs text-amber-900">
                  <b>Aktif Parametre:</b> Dynamic Gating Slope (Avg. G_contrast) — <b>{seri[seri.length - 1].toFixed(2)}</b> · {secSinif} · {d ? `Öğrenci ${d.ogrenciler.length} · Ort. Fslope ${d.ortalamaFslope.toFixed(2)}` : ''} [PRD §3.A deseninden MOCK]
                </div>
                <div className="mt-3 text-xs font-semibold text-slate-700">G_contrast gün-içi eğrisi (sentetik-gösterim)</div>
                <svg width="100%" height={64} viewBox="0 0 280 64" className="mt-1" data-testid="sinif-egri">
                  <polyline points={noktalar(seri, 280, 64)} fill="none" stroke="#f59e0b" strokeWidth="2" />
                </svg>
                <div className="mt-3 space-y-1">
                  {(d?.ogrenciler ?? []).map((o) => (
                    <div key={o.id} className="flex items-center gap-2 text-xs">
                      <span className="w-16 font-semibold">{o.takmaAd}</span>
                      <span className="text-slate-500">GFI {o.gfi.toFixed(2)} · Fslope {o.fslope.toFixed(2)} · görev {o.aktifGorev}</span>
                    </div>
                  ))}
                </div>
              </div>
            );
          })()}
        </div>
      )}

      {ekran === 'izleme' && (
        <div className="space-y-3">
          <h2 className="font-bold">Gelişim Takibi</h2>
          <p className="text-xs text-slate-500 mb-4">Öğrencinin akademik ve sosyal becerilerindeki ilerlemeyi haftalık ve aylık bazda izleyin.</p>
          <IzlemePaneli />
          <GelisimTakibi />
        </div>
      )}

      {ekran === 'ogrenci' && (
        <div className="space-y-3">
          <h2 className="font-bold">Öğrenci (Cihaz & Olay Dinleyicileri)</h2>
          <p className="text-sm text-slate-600">Öğrenci Terminal UI. EventListener kilitleri (PRD §3.B) dürtüsel hataları engeller — mini-simülasyonda deneyin.</p>
          <div className="grid md:grid-cols-3 gap-3">
            {GOREVLER.map((g) => (
              <button key={g.id} type="button" data-testid={`ogrenci-gorev-${g.id}`}
                onClick={() => { setSecGorev(g.id); setGeriSay(null); }}
                className={`text-left bg-white border p-3 rounded-xl shadow-sm cursor-pointer ${secGorev === g.id ? 'border-indigo-500 ring-2 ring-indigo-100' : 'border-slate-200'}`}>
                <div className="font-bold text-sm">{g.baslik}</div>
                <div className="text-xs text-slate-500">{g.dersId} | {g.modul}</div>
              </button>
            ))}
          </div>
          {secGorev && (() => {
            const g = GOREVLER.find((x) => x.id === secGorev)!;
            return (
              <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="ogrenci-gorev-detay">
                <div className="font-bold text-sm">{g.baslik} — Terminal önizlemesi (MOCK)</div>
                <p className="text-xs text-slate-600 mt-1">Görev düğmesi ilk 3 sn KİLİTLİDİR (PRD §3.B EventListener): dürtüsel-tık engellenir.</p>
                <button type="button" data-testid="ogrenci-durtu-kilidi" disabled={geriSay !== null}
                  onClick={() => setGeriSay(3)}
                  className={`mt-2 px-4 py-2 rounded-xl text-sm font-semibold ${geriSay !== null ? 'bg-slate-200 text-slate-400 cursor-not-allowed' : 'bg-indigo-600 text-white hover:bg-indigo-700'}`}>
                  {geriSay !== null ? `Kilit — ${geriSay} sn` : 'Göreve Başla (kilit-demosu)'}
                </button>
                {geriSay === null && <span className="ml-3 text-xs text-emerald-700 font-semibold" data-testid="ogrenci-gorev-acildi">Göreve başlandı ✓ — bu önizlemede görev-içeriği açılmaz (K-05); kilit-mantığı gösterilmiştir.</span>}
              </div>
            );
          })()}
        </div>
      )}

      {ekran === 'ogretmen' && (
        <div className="space-y-3">
          <h2 className="font-bold">Öğretmen Paneli (Teacher Cockpit)</h2>
          <Cockpit secSinif={secSinif} />
          <OneriSablonlari secSinif={secSinif} />
        </div>
      )}

      {ekran === 'transfer' && <TransferGozlemKarti />}

      {ekran === 'ders' && (
        <div className="space-y-3">
          <h2 className="font-bold">Ders & Görev</h2>
          <p className="text-sm text-slate-600">2. sınıf kazanım-ağacı (62) + ders-işleme yönergeleri (özgün) · öğrenciye etkinlik-atama · sonuç-notu defteri (sınırlı).</p>
          <GorevAtama />
          <SonucNotu />
        </div>
      )}

      {ekran === 'bep' && (
        <div className="space-y-3">
          <h2 className="font-bold">BEP Hazırlık</h2>
          <p className="text-sm text-slate-600">Kazanım→hedef-şablonu (öğretmen-düzenler; resmî-BEP-DEĞİL) + haftalık gözlem-probu izgarası (yorum-yok). Kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.</p>
          <BepHedef />
        </div>
      )}

      {ekran === 'veli' && (
        <div className="space-y-3">
          <h2 className="font-bold">Aile Bilgilendirme</h2>
          <p className="text-xs text-slate-500 mb-4">Veliler ile paylaşılacak gözlem notları, haftalık özetler ve genel iletişim araçları.</p>
          <p className="text-sm text-slate-600">Aile-bilgilendirme bülteni TASLAĞI + veli görüşme-randevu defteri (yerel; otomasyon-yok).</p>
          <VeliKoprusu />
        </div>
      )}

      {ekran === 'eba' && (
        <div className="space-y-3">
          <h2 className="font-bold">MEB EBA Entegrasyonu</h2>
          <p className="text-xs text-slate-500 mb-4">Tek tıkla (SSO) MEB EBA platformuna güvenli giriş yapın ve ders materyallerine erişin. Sisteme veri çekilmez veya gönderilmez.</p>
          <p className="text-sm text-slate-600">Görev geri çağırma ve tek-tık SSO entegrasyon köprüsü — salt-okunur akış:</p>
          <EbaPaneli />
        </div>
      )}

      {ekran === 'ses' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sınıf İçi Ses Yönetimi</h2>
          <p className="text-xs text-slate-500 mb-4">Sınıfın akustik durumunu, arka plan gürültüsünü ve dikkat dağıtıcı uyaranları izleyerek optimal öğrenme ortamını sağlayın.</p>
          <SesPaneli />
        </div>
      )}

      {ekran === 'rapor' && (
        <div className="space-y-3">
          <h2 className="font-bold">Rapor</h2>
          <RaporOzeti />
          <Portfoy />
        </div>
      )}

      {ekran === 'ayarlar' && (
        <div className="space-y-3">
          <h2 className="font-bold">Ayarlar</h2>
          <p className="text-sm text-slate-600">Kurum politikası, şube yönetimi ve sistem parametreleri. K-334 idari-mali kapsam dışı onaylıdır — bu ecran salt-okunur kalır.</p>
          <div className="flex flex-wrap gap-2">
            {SUBELER.map((s) => (
              <div key={s.id} className="text-xs bg-slate-50 p-2 rounded border">{s.ad} ({s.ogrenciSayisi} slot)</div>
            ))}
          </div>
          <p className="text-[11px] text-slate-500">MOCK (K-05): şube-listesi sentetik örneklemdir; kurum-yönetimi gerçek-randumda.</p>
        </div>
      )}

      {ekran === 'yardim' && (
        <div className="space-y-3">
          <h2 className="font-bold">Sistem Kılavuzu ve Terimler</h2>
          <p className="text-xs text-slate-500 mb-4">Ekosistemde kullanılan eğitim terimleri ve kullanım kılavuzu.</p>
          <div className="rounded-2xl border border-slate-200 bg-white p-4 text-xs space-y-2" data-testid="yardim-sozluk">
            <div><b>K-05:</b> Sunucusuz-önce: hiçbir veri ağa gitmez; tüm kayıtlar yalnız bu tarayıcıdadır.</div>
            <div><b>K-02:</b> Ölçen değil, gözlemleyen: tanı/değerlendirme-yargısı yok; gözlemlenebilir-sayılabilir dil.</div>
            <div><b>K-331:</b> MEB/EBA salt-okunur: ödev/içerik yazılmaz, e-sınav girişi yok.</div>
            <div><b>K-334:</b> Idari-mali otomasyon kapsam-dışı (e-fatura/MEBBİS/BKDS yok).</div>
            <div><b>K-05/MOCK:</b> ÖĞR/ARD/KRT/SRY kodları sentetiktir; gerçek öğrenci verisi girilmez.</div>
            <div><b>MOCK-değerleri:</b> <code>{JSON.stringify(KISITLAR)}</code></div>
          </div>
          
        </div>
      )}
    </Kabuk>
  );
}

~~~~

### `components/bep/BepHedef.tsx`

7347 B · SHA-256 `62fe87c1bb7025199114bbda17bd8cc76ad805a3125f2ff9b455e46d39de39a1`

~~~~tsx
/**
 * BEP HAZIRLIK — Hedef-şablonu + gözlem-probu izgarası (K-558 · Yol-2; gap-analizi).
 * Kazanım→BEP-hedef-ŞABLONU üretimi (öğretmen düzenler; resmî BEP belgesi BURADA YAZILMAZ —
 * sınıf-öncesi gözlem-hazırlığıdır). Periyodik-probu: haftalık 3-durum gözlem (var/kısmen/yok) →
 * İZGARA (her-hücre bir-probe; eğilim-yorumu YAPILMAZ — K-02/K-04). Ekosistem-köprüsü: MENTORIA
 * Z-17 kanıt-paketi TASLAK'ı kurum-tarafıyla konuşur. Defter yalnız-yerel (K-05).
 */
import { useState } from 'react';
import { Target } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';
import { MUFREDAT_2 } from '../../data/mufredatYonerge';

const DEFTER = 'scholaria_bep_defteri_v024';
interface Probe { tarih: string; durum: 0 | 1 | 2 } // 0=yok · 1=kısmen · 2=gözlemlendi
interface Hedef { id: string; ogrenci: string; kazanımKod: string; metin: string; probe: Probe[] }

function oku(): Hedef[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Hedef[]; } catch { return []; } }
function yaz(h: Hedef[]) { try { localStorage.setItem(DEFTER, JSON.stringify(h)); } catch { /* yerel-yalnız */ } }

const DURUM_ETIKET = ['yok', 'kısmen', 'gözlemlendi'];
const DURUM_RENK = ['bg-slate-100 text-slate-500', 'bg-amber-100 text-amber-700', 'bg-emerald-100 text-emerald-700'];

export default function BepHedef() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [kod, setKod] = useState(MUFREDAT_2[0].kod);
  const [hedefler, setHedefler] = useState<Hedef[]>(() => oku());

  const kazanım = MUFREDAT_2.find((m) => m.kod === kod)!;
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  const sablon =
    `GÖZLEM-HEDEFİ ŞABLONU (taslak — öğretmen düzenler; resmî BEP belgesi değildir)\n` +
    `Öğrenci: ${o.takmaAd} (maske-ÖĞR) · Kazanım: ${kazanım.kod} — ${kazanım.ad}\n\n` +
    `Hedef-cümlesi (gözlemlenebilir-dil, K-14): ${o.takmaAd}, ${kazanım.ad.toLowerCase()} kazanımına bağlı ` +
    `sınıf-etkinliklerinde yönerge-izlerini GÖZLEMLENİR kılınacaktır: ${kazanım.yonerge}\n\n` +
    `İzleme: haftada-1 gözlem-probu (var/kısmen/yok) · 4 hafta · yorum-yok izgara.\n` +
    `Tanı/değerlendirme-yargısı içermez (K-02); kurum-tarafında MENTORIA Z-17 TASLAK-kanıt-paketine taşınır.`;

  function hedefEkle() {
    const h: Hedef = { id: Math.random().toString(36).slice(2, 9), ogrenci, kazanımKod: kod, metin: sablon, probe: [] };
    const yeni = [h, ...hedefler]; setHedefler(yeni); yaz(yeni);
  }
  function probeEkle(id: string) {
    const yeni = hedefler.map((h) => h.id === id
      ? { ...h, probe: [...h.probe, { tarih: new Date().toISOString().slice(0, 10), durum: ([0, 1, 2] as const)[h.probe.length % 3] }] }
      : h);
    setHedefler(yeni); yaz(yeni);
  }
  function probeCevir(id: string, idx: number) {
    const yeni = hedefler.map((h) => h.id !== id ? h : { ...h, probe: h.probe.map((p, k) => k === idx ? { ...p, durum: ((p.durum + 1) % 3) as 0 | 1 | 2 } : p) });
    setHedefler(yeni); yaz(yeni);
  }
  function sil(id: string) {
    const yeni = hedefler.filter((x) => x.id !== id); setHedefler(yeni); yaz(yeni);
  }

  return (
    <div className="space-y-4" data-testid="bep-hazirlik">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>Sınır-şerhi:</b> Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlığı ve hedef-şablonu
        taslağıdır (K-02/K-263-deseni). Defter yalnız bu-cihazdadır (K-05); kurum-akışında MENTORIA Z-17 TASLAK'ıyla konuşur.
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4 space-y-3">
        <h3 className="font-bold text-sm flex items-center gap-2"><Target className="w-4 h-4 text-indigo-600" /> Hedef-şablonu üretimi</h3>
        <div className="grid md:grid-cols-2 gap-2 text-xs">
          <label className="font-semibold text-slate-700">Öğrenci:
            <select data-testid="bep-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Kazanım:
            <select data-testid="bep-kazanim" value={kod} onChange={(e) => setKod(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {MUFREDAT_2.map((m) => <option key={m.kod} value={m.kod}>{m.kod} — {m.ad}</option>)}
            </select>
          </label>
        </div>
        <button type="button" data-testid="bep-sablon-uret" onClick={hedefEkle}
          className="px-4 py-2 rounded-xl bg-indigo-600 text-white text-sm font-semibold hover:bg-indigo-700">
          Hedef-şablonunu deftere ekle
        </button>
      </div>

      <div className="space-y-3">
        {hedefler.length === 0 ? (
          <p className="text-sm text-slate-500" data-testid="bep-bos">Defter boş — yukarıdan hedef-şablonu üretin.</p>
        ) : hedefler.slice(0, 6).map((h) => {
          const m = MUFREDAT_2.find((x) => x.kod === h.kazanımKod);
          const oo = OGRENCILER.find((x) => x.id === h.ogrenci);
          return (
            <div key={h.id} className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="bep-hedef-kart">
              <div className="flex items-center gap-2 text-xs">
                <span className="font-bold">{oo?.takmaAd}</span>
                <span className="text-slate-500">{h.kazanımKod} · {m?.ad}</span>
                <button type="button" onClick={() => sil(h.id)} className="ml-auto text-rose-600 text-[11px] font-semibold">sil</button>
              </div>
              <textarea readOnly rows={5} value={h.metin} data-testid="bep-sablon-metin"
                className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-[11px] font-mono" />
              <div className="mt-2 flex flex-wrap items-center gap-2 text-xs">
                <span className="font-semibold text-slate-700">Haftalık gözlem-probu izgarası ({h.probe.length}/4):</span>
                {h.probe.map((p, k) => (
                  <button key={k} type="button" data-testid={`bep-probe-${k}`} onClick={() => probeCevir(h.id, k)}
                    title="tıkla: durum değişir (yok→kısmen→gözlemlendi)"
                    className={`px-2 py-1 rounded-lg text-[10px] font-bold cursor-pointer ${DURUM_RENK[p.durum]}`}>
                    H{k + 1} · {p.tarih} · {DURUM_ETIKET[p.durum]}
                  </button>
                ))}
                {h.probe.length < 4 && (
                  <button type="button" onClick={() => probeEkle(h.id)} data-testid="bep-probe-ekle"
                    className="px-2 py-1 rounded-lg bg-slate-800 text-white text-[10px] font-bold">+ haftalık-probe ekle</button>
                )}
              </div>
              <p className="text-[11px] text-slate-500 mt-1">
                İzgara = her-hücre bir-haftalık gözlem (yok/kısmen/gözlemlendi). Eğilim-yorumu, puan ve karşılaştırma YAPILMAZ (K-02/K-04/K-14).
              </p>
            </div>
          );
        })}
      </div>
    </div>
  );
}

~~~~

### `components/defter/SonucNotu.tsx`

3033 B · SHA-256 `968827d3432cc289c24040ee9be469ed390899d353c4823c42e4477219884abb`

~~~~tsx
/**
 * SONUÇ-NOTU DEFTERİ (K-555-4, SINIRLI-çerçeve): öğretmenin KENDİ sınıf-içi ölçme-işi (MEB öğretmeni
 * yapar) burada İŞLENMEZ — yalnız tarih + serbest-not defteri tutulur; kategori/eşik-yorumu ÜRETİLMEZ
 * (K-02/K-04: ürün ölçme-arağı değildir). "Ders & Görev" ekranına gömülü.
 */
import { useState } from 'react';
import { NotebookPen } from 'lucide-react';

const DEFTER = 'scholaria_sonuc_notu_v023';
interface Satir { id: string; zaman: string; metin: string }

function oku(): Satir[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Satir[]; } catch { return []; } }

export default function SonucNotu() {
  const [metin, setMetin] = useState('');
  const [satirlar, setSatirlar] = useState<Satir[]>(() => oku());

  function ekle() {
    if (!metin.trim()) return;
    const s: Satir = { id: Math.random().toString(36).slice(2, 9), zaman: new Date().toISOString(), metin: metin.trim() };
    const yeni = [s, ...satirlar]; setSatirlar(yeni); setMetin('');
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }
  function sil(id: string) {
    const yeni = satirlar.filter((x) => x.id !== id); setSatirlar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }

  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="sonuc-notu">
      <h3 className="font-bold text-sm flex items-center gap-2"><NotebookPen className="w-4 h-4 text-slate-600" /> Sınav/gözlem Sonuç-Notu Defteri (sınırlı)</h3>
      <p className="text-[11px] text-slate-500 mt-1">
        Öğretmenin kendi ölçme-işi bu-üründe İŞLENMEZ; burada yalnız notunuzu tarihle tutarsınız.
        Kategori/eşik-yorumu üretülmez (K-02/K-04) — ürün ölçme-arağı değildir.
      </p>
      <div className="mt-2 flex gap-2">
        <input data-testid="sonuc-notu-gir" value={metin} onChange={(e) => setMetin(e.target.value)}
          placeholder='ör. "Pazartesi kısa-sayma-yazılısı — sınıf-geneli notu defterimde" (kategori-yazmayın)'
          className="flex-1 rounded-xl border border-slate-300 px-3 py-2 text-xs" />
        <button type="button" data-testid="sonuc-notu-ekle" onClick={ekle} className="px-3 py-2 rounded-xl bg-slate-800 text-white text-xs font-semibold">Deftere yaz</button>
      </div>
      <div className="mt-2 space-y-1">
        {satirlar.length === 0 ? (
          <p className="text-xs text-slate-500" data-testid="sonuc-bos">Defter boş.</p>
        ) : satirlar.slice(0, 6).map((s) => (
          <div key={s.id} data-testid="sonuc-satiri" className="flex items-center gap-2 text-[11px] rounded-lg border border-slate-200 px-2 py-1">
            <span className="text-slate-400">{s.zaman.slice(0, 10)}</span><span>{s.metin}</span>
            <button type="button" onClick={() => sil(s.id)} className="ml-auto text-rose-600 font-semibold">sil</button>
          </div>
        ))}
      </div>
    </div>
  );
}

~~~~

### `components/ders/GorevAtama.tsx`

6569 B · SHA-256 `6595fac05cd05f4b913ec1d3eef602382cb57b66ab8fb6fe229bb717a4cccce3`

~~~~tsx
/**
 * DERS & GÖREV — Görev Atama (K-555-1/5): öğretmen, MOCK-öğrenciye MEB-haritalı kazanım + etkinlik
 * ATAMASI yapar; kazanım-başına ders-işleme-yönergesi gösterilir (mufredatYonerge.ts — özgün).
 * Atama yalnız YEREL-deftere işlenir (K-05): çocuğa/cihaza gönderim YOKTUR; etkinliği çalıştıran
 * katman PERSONA'dır (MEB Ders Görevleri/Çocuk-modu) — SCHOLARIA atayan-katmandır.
 */
import { useState } from 'react';
import { BookOpen, ClipboardList } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';
import { MUFREDAT_2, MUFREDAT_KAYNAK_NOTU, MUFREDAT_SINIF } from '../../data/mufredatYonerge';

const DEFTER = 'scholaria_atama_defteri_v023';
interface Atama { id: string; zaman: string; ogrenci: string; kazanımKod: string; etkinlik: string }

function oku(): Atama[] { try { return JSON.parse(localStorage.getItem(DEFTER) ?? '[]') as Atama[]; } catch { return []; } }

export default function GorevAtama() {
  const [ders, setDers] = useState<'MAT' | 'TR'>('MAT');
  const [kod, setKod] = useState<string>(MUFREDAT_2[0].kod);
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [etkinlik, setEtkinlik] = useState(GOREVLER[0].id);
  const [atamalar, setAtamalar] = useState<Atama[]>(() => oku());

  const kazanım = MUFREDAT_2.find((m) => m.kod === kod)!;
  const listem = ders === 'MAT' ? MUFREDAT_2.filter((m) => m.ders === 'MAT') : MUFREDAT_2.filter((m) => m.ders === 'TR');

  function isle() {
    const a: Atama = { id: Math.random().toString(36).slice(2, 9), zaman: new Date().toISOString(), ogrenci, kazanımKod: kod, etkinlik };
    const yeni = [a, ...atamalar]; setAtamalar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }
  function sil(id: string) {
    const yeni = atamalar.filter((x) => x.id !== id); setAtamalar(yeni);
    try { localStorage.setItem(DEFTER, JSON.stringify(yeni)); } catch { /* yerel-yalnız */ }
  }

  return (
    <div className="space-y-4" data-testid="gorev-atama">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>{MUFREDAT_SINIF} kazanım-ağacı</b> · {MUFREDAT_2.length} kazanım (Matematik 25 + Türkçe 37). {MUFREDAT_KAYNAK_NOTU}
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4 space-y-3">
        <div className="flex flex-wrap gap-2 items-center text-xs">
          <span className="font-semibold text-slate-700 flex items-center gap-1"><BookOpen className="w-4 h-4 text-indigo-600" /> Ders:</span>
          <button type="button" data-testid="ders-mat" onClick={() => { setDers('MAT'); setKod('MAT.2.1.1'); }}
            className={`px-3 py-1.5 rounded-xl font-semibold ${ders === 'MAT' ? 'bg-indigo-600 text-white' : 'bg-slate-100 text-slate-700'}`}>Matematik (25)</button>
          <button type="button" data-testid="ders-tr" onClick={() => { setDers('TR'); setKod('T.D.1.1'); }}
            className={`px-3 py-1.5 rounded-xl font-semibold ${ders === 'TR' ? 'bg-indigo-600 text-white' : 'bg-slate-100 text-slate-700'}`}>Türkçe (37)</button>
        </div>

        <div className="grid md:grid-cols-3 gap-2 text-xs">
          <label className="font-semibold text-slate-700">Kazanım:
            <select data-testid="mufredat-sec" value={kod} onChange={(e) => setKod(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {listem.map((m) => <option key={m.kod} value={m.kod}>{m.kod} — {m.ad}</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Öğrenci (maskeli):
            <select data-testid="atama-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {OGRENCILER.map((o) => <option key={o.id} value={o.id}>{o.takmaAd} ({o.id})</option>)}
            </select>
          </label>
          <label className="font-semibold text-slate-700">Etkinlik:
            <select data-testid="atama-etkinlik" value={etkinlik} onChange={(e) => setEtkinlik(e.target.value)} className="mt-1 w-full rounded-lg border border-slate-200 px-2 py-1.5">
              {GOREVLER.map((g) => <option key={g.id} value={g.id}>{g.baslik}</option>)}
            </select>
          </label>
        </div>

        <div className="rounded-xl border border-indigo-200 bg-indigo-50 p-3 text-xs" data-testid="mufredat-yonerge">
          <b>Ders-işleme yönergesi ({kazanım.kod}):</b> {kazanım.yonerge}
        </div>

        <button type="button" data-testid="atama-isle" onClick={isle}
          className="px-4 py-2 rounded-xl bg-indigo-600 text-white text-sm font-semibold hover:bg-indigo-700">
          Atamayı deftere işle
        </button>
        <p className="text-[11px] text-slate-500">
          Atama yalnız bu-cihaz defterine işlenir (K-05) — çocuğa/cihaza gönderilmez; etkinliğin çalıştırılması
          PERSONA'nın MEB Ders Görevleri ekranındadır. SCHOLARIA atayan-katmandır.
        </p>
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><ClipboardList className="w-4 h-4 text-indigo-600" /> Atama-defteri ({atamalar.length})</h3>
        {atamalar.length === 0 ? (
          <p className="text-sm text-slate-500 mt-2" data-testid="atama-bos">Defter boş — yukarıdan atama işleyin.</p>
        ) : (
          <div className="mt-2 space-y-1.5">
            {atamalar.slice(0, 10).map((a) => {
              const o = OGRENCILER.find((x) => x.id === a.ogrenci);
              const g = GOREVLER.find((x) => x.id === a.etkinlik);
              const m = MUFREDAT_2.find((x) => x.kod === a.kazanımKod);
              return (
                <div key={a.id} data-testid="atama-satiri" className="flex items-center gap-2 text-xs rounded-xl border border-slate-200 px-3 py-2">
                  <span className="font-semibold">{o?.takmaAd}</span>
                  <span className="text-slate-500">{a.kazanımKod} · {m?.ad.slice(0, 32)}{m && m.ad.length > 32 ? '…' : ''}</span>
                  <span className="text-slate-400">{g?.baslik} · {a.zaman.slice(0, 10)}</span>
                  <button type="button" onClick={() => sil(a.id)} className="ml-auto text-rose-600 text-[11px] font-semibold">sil</button>
                </div>
              );
            })}
          </div>
        )}
      </div>
    </div>
  );
}

~~~~

### `components/ders/OneriSablonlari.tsx`

5240 B · SHA-256 `4d4bcaf870d4ede6648ee454e3fa0b2785ace68806b77e5d217116ce4ddf9c88`

~~~~tsx
/**
 * ÖĞRENCİ EĞİTİMSEL DESTEK ÖNERİLERİ (Human-Accountable AI): davranış-gözlemine bağlı sınıf-yönlendirme-önerileri;
 * tanı/kişi-yargısı yok (K-02) — öğretmen-sözüyle yürütülür. Cockpit'in altında çalışır.
 */
import { useState } from 'react';
import { Brain } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';

const SABLONLAR = [
  'Görev-bölme: uzun-görevi iki-kısa-bölüme ayırıp ara-mola verin.',
  'İpucu-kademesi: önce sözel-ipucu → sonra model-showing → sonra birlikte-yapma.',
  'Nefes Halkası (4-4-4) iki-tur: geçiş-anlarında sınıfça uygulayın.',
  'Yer-seçimi: dikkat-dağınıklığı-anında öne-yakın sessiz-masa önerin.',
  'Görev-başlatma kartı: "ilk-adım" kartı verin, kendi-başlamayı bekleyin.',
];

export default function OneriSablonlari({ secSinif }: { secSinif: string }) {
  const [secili, setSecili] = useState<number[]>([]);
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [yzMod, setYzMod] = useState(false);
  const [reddedildi, setReddedildi] = useState(false);
  
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  
  const metin = secili.length === 0 ? null :
    `EĞİTİMSEL DESTEK ÖNERİSİ (Öğretmen Sorumluluğunda · ${o.takmaAd} · ${secSinif}):\n` +
    secili.map((i) => `• ${SABLONLAR[i]}`).join('\n') +
    `\n\n⚠️ Bu not pedagojik sınıf-içi yönlendirme içindir; istatistiksel bir öneridir. Kesinlikle klinik/tanı yargısı içermez (K-02). Yalnızca öğretmenin onayıyla yürürlüğe girer.`;
    
  return (
    <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="oneri-sablonlari">
      <h3 className="font-bold text-sm flex items-center gap-2 text-indigo-900"><Brain className="w-4 h-4 text-indigo-600" /> Human-Accountable AI (YZ Asistanı) — Eğitimsel Destek Önerileri</h3>
      <p className="text-[11px] text-indigo-700 leading-relaxed mb-3 mt-1">YZ, öğrencinin T1 (Merkez) ve L1 (Ev) verilerini analiz ederek sınıf içi stratejiler sunar. Son karar daima öğretmendedir.</p>
      
      <div className="mt-2 flex items-center gap-2 text-xs">
        <span className="font-semibold text-slate-700">Öğrenci:</span>
        <select data-testid="oneri-ogrenci-sec" value={ogrenci} onChange={(e) => { setOgrenci(e.target.value); setYzMod(false); setReddedildi(false); setSecili([]); }} className="rounded-lg border border-slate-200 px-2 py-1">
          {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
        </select>
        {!yzMod && <button type="button" onClick={() => { setYzMod(true); setSecili([0, 2]); }} className="ml-2 bg-indigo-600 text-white px-3 py-1.5 rounded-lg font-semibold hover:bg-indigo-700">YZ Önerisi İste</button>}
      </div>
      
      {yzMod && !reddedildi && (
        <div className="mt-3">
          <div className="space-y-2 bg-white p-3 rounded-xl border border-indigo-100">
            <span className="text-[10px] font-bold text-amber-700 bg-amber-50 px-2 py-0.5 rounded-full border border-amber-200">BELİRSİZLİK KATMANI BİLDİRİMİ (Uyarı)</span>
            <p className="text-[11px] text-slate-600">Bu %78 güven aralığında bir pedagojik öneridir. YZ bir karar verici değil, asistan niteliğindedir. Lütfen öğretimsel bağlama göre inceleyin.</p>
            
            <div className="mt-2 space-y-1">
              {SABLONLAR.map((s, i) => (
                <label key={i} className="flex items-center gap-2 text-xs">
                  <input type="checkbox" data-testid={`oneri-${i}`} checked={secili.includes(i)}
                    onChange={() => setSecili((p) => (p.includes(i) ? p.filter((x) => x !== i) : [...p, i]))} />
                  {s}
                </label>
              ))}
            </div>
          </div>
          
          <div className="flex flex-wrap gap-2 mt-3">
            <button type="button" className="px-3 py-1.5 rounded-lg bg-teal-600 text-white text-xs font-semibold hover:bg-teal-700">✓ Onayla ve Yürürlüğe Al</button>
            <button type="button" onClick={() => setReddedildi(true)} className="px-3 py-1.5 rounded-lg bg-white border border-rose-200 text-rose-700 text-xs font-semibold hover:bg-rose-50">✕ Reddet ve Gerekçelendir</button>
          </div>
        </div>
      )}
      
      {reddedildi && (
         <div className="mt-3 p-3 bg-rose-50 border border-rose-200 rounded-xl space-y-2">
            <p className="text-xs font-bold text-rose-800">YZ Önerisi Öğretmen Tarafından Reddedildi</p>
            <input type="text" placeholder="Gerekçe (Örn: Sınıf dinamiklerine bugün uygun değil)" className="w-full text-xs p-2 rounded-lg border border-rose-300" />
            <button type="button" onClick={() => { setReddedildi(false); setYzMod(false); setSecili([]); }} className="px-3 py-1.5 bg-rose-600 text-white text-xs font-semibold rounded-lg mt-2">Kaydet</button>
         </div>
      )}
      
      {metin && yzMod && !reddedildi && <textarea readOnly rows={5} value={metin} data-testid="oneri-notu" className="w-full mt-3 rounded-xl border border-indigo-200 bg-white p-3 text-[11px] font-mono shadow-sm" />}
    </div>
  );
}
~~~~

### `components/eba/EbaPaneli.tsx`

4582 B · SHA-256 `293b1645d394763b4ed18fcf74ca9c076d9f6a91b9947d421fa1f411994ef9eb`

~~~~tsx
/**
 * MEB EBA — salt-okunur akış + yerel daily-insight TASLAĞI (K-554; PCV-brifing görev-F).
 * K-331: EBA'dan yalnız çağrılır, yazılmaz (ödev/içerik/e-sınav girişi YOK) · K-334 idari-mali dışarı ·
 * KVKK: EBA-UID cihazda maskelenir · [EBA POST] = PLANLI entegrasyon-adıdır — bu önizlemede ağ-gönderimi YOK (K-05).
 */
import { useState } from 'react';
import { ShieldCheck } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020'; // TransferGozlemKarti deposu — burada SALT-OKUNUR okunur
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

const DAVRANISLAR = [
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
];

export default function EbaPaneli() {
  const [taslak, setTaslak] = useState<string | null>(null);
  function uret() {
    let kayitlar: HcKayit[] = [];
    try { kayitlar = JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[]; } catch { kayitlar = []; }
    const satirlar = kayitlar.slice(0, 5).map((k) => {
      const o = OGRENCILER.find((x) => x.id === k.ogrenci);
      const g = GOREVLER.find((x) => x.id === k.gorev);
      const ilk = k.davranislar?.[0] !== undefined ? DAVRANISLAR[k.davranislar[0]] : 'gözlem-girişi';
      return `• ${o?.takmaAd ?? '•••'} (maske-UID ÖĞR-•••) — ${g?.baslik ?? 'görev'}: ${k.davranislar?.length ?? 0} davranış-gözlemi; ör. "${ilk}" (gözlemlenebilir-sayılabilir dil).`;
    });
    const govde = satirlar.length > 0
      ? satirlar.join('\n')
      : '• Bugün H-c kaydı yok — örnek-desen (sentetik): "ARD-05, Renk Eşleştirme görevi sırasında 2 kez kendi başladı; 1 kez ipucu istedi ve sürdürdü."';
    setTaslak(
      'GÜNLÜK EV–OKUL GÖZLEM-ÖZETİ — TASLAK (yerel-üretim; gönderilmez)\n' +
      `Tarih: ${new Date().toISOString().slice(0, 10)} · sınıf-bazlı, kişi-değerlendirmesi-olmayan dil (K-02)\n\n` +
      govde +
      '\n\n[Başarı Notu YAZILMAZ — yalnız gözlem-dili · maske-UID · K-331: EBA\'ya yazma-yok]'
    );
  }
  return (
    <div className="space-y-4" data-testid="eba-paneli">
      <div className="grid md:grid-cols-3 gap-3" data-testid="eba-akis">
        <div className="rounded-xl border border-slate-200 bg-white p-3 text-xs">
          <b>1 · Cihaz (Terminal)</b><br />EBA-UID cihazda maskelenir: ÖĞR-••• · sunucuda açık-metin yok (KVKK-yerel).
        </div>
        <div className="rounded-xl border border-slate-200 bg-white p-3 text-xs">
          <b>2 · daily-insight TASLAĞI</b><br />Yerel-üretim; gözlemlenebilir-sayılabilir dil; kişi-değerlendirmesi yok (K-02).
        </div>
        <div className="rounded-xl border border-emerald-300 bg-emerald-50 p-3 text-xs">
          <b>3 · [EBA POST] /api/v1/report/daily-insight</b><br />
          <span data-testid="eba-yok-rozeti" className="inline-block mt-1 px-2 py-0.5 rounded-full bg-emerald-600 text-white font-bold">PLANLI ENTEGRASYON — bu önizlemede gönderim YOK</span>
        </div>
      </div>

      <div className="flex flex-wrap gap-2 text-[11px]">
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">K-331: salt-okunur çağrı — ödev/içerik yazılmaz</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">e-sınav girişi YOK</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">K-334: idari-mali otomasyon dışarı</span>
        <span className="px-2 py-1 rounded-full bg-slate-100 border border-slate-200">Başarı Notu Yazılmaz · Maskeli UID</span>
      </div>

      <button type="button" data-testid="eba-taslagi-uret" onClick={uret}
        className="px-4 py-2 rounded-xl bg-emerald-600 text-white text-sm font-semibold hover:bg-emerald-700">
        Insight Taslağı Üret (yerel)
      </button>
      {taslak && (
        <textarea data-testid="eba-taslagi" readOnly value={taslak} rows={9}
          className="w-full rounded-xl border border-slate-300 p-3 text-xs font-mono" />
      )}
      <p className="text-[11px] text-slate-500 flex items-center gap-1">
        <ShieldCheck className="w-3.5 h-3.5" /> OAuth 2.0 bağlantısı gerçek-randumda (kurum–MEB sözleşmesi) kurulur;
        bu önizleme sunucusuzdur (K-05) ve hiçbir veri göndermez.
      </p>
    </div>
  );
}

~~~~

### `components/izleme/FrictionMap.tsx`

4020 B · SHA-256 `7eb9534884375219f1fbd6734c51a5240c4753aa9d4a69e03217ca29b8cac3eb`

~~~~tsx
// K-649: SCHOLARIA - Öğrenme Sürtünme Haritası (Learning Friction Map)
// Öğretmen ekranında öğrencilerin zorlanma alanlarını (yanlış/doğru diye değil) 
// başlama, sürdürme ve sonlandırma süreçlerindeki direnç olarak ısı haritasıyla gösterir.

// React importu projede otomatik ekleniyorsa siliyoruz. TS6133
// import React from 'react';

// Persona modülünden (patternStore) aktarılacak olan varsayımsal kanıt verisi
interface OgrenciFrictionVerisi {
  ogrenciAd: string;
  gorevKodu: string;
  baslamaDirenc: 'dusuk' | 'orta' | 'yuksek';
  surdurmeDirenc: 'dusuk' | 'orta' | 'yuksek';
  gecisDirenc: 'dusuk' | 'orta' | 'yuksek';
}

const MOCK_DATA: OgrenciFrictionVerisi[] = [
  { ogrenciAd: 'Ali Y.', gorevKodu: 'MAT-02', baslamaDirenc: 'yuksek', surdurmeDirenc: 'dusuk', gecisDirenc: 'orta' },
  { ogrenciAd: 'Ayşe T.', gorevKodu: 'TR-05', baslamaDirenc: 'dusuk', surdurmeDirenc: 'orta', gecisDirenc: 'dusuk' },
  { ogrenciAd: 'Can B.', gorevKodu: 'MAT-02', baslamaDirenc: 'orta', surdurmeDirenc: 'yuksek', gecisDirenc: 'yuksek' },
];

const getColor = (seviye: string) => {
  switch (seviye) {
    case 'dusuk': return 'bg-green-100 text-green-700'; // Akıcı
    case 'orta': return 'bg-yellow-100 text-yellow-700'; // Gecikmeli
    case 'yuksek': return 'bg-red-100 text-red-700'; // Dirençli (Kopma noktası)
    default: return 'bg-slate-100 text-slate-500';
  }
};

export default function FrictionMap() {
  return (
    <div className="p-5 bg-white rounded-lg shadow border border-slate-200">
      <div className="mb-4 border-b pb-2">
        <h2 className="text-lg font-bold text-slate-800">Öğrenme Sürtünme Haritası (Friction Map)</h2>
        <p className="text-xs text-slate-500">Öğrencilerin görev aşamalarındaki bilişsel dirençlerini ve kopma noktalarını gösterir.</p>
      </div>

      <div className="overflow-x-auto">
        <table className="w-full text-left text-sm">
          <thead>
            <tr className="bg-slate-50 border-b">
              <th className="p-2 font-medium text-slate-600">Öğrenci</th>
              <th className="p-2 font-medium text-slate-600">Görev</th>
              <th className="p-2 font-medium text-slate-600">Başlama Direnci</th>
              <th className="p-2 font-medium text-slate-600">Görev Sürdürme</th>
              <th className="p-2 font-medium text-slate-600">Geçiş / Sonlandırma</th>
            </tr>
          </thead>
          <tbody>
            {MOCK_DATA.map((veri, idx) => (
              <tr key={idx} className="border-b last:border-0 hover:bg-slate-50">
                <td className="p-2 font-medium">{veri.ogrenciAd}</td>
                <td className="p-2 text-slate-500">{veri.gorevKodu}</td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.baslamaDirenc)}`}>
                    {veri.baslamaDirenc.toUpperCase()}
                  </span>
                </td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.surdurmeDirenc)}`}>
                    {veri.surdurmeDirenc.toUpperCase()}
                  </span>
                </td>
                <td className="p-2">
                  <span className={`px-2 py-1 rounded text-xs font-semibold ${getColor(veri.gecisDirenc)}`}>
                    {veri.gecisDirenc.toUpperCase()}
                  </span>
                </td>
              </tr>
            ))}
          </tbody>
        </table>
      </div>
      
      <div className="mt-4 p-3 bg-blue-50 text-blue-800 text-xs rounded border border-blue-200">
        <strong>Eğitsel Çıkarım Örneği:</strong> Ali'nin MAT-02 görevine başlaması çok zor (Yüksek Direnç) ancak başladıktan sonra akıcı bir şekilde bitiriyor (Düşük Sürdürme Direnci). Ali'ye göreve başlarken kısa bir görsel tetikleyici vermek sürtünmeyi (friction) kırabilir.
      </div>
    </div>
  );
}

~~~~

### `components/izleme/IzlemePaneli.tsx`

2509 B · SHA-256 `1cb97d48aefce6d265fb36125e60c6338cab472c2c7f6027be94a2c30c9d3f4e`

~~~~tsx
/**
 * İzleme — d(SDRT)/dt öğrenci-serisi (K-554; PCV-brifing görev-G-izleme).
 * Sentetik-gösterim (K-05); XR/Control-Task Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
 * K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.
 */
import { useState } from 'react';
import { OGRENCILER } from '../../data/mock';
import { sdrtSeri, noktalar } from '../../data/seriler';

export default function IzlemePaneli() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  return (
    <div className="space-y-4" data-testid="izleme-paneli">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>MOCK:</b> seriler sentetik-gösterimdir (K-05); XR/Control-Task Faz-3 PLANLI-katmandır — bu ekranda koşmaz.
      </div>
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <label className="text-xs font-semibold text-slate-700">
          Öğrenci (maskeli):
          <select data-testid="izleme-ogrenci-sec" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)}
            className="ml-2 rounded-lg border border-slate-200 px-2 py-1 text-xs">
            {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
          </select>
        </label>
        <div className="mt-3 grid md:grid-cols-2 gap-4">
          <div>
            <div className="text-xs font-semibold text-slate-700">d(SDRT)/dt — {o.takmaAd} (12 gözlem-noktası)</div>
            <svg width="100%" height={64} viewBox="0 0 280 64" className="mt-1" data-testid="izleme-egri">
              <polyline points={noktalar(sdrtSeri(o.id), 280, 64)} fill="none" stroke="#0ea5e9" strokeWidth="2" />
            </svg>
          </div>
          <div className="text-xs space-y-2">
            <div className="rounded-xl border border-slate-200 p-3">
              <b>Gaze-Lock etkileşim-oranı:</b> %88.4 <span className="text-slate-400">(sentetik-sabit · Faz-3 Control Task-M11)</span>
            </div>
            <div className="rounded-xl border border-slate-200 p-3">
              <b>Aktif görev:</b> {o.aktifGorev} · <b>GFI:</b> {o.gfi.toFixed(2)} · <b>Fslope:</b> {o.fslope.toFixed(2)}
            </div>
            <div className="text-[11px] text-slate-500">K-14: akran-karşılaştırması yok — yalnız öğrencinin kendi-serisi.</div>
          </div>
        </div>
      </div>
    </div>
  );
}

~~~~

### `components/ogretmen/Cockpit.tsx`

4701 B · SHA-256 `df4cd8759dcb30891418fcdfd5c72a59601ceb7da6dba768a2862b57651420aa`

~~~~tsx
/**
 * Öğretmen Paneli (Teacher Cockpit) — K-554 CANLI (PCV-brifing görev-E).
 * Toplu yorgunluk (Fslope) satırları + d(SDRT)/dt sınıf-eğrisi + Nefes Halkası yönlendirme-kartı.
 * Sentetik veri (K-05 MOCK): fslope/GFI değerleri gösterim-verisidir — sensör-akışı DEĞİLDİR;
 * "ölçen değil, gözlemleyen" konumu (K-02): eşik-geçene YÖNLENDİRME-önerisi üretilir, ölçüm/tanı yok.
 */
import { useState } from 'react';
import { GraduationCap, Wind } from 'lucide-react';
import { SINIF_DURUMU } from '../../data/mock';
import { sdrtSeri, noktalar } from '../../data/seriler';

export default function Cockpit({ secSinif }: { secSinif: string }) {
  const [yonlendirildi, setYonlendirildi] = useState(false);
  const durum = SINIF_DURUMU.find((s) => s.sinifId === secSinif);
  const ogrenciler = durum?.ogrenciler ?? [];
  const alarmli = ogrenciler.filter((o) => o.fslope >= 0.07);
  const egri = sdrtSeri('SNF' + secSinif);
  const renk = (f: number) => (f >= 0.07 ? 'bg-rose-500' : f >= 0.05 ? 'bg-amber-500' : 'bg-emerald-500');
  return (
    <div className="space-y-4" data-testid="cockpit">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>MOCK:</b> tüm değerler sentetiktir (K-05) · bu panel ölçüm-arağı değildir; sınıf-içi gözlem için
        yönlendirme-desteğidir (K-02) · eşik-önerisi: Fslope ≥ 0.07 → Nefes Halkası.
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><GraduationCap className="w-4 h-4 text-indigo-600" /> Toplu Yorgunluk (Fslope) — {secSinif}</h3>
        <div className="mt-3 space-y-2" data-testid="cockpit-fsatirlari">
          {ogrenciler.map((o) => (
            <div key={o.id} className="flex items-center gap-2 text-xs">
              <span className="w-16 font-semibold">{o.takmaAd}</span>
              <div className="flex-1 h-3 rounded-full bg-slate-100 overflow-hidden">
                <div className={`h-full ${renk(o.fslope)}`} style={{ width: `${Math.min(100, o.fslope * 900)}%` }} />
              </div>
              <span className="w-24 text-right text-slate-500">Fslope {o.fslope.toFixed(2)}</span>
              <span className="w-20 text-right text-slate-400">GFI {o.gfi.toFixed(2)}</span>
              {o.fslope >= 0.07 && <span className="text-[10px] px-1.5 py-0.5 rounded-full bg-rose-100 text-rose-700 font-bold">yorgunluk-uyarısı</span>}
            </div>
          ))}
        </div>
        <div className="mt-4">
          <div className="text-xs font-semibold text-slate-700">d(SDRT)/dt sınıf-eğrisi (sentetik-gösterim)</div>
          <svg width={280} height={56} className="mt-1" data-testid="cockpit-egri">
            <polyline points={noktalar(egri, 280, 56)} fill="none" stroke="#4f46e5" strokeWidth="2" />
          </svg>
        </div>
      </div>

      <div className="rounded-2xl border border-indigo-200 bg-indigo-50 p-4" data-testid="cockpit-nefes">
        <h3 className="font-bold text-sm flex items-center gap-2"><Wind className="w-4 h-4 text-indigo-600" /> Nefes Halkası (Breathing Circle)</h3>
        <div className="mt-2 flex items-center gap-4">
          <div className="relative w-16 h-16 shrink-0">
            <div className="absolute inset-0 rounded-full bg-indigo-300 animate-ping opacity-60" />
            <div className="absolute inset-2 rounded-full bg-indigo-500 opacity-80" />
          </div>
          <div className="text-xs text-slate-700">
            Kılavuz-tempo: <b>4 sn al — 4 sn tut — 4 sn ver</b> · sınıf-öncesi/arası 2 tur.<br />
            {alarmli.length > 0
              ? <span className="text-rose-700 font-semibold">{alarmli.length} öğrenci eşik-üstü → yönlendirme-önerisi hazır.</span>
              : 'Eşik-üstü öğrenci yok.'}
          </div>
        </div>
        <button type="button" data-testid="cockpit-yonlendir" onClick={() => setYonlendirildi(true)}
          className="mt-3 px-3 py-1.5 rounded-xl bg-indigo-600 text-white text-xs font-semibold hover:bg-indigo-700">
          Yönlendirme-kartı üret
        </button>
        {yonlendirildi && (
          <div className="mt-2 rounded-xl bg-white border border-indigo-200 p-3 text-xs" data-testid="cockpit-yonlendirme-karti">
            <b>{secSinif} — gözlem-notu (MOCK):</b> {alarmli.length > 0 ? alarmli.map((a) => a.takmaAd).join(', ') : 'sınıf-geneli'} için
            Nefes Halkası-tempo (4-4-4) denenebilir. Bu kart cihaza komut GÖNDERMEZ; öğretmen-sözüyle yürütülür.
          </div>
        )}
      </div>
    </div>
  );
}

~~~~

### `components/ogretmen/TransferGozlemKarti.tsx`

6843 B · SHA-256 `054db5d944b131928f7d4ce02d5f858316d58b057f946d86fe2a5be342ecfd60`

~~~~tsx
/**
 * H(c) — Transfer Gözlem Kartı MOCK (öğretmen formu) · K-451 (P/S kod turu ②)
 * Yerleşim Taslağı v1.0 §3-14: ≤30 sn tek ekran; 3'lü Likert YERİNE davranışsal giriş;
 * sentetik/yerel-önce (K-05). Kişi değerlendirmesi YOK — yalnız gözlenen davranış kaydı (K-02).
 */
import { useEffect, useState } from 'react';
import { ClipboardCheck, Save, Trash2 } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020';

// Davranış anahtarları (Likert değil; "gözlendi / gözlenmedi" girişi)
const DAVRANISLAR = [
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
] as const;

interface HcKayit {
  id: string;
  ogrenci: string;
  gorev: string;
  davranislar: number[];
  not: string;
  zaman: string;
}

function kayitlariOku(): HcKayit[] {
  try {
    return JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[];
  } catch {
    return [];
  }
}

export default function TransferGozlemKarti() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [gorev, setGorev] = useState(GOREVLER[0].id);
  const [secili, setSecili] = useState<number[]>([]);
  const [not, setNot] = useState('');
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);

  useEffect(() => { setKayitlar(kayitlariOku()); }, []);

  function davranisDegistir(i: number) {
    setSecili(oncesi => oncesi.includes(i) ? oncesi.filter(x => x !== i) : [...oncesi, i]);
  }

  function kaydet() {
    const o = OGRENCILER.find(x => x.id === ogrenci);
    const g = GOREVLER.find(x => x.id === gorev);
    const yeni: HcKayit = {
      id: 'HC-' + Date.now(),
      ogrenci: o ? o.takmaAd : ogrenci,
      gorev: g ? g.baslik : gorev,
      davranislar: secili,
      not: not.trim(),
      zaman: new Date().toLocaleString('tr-TR'),
    };
    const guncel = [yeni, ...kayitlar].slice(0, 20);
    localStorage.setItem(ANAHTAR, JSON.stringify(guncel));
    setKayitlar(guncel);
    setSecili([]); setNot('');
  }

  function hepsiniSil() {
    localStorage.removeItem(ANAHTAR);
    setKayitlar([]);
  }

  return (
    <div data-testid="hc-kart" className="space-y-3 max-w-2xl">
      <div className="flex items-center gap-3">
        <div className="w-10 h-10 rounded-xl bg-indigo-100 grid place-items-center">
          <ClipboardCheck size={20} className="text-indigo-700" />
        </div>
        <div>
          <h2 className="font-bold">Transfer Gözlem Kartı</h2>
          <p className="text-xs text-slate-500 mb-4">Öğrencinin sınıf içi beceri transferini ve yönergelere uyumunu hızla kaydedebileceğiniz gözlem formu.</p>
          <p className="text-xs text-slate-500">
            Sınıfta kazanılan becerinin günlük derse taşınması — 30 saniyelik davranış kaydı.
            Değerlendirme değildir; gözlem kayıtlar. Veri bu cihazda kalır (yerel-önce).
          </p>
        </div>
      </div>

      <div className="bg-amber-50 border border-amber-200 rounded-lg px-3 py-1.5 text-[11px] font-semibold text-amber-800" data-testid="hc-mock-rozet">
        MOCK — sentetik öğrenci/görev verisiyle demo (K-05); gerçek gözlem akışı pilot fazında
      </div>

      <div className="grid grid-cols-2 gap-2">
        <label className="text-xs font-semibold text-slate-700">
          Öğrenci (sentetik):
          <select data-testid="hc-ogrenci-sec" value={ogrenci} onChange={e => setOgrenci(e.target.value)}
            className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs">
            {OGRENCILER.map(o => <option key={o.id} value={o.id}>{o.takmaAd} ({o.id})</option>)}
          </select>
        </label>
        <label className="text-xs font-semibold text-slate-700">
          Gözlenen etkinlik:
          <select data-testid="hc-gorev-sec" value={gorev} onChange={e => setGorev(e.target.value)}
            className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs">
            {GOREVLER.map(g => <option key={g.id} value={g.id}>{g.baslik}</option>)}
          </select>
        </label>
      </div>

      <div className="space-y-1.5">
        <div className="text-xs font-semibold text-slate-700">Gözlenen davranışlar (işaretleyerek):</div>
        {DAVRANISLAR.map((d, i) => {
          const akt = secili.includes(i);
          return (
            <button key={i} type="button" data-testid={`hc-davranis-${i}`} onClick={() => davranisDegistir(i)}
              className={`w-full text-left px-3 py-2 rounded-xl border text-xs transition-colors ${
                akt ? 'bg-indigo-600 text-white border-indigo-600 font-semibold'
                    : 'bg-white text-slate-700 border-slate-200 hover:bg-slate-50'}`}>
              {akt ? '✓ ' : '○ '}{d}
            </button>
          );
        })}
      </div>

      <label className="block text-xs font-semibold text-slate-700">
        Kısa not (isteğe bağlı):
        <input data-testid="hc-not" value={not} maxLength={140} onChange={e => setNot(e.target.value)}
          placeholder="Örn. tahta örneğinden sonra kendi uygulamasına geçti"
          className="mt-1 w-full rounded-lg border border-slate-200 bg-white px-2 py-1.5 text-xs" />
      </label>

      <div className="flex items-center gap-2">
        <button type="button" data-testid="hc-kaydet" onClick={kaydet}
          className="inline-flex items-center gap-1.5 bg-indigo-600 text-white text-xs font-semibold px-4 py-2 rounded-xl hover:bg-indigo-700">
          <Save size={14} /> Kaydet (yerel)
        </button>
        <span data-testid="hc-kayit-sayisi" className="text-[11px] text-slate-500">
          {kayitlar.length} kayıt · yalnız bu tarayıcıda
        </span>
      </div>

      {kayitlar.length > 0 && (
        <div className="space-y-1.5">
          <div className="flex items-center justify-between">
            <div className="text-xs font-semibold text-slate-700">Son kayıtlar:</div>
            <button type="button" data-testid="hc-temizle" onClick={hepsiniSil}
              className="inline-flex items-center gap-1 text-[11px] text-slate-400 hover:text-red-500">
              <Trash2 size={12} /> hepsini temizle
            </button>
          </div>
          {kayitlar.slice(0, 5).map((k, i) => (
            <div key={k.id} data-testid={`hc-kayit-${i}`}
              className="border border-slate-200 rounded-lg px-3 py-2 text-[11px] bg-white">
              <b>{k.ogrenci}</b> · {k.gorev} · {k.davranislar.length} davranış
              {k.not ? ` · “${k.not}”` : ''} <span className="text-slate-400">({k.zaman})</span>
            </div>
          ))}
        </div>
      )}
    </div>
  );
}

~~~~

### `components/portfoy/Portfoy.tsx`

4755 B · SHA-256 `c23e69cb4b94a5575387d684c36edddcdf0f3f2a916c2861a0ea2bdd64c07b1e`

~~~~tsx
/**
 * ÖĞRENCİ DEFTERİ — yazılı-portfolyo (K-559 · Yol-3; Seesaw-deseninin K-05-metin-yalnız uyarlaması).
 * 4-yerel-defteri (H-c gözlem · atama · BEP-probe · sonuç-notu) SALT-OKUNUR birleştirip
 * öğrenci-bazlı zaman-çizelgesi sunar. Görüntü/ses-yükleme YOK; yazdırma/dışa-aktarım YOK
 * (PCV-kural-1); gerçek-rapor-çıktısı planlı-katmandır. Kimlik: yalnız maskeli-takma-ad (K-05).
 */
import { useEffect, useState } from 'react';
import { FolderOpen } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';

const KAYNAKLAR = [
  { anahtar: 'scholaria_hc_kayitlar_v020', ad: 'Gözlem-kartı (H-c)' },
  { anahtar: 'scholaria_atama_defteri_v023', ad: 'Görev-ataması' },
  { anahtar: 'scholaria_bep_defteri_v024', ad: 'BEP-hazırlık' },
  { anahtar: 'scholaria_sonuc_notu_v023', ad: 'Sonuç-notu' },
] as const;

interface Satir { kaynak: string; zaman: string; metin: string }

function topla(ogrenci: string): Satir[] {
  const satirlar: Satir[] = [];
  function ekle(anahtar: string, ad: string, sec: (r: Record<string, unknown>) => { zaman: string; metin: string } | null) {
    try {
      const liste = JSON.parse(localStorage.getItem(anahtar) ?? '[]') as Array<Record<string, unknown>>;
      liste.filter((r) => !r.ogrenci || r.ogrenci === ogrenci).forEach((r) => {
        const s = sec(r);
        if (s) satirlar.push({ kaynak: ad, zaman: s.zaman, metin: s.metin });
      });
    } catch { /* yerel-okuma-hatası — yoksay */ }
  }
  ekle(KAYNAKLAR[0].anahtar, KAYNAKLAR[0].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `${r.gorev ?? 'görev'}: ${(r.davranislar as number[] | undefined)?.length ?? 0} davranış-gözlemi${r.not ? ` · "${String(r.not)}"` : ''}`,
  }));
  ekle(KAYNAKLAR[1].anahtar, KAYNAKLAR[1].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `etkinlik atandı: ${r.etkinlik ?? ''} · kazanım ${r.kazanımKod ?? r.kazanimKod ?? ''}`,
  }));
  ekle(KAYNAKLAR[2].anahtar, KAYNAKLAR[2].ad, (r) => ({
    zaman: '—', metin: `BEP-hazırlık hedefi (${r.kazanımKod ?? r.kazanimKod ?? ''}) · ${(r.probe as unknown[] | undefined)?.length ?? 0} haftalık-probu`,
  }));
  ekle(KAYNAKLAR[3].anahtar, KAYNAKLAR[3].ad, (r) => ({
    zaman: String(r.zaman ?? ''), metin: `sonuç-notu: "${String(r.metin ?? '')}"`,
  }));
  return satirlar.sort((a, b) => b.zaman.localeCompare(a.zaman));
}

export default function Portfoy() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [satirlar, setSatirlar] = useState<Satir[]>([]);
  const [taze, setTaze] = useState(0);
  useEffect(() => { setSatirlar(topla(ogrenci)); }, [ogrenci, taze]);

  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="portfoy">
      <h3 className="font-bold text-sm flex items-center gap-2"><FolderOpen className="w-4 h-4 text-indigo-600" /> Öğrenci Defteri — yazılı-portfolyo</h3>
      <div className="mt-2 flex flex-wrap gap-2 items-center text-xs">
        <label className="font-semibold text-slate-700">Öğrenci:
          <select data-testid="portfoy-ogrenci" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="ml-2 rounded-lg border border-slate-200 px-2 py-1">
            {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
          </select>
        </label>
        <button type="button" data-testid="portfoy-tazele" onClick={() => setTaze((t) => t + 1)} className="px-3 py-1.5 rounded-xl bg-indigo-600 text-white font-semibold">Defterleri tara</button>
        <span className="text-[11px] text-slate-500">{satirlar.length} kayıt · 4-defter salt-okunur</span>
      </div>
      {satirlar.length === 0 ? (
        <p className="text-sm text-slate-500 mt-2" data-testid="portfoy-bos">Defterler boş — H-c kartı doldurdukça / atama işledikçe bu manzara dolar.</p>
      ) : (
        <div className="mt-3 space-y-1.5" data-testid="portfoy-zaman-cizelgesi">
          {satirlar.slice(0, 14).map((s, i) => (
            <div key={i} className="text-xs rounded-xl border border-slate-200 px-3 py-2">
              <span className="inline-block text-[10px] font-bold px-1.5 py-0.5 rounded-full bg-slate-100 text-slate-600 mr-2">{s.kaynak}</span>
              <span className="text-slate-400 text-[10px] mr-2">{s.zaman ? s.zaman.slice(0, 10) : ''}</span>
              {s.metin}
            </div>
          ))}
        </div>
      )}
      <p className="text-[11px] text-slate-500 mt-2">
        Metin-yalnız portfolyo (K-05: görüntü/ses yüklenmez, hiçbir şey ağa gitmez); veli-manzarası bülten-taslağıyla
        bütünleşiktir (Aile Bilgilendirme). Yazdırma/dışa-aktarım bu önizlemede YOK (PCV-kural-1).
      </p>
    </div>
  );
}

~~~~

### `components/rapor/RaporOzeti.tsx`

3034 B · SHA-256 `116a78db9a529d4f59a515c252dc084a4ceca28554f0315565ab88b6059eadc8`

~~~~tsx
/**
 * Rapor — Günlük Ev–Okul gözlem-notu ÖNİZLEMESİ (K-554; PCV-brifing görev-H).
 * H(c) Transfer-kayıtlarından (localStorage, salt-okunur) gözlemlenebilir-sayılabilir dil üretir.
 * Bu ekranda yazdırma/dışa-aktarım YOKTUR (PCV-kural-1); gerçek-rapor-çıktısı planlı-katmandır.
 */
import { useEffect, useState } from 'react';
import { FileText } from 'lucide-react';
import { OGRENCILER, GOREVLER } from '../../data/mock';

const ANAHTAR = 'scholaria_hc_kayitlar_v020'; // TransferGozlemKarti deposu — salt-okunur
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

const DAVRANISLAR = [ // TransferGozlemKarti listesiyle aynıdır (kaynak-orası; burada salt-okunur gösterim)
  'Göreve kendi başladı (yönlendirme olmadan)',
  'Zorlanınca ipucu istedi ve sürdürdü',
  'Mola verdi ve döndü (akışı korudu)',
  'Sözel yönerge tek başına yeterli oldu',
];

export default function RaporOzeti() {
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);
  useEffect(() => {
    try { setKayitlar(JSON.parse(localStorage.getItem(ANAHTAR) ?? '[]') as HcKayit[]); } catch { setKayitlar([]); }
  }, []);
  const notlar = kayitlar.slice(0, 8).map((k) => {
    const o = OGRENCILER.find((x) => x.id === k.ogrenci);
    const g = GOREVLER.find((x) => x.id === k.gorev);
    const d = k.davranislar?.map((i) => `"${DAVRANISLAR[i] ?? 'gözlem'}"`).join(', ');
    return `• ${o?.takmaAd ?? '•••'} — ${g?.baslik ?? 'görev'}: ${d || 'gözlem-girişi yok'}${k.not ? `; öğretmen-notu: "${k.not}"` : ''}. (${k.zaman?.slice(0, 10) ?? ''})`;
  });
  return (
    <div className="space-y-4" data-testid="rapor-ozeti">
      <div className="bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-[11px] text-slate-600">
        <b>Görev-H deseni:</b> "40 dk derste 3 kez yerinden kalktı" tipi <b>gözlemlenebilir-sayılabilir dil</b>.
        Bu önizleme kaydetmez/yazdırmaz (PCV-kural-1 · yerel-yalnız); gerçek-rapor-çıktısı planlı-katmandır.
      </div>
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><FileText className="w-4 h-4 text-indigo-600" /> Günün Ev–Okul Notu Taslağı (H-c kaynaklı)</h3>
        {notlar.length === 0 ? (
          <p className="text-sm text-slate-500 mt-2" data-testid="rapor-bos">
            Henüz H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından 1 kart doldurun; bu not-önizlemesi o kayıttan üretilir.
          </p>
        ) : (
          <textarea readOnly rows={7} value={notlar.join('\n')} data-testid="rapor-not-ornegi"
            className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-xs font-mono" />
        )}
        <p className="text-[11px] text-slate-500 mt-2">
          Tanı/değerlendirme-yargısı İÇERMEZ (K-02); veli-görüşme-çıktısı planlı-katmanda TASLAK mührüyle üretilir.
        </p>
      </div>
    </div>
  );
}

~~~~

### `components/ses/SesPaneli.tsx`

2419 B · SHA-256 `7f48dcf19642652e6c0e4341228679b96fb6972fa2264d0226281932f5505fd6`

~~~~tsx
/**
 * Ses Ortamı Yönetimi — ana-sinyal izolasyonu GÖRSEL-simülasyonu (K-554; PCV-brifing görev-G).
 * Bu önizlemede ses-işleme/donanım YOKTUR (planlı-katman): dalga-grafiği sentetik-gösterimdir (K-05/K-02).
 */
import { useState } from 'react';
import { noktalar } from '../../data/seriler';

const ANA = noktalar(Array.from({ length: 48 }, (_, i) => 0.5 + 0.32 * Math.sin(i * 0.55)), 480, 80);
const GURULTU = noktalar(Array.from({ length: 48 }, (_, i) => 0.5 + 0.3 * Math.sin(i * 2.3) * (0.4 + 0.6 * Math.abs(Math.sin(i * 0.9)))), 480, 80);

export default function SesPaneli() {
  const [izolasyon, setIzolasyon] = useState(60);
  return (
    <div className="space-y-4" data-testid="ses-paneli">
      <div className="bg-amber-50 border border-amber-200 rounded-xl px-3 py-2 text-[11px] text-amber-900" data-testid="ses-planli">
        <b>PLANLI-KATMAN şerhi:</b> donanımsal matris-filtresi bu önizlemede YOK — burada yalnızca ana-sinyal/gürültü
        ayrımının <b>görsel-simülasyonu</b> vardır (K-02: algı-iddiası kurulmaz · K-05: sentetik).
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm">Ana Sinyal İzolasyonu — {izolasyon}%</h3>
        <input type="range" min={0} max={100} value={izolasyon} data-testid="ses-slider"
          onChange={(e) => setIzolasyon(Number(e.target.value))} className="w-full mt-2" />
        <svg width="100%" height={80} viewBox="0 0 480 80" className="mt-2 bg-slate-50 rounded-xl" data-testid="ses-dalga">
          <polyline points={GURULTU} fill="none" stroke="#f59e0b" strokeWidth="1.5" opacity={Math.max(0.06, 1 - izolasyon / 100)} />
          <polyline points={ANA} fill="none" stroke="#4f46e5" strokeWidth="2" />
        </svg>
        <div className="flex gap-3 mt-2 text-[11px] text-slate-600">
          <span className="flex items-center gap-1"><span className="w-3 h-0.5 bg-indigo-600 inline-block" /> ana-sinyal</span>
          <span className="flex items-center gap-1"><span className="w-3 h-0.5 bg-amber-500 inline-block" /> ortam-gürültüsü (izolasyon-arttıkça söner)</span>
        </div>
      </div>

      <label className="flex items-center gap-2 text-xs text-slate-600">
        <input type="checkbox" disabled /> Donanımsal matris-filtresi (planlı-katman — kurum-donanımıyla birlikte açılır)
      </label>
    </div>
  );
}

~~~~

### `components/shell/Kabuk.tsx`

3209 B · SHA-256 `d2ab731e07cd2cf4ea63261fd807361b3816a4119ccc7dc89dcac6aef95a1b2f`

~~~~tsx
/** SCHOLARIA kabuğu: B2B sınıf düğümü. Kurumsal panel; öğrenci/öğretmen/sınıf/yönetici rolleri. */
import type { ReactNode } from 'react';
import { LayoutDashboard, Users, GraduationCap, FileText, Settings, Activity, Database, ShieldCheck, HelpCircle, BarChart3, ClipboardCheck, BookOpen, HeartHandshake, Target } from 'lucide-react';

export const EKRANLAR = [
  { id: 'pano', ad: 'Sınıf Özeti', ikon: LayoutDashboard },
  { id: 'sinif', ad: 'Sınıf', ikon: Activity },
  { id: 'ogrenci', ad: 'Öğrenci', ikon: Users },
  { id: 'ogretmen', ad: 'Öğretmen', ikon: GraduationCap },
  { id: 'transfer', ad: 'Transfer Gözlem Kartı', ikon: ClipboardCheck },
  { id: 'ders', ad: 'Ders & Görev', ikon: BookOpen },
  { id: 'veli', ad: 'Aile Bilgilendirme', ikon: HeartHandshake },
  { id: 'bep', ad: 'BEP Hazırlık', ikon: Target },
  { id: 'eba', ad: 'MEB EBA Entegrasyonu', ikon: Database },
  { id: 'izleme', ad: 'Gelişim Takibi', ikon: BarChart3 },
  { id: 'ses', ad: 'Sınıf İçi Ses Yönetimi', ikon: ShieldCheck },
  { id: 'rapor', ad: 'Rapor', ikon: FileText },
  { id: 'ayarlar', ad: 'Ayarlar', ikon: Settings },
  { id: 'yardim', ad: 'Sistem Kılavuzu ve Terimler', ikon: HelpCircle },
] as const;
export type EkranId = (typeof EKRANLAR)[number]['id'];

export default function Kabuk({ ekran, setEkran, rol, children }:
  { ekran: EkranId; setEkran: (e: EkranId) => void; rol: string; children: ReactNode }) {
  return (
    <div className="min-h-screen flex">
      <aside className="w-60 bg-white border-r border-slate-200 flex flex-col shrink-0">
        <div className="px-4 py-4 border-b border-slate-100">
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 rounded-xl bg-indigo-600 text-white grid place-items-center font-black">S</div>
            <div>
              <div className="font-bold text-sm">SEDUVA Scholaria™</div>
              <div className="text-[10px] text-slate-500">School Node · v{__SURUM__}</div>
            </div>
          </div>
        </div>
        <nav className="flex-1 p-2 space-y-0.5">
          {EKRANLAR.map((e) => {
            const I = e.ikon; const akt = ekran === e.id;
            return (
              <button key={e.id} type="button" data-testid={`nav-${e.id}`} onClick={() => setEkran(e.id)}
                className={`w-full flex items-center gap-2 px-3 py-2 rounded-xl text-sm transition-colors ${
                  akt ? 'bg-indigo-600 text-white font-semibold' : 'text-slate-700 hover:bg-slate-100'}`}>
                <I className="w-4 h-4" /> {e.ad}
              </button>
            );
          })}
        </nav>
        <div className="p-3 border-t border-slate-100 text-[10px] text-slate-500">
          Rol: <b>{rol}</b> · B2B Sınıf Düğümü (School Node)
        </div>
      </aside>
      <main className="flex-1 min-w-0">
        <div className="bg-white border-b border-slate-200 px-6 py-2">
          <p className="text-[11px] text-slate-600"><b>SEDUVA Scholaria:</b> Toplu sınıf içi dikkat ve yürütücü işlev kalibrasyon sistemi (B2B).</p>
        </div>
        <div className="p-6 space-y-5 max-w-6xl">{children}</div>
      </main>
    </div>
  );
}

~~~~

### `components/takip/GelisimTakibi.tsx`

3140 B · SHA-256 `92609adabdfbeb7080400fc6301a0900afb5dd2968a285a4edf31d810b532a13`

~~~~tsx
/**
 * GELİŞİM-TAKİBİ (K-555-3) — "gözlem-takibi" (performans-iddiası DİLİ YOK, K-02/K-04):
 * öğrenci-bazlı H-c kayıt-zaman-çizelgesi (salt-okunur) + MOCK GFI/Fslope serisi (K-05).
 * İzleme ekranına gömülü çalışır.
 */
import { useEffect, useState } from 'react';
import { TrendingUp } from 'lucide-react';
import { OGRENCILER } from '../../data/mock';
import { sdrtSeri, noktalar } from '../../data/seriler';

const HC = 'scholaria_hc_kayitlar_v020';
interface HcKayit { id: string; ogrenci: string; gorev: string; davranislar: number[]; not: string; zaman: string }

export default function GelisimTakibi() {
  const [ogrenci, setOgrenci] = useState(OGRENCILER[0].id);
  const [kayitlar, setKayitlar] = useState<HcKayit[]>([]);
  useEffect(() => {
    try { setKayitlar(JSON.parse(localStorage.getItem(HC) ?? '[]') as HcKayit[]); } catch { setKayitlar([]); }
  }, []);
  const benim = kayitlar.filter((k) => k.ogrenci === ogrenci);
  const o = OGRENCILER.find((x) => x.id === ogrenci)!;
  return (
    <div className="rounded-2xl border border-slate-200 bg-white p-4" data-testid="gelisim-takibi">
      <h3 className="font-bold text-sm flex items-center gap-2"><TrendingUp className="w-4 h-4 text-sky-600" /> Gelişim-takibi (gözlem-çizelgesi) — {o.takmaAd}</h3>
      <label className="text-xs font-semibold text-slate-700 mt-2 inline-block">
        Öğrenci:
        <select data-testid="takip-ogrenci-sec" value={ogrenci} onChange={(e) => setOgrenci(e.target.value)} className="ml-2 rounded-lg border border-slate-200 px-2 py-1 text-xs">
          {OGRENCILER.map((x) => <option key={x.id} value={x.id}>{x.takmaAd} ({x.id})</option>)}
        </select>
      </label>
      <div className="mt-3 grid md:grid-cols-2 gap-4">
        <div>
          <div className="text-xs font-semibold text-slate-700">GFI/Fslope serisi (MOCK-gösterim)</div>
          <svg width="100%" height={56} viewBox="0 0 280 56" className="mt-1" data-testid="takip-seri">
            <polyline points={noktalar(sdrtSeri(o.id), 280, 56)} fill="none" stroke="#0284c7" strokeWidth="2" />
          </svg>
          <div className="text-[11px] text-slate-500">Bu seride "yükseliş/düşüş yorumu" YAPILMAZ — gösterim-dir (K-02/K-04).</div>
        </div>
        <div>
          <div className="text-xs font-semibold text-slate-700">H-c gözlem-zaman-çizelgesi ({benim.length} kayıt)</div>
          {benim.length === 0 ? (
            <p className="text-xs text-slate-500 mt-1" data-testid="takip-bos">Bu-öğrenci için H-c kaydı yok — "Transfer Gözlem (H-c)" ekranından kart doldurun.</p>
          ) : (
            <div className="mt-1 space-y-1">
              {benim.slice(0, 5).map((k) => (
                <div key={k.id} data-testid="takip-satiri" className="text-[11px] rounded-lg border border-slate-200 px-2 py-1">
                  {k.zaman?.slice(0, 10)} · {k.davranislar?.length ?? 0} davranış-gözlemi{k.not ? ` · "${k.not.slice(0, 30)}${k.not.length > 30 ? '…' : ''}"` : ''}
                </div>
              ))}
            </div>
          )}
        </div>
      </div>
    </div>
  );
}

~~~~

### `components/veli/VeliKoprusu.tsx`

7115 B · SHA-256 `5f5c9aab8a91dbbd75d5adad29f43a2d2082376d6b18fb3eb5ae7862dce045d2`

~~~~tsx
/**
 * VELİ KÖPRÜSÜ (K-555-6/7): ① haftalık aile-bilgilendirme BÜLTENİ TASLAĞI (sınıf-geneli gözlem-dili +
 * genel-öneriler; aile-EĞİTİMİ içeriği SUPPORTA'dadır — buradan yönlendirilir) ② veli görüşme-RANDEVU
 * DEFTERİ (yerel; SMS/hatırlatma-otomasyonu YOK — K-334; MENTORIA-SMS ayrı-rol).
 */
import { useEffect, useState } from 'react';
import { CalendarClock, Home } from 'lucide-react';
import { SINIF_DURUMU } from '../../data/mock';

const RANDEVU = 'scholaria_veli_randevu_v023';
const HC = 'scholaria_hc_kayitlar_v020';
interface Randevu { id: string; tarih: string; saat: string; konu: string; not: string; durum: 'planlandı' | 'gerçekleşti' | 'ertelendi' }

const ONERILER = [
  'Eve dönüşte gün-içi bir gözlemi tek-cümleyle paylaşın ("bugün görevine kendi başladı").',
  'Ödevi tek-seferde değil, 10 dakikalık iki-bölüm olarak planlayın.',
  'Ekran-öncesi kısa nefes-rutini (4-4-4) birlikte deneyin.',
  'Talimatları tek-tek ve sırayla verin; tamamlanınca sözel takdir edin.',
  'Uyku ve oyun-düzeni gözlem-notlarını hafta-sonu karşılaştırın.',
];

function oku(): Randevu[] { try { return JSON.parse(localStorage.getItem(RANDEVU) ?? '[]') as Randevu[]; } catch { return []; } }

export default function VeliKoprusu() {
  const [sinif, setSinif] = useState('2A');
  const [bulten, setBulten] = useState<string | null>(null);
  const [randevular, setRandevular] = useState<Randevu[]>(() => oku());
  const [tarih, setTarih] = useState(new Date().toISOString().slice(0, 10));
  const [saat, setSaat] = useState('16:30');
  const [konu, setKonu] = useState('Haftalık gözlem paylaşımı');
  const [not, setNot] = useState('');

  useEffect(() => { try { localStorage.setItem(RANDEVU, JSON.stringify(randevular)); } catch { /* yerel-yalnız */ } }, [randevular]);

  function bultenUret() {
    const d = SINIF_DURUMU.find((x) => x.sinifId === sinif);
    let hc = 0; try { hc = (JSON.parse(localStorage.getItem(HC) ?? '[]') as unknown[]).length; } catch { hc = 0; }
    setBulten(
      `HAFTALIK SINIF BÜLTENİ — TASLAK (yerel-üretim; gönderilmez)\nSınıf: ${sinif} · Tarih: ${new Date().toISOString().slice(0, 10)}\n\n` +
      `Sınıf-gözlemi (MOCK): öğrenci ${d?.ogrenciler.length ?? 0} · ort. Fslope ${(d?.ortalamaFslope ?? 0).toFixed(2)} · son-alarm: ${d?.sonAlarm ?? '—'} · bu-hafta ${hc} gözlem-kartı (H-c).\n\n` +
      `Bu haftanın genel-önerileri (sınıf-geneli; kişi-değerlendirmesi yok — K-02):\n` +
      ONERILER.map((o, i) => `${i + 1}. ${o}`).join('\n') +
      `\n\nAile-EĞİTİMİ programı ve kişiye-özel içerik SUPPORTA ürünündedir; bu bülten yalnız bilgilendirme-notudur.`
    );
  }

  function randevuEkle() {
    const r: Randevu = { id: Math.random().toString(36).slice(2, 9), tarih, saat, konu, not, durum: 'planlandı' };
    setRandevular((p) => [r, ...p]); setNot('');
  }
  function durumDegistir(id: string) {
    setRandevular((p) => p.map((r) => r.id === id ? { ...r, durum: r.durum === 'planlandı' ? 'gerçekleşti' : r.durum === 'gerçekleşti' ? 'ertelendi' : 'planlandı' } : r));
  }

  return (
    <div className="space-y-4" data-testid="veli-koprusu">
      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><Home className="w-4 h-4 text-indigo-600" /> Haftalık Aile Bülteni — TASLAK</h3>
        <div className="mt-2 flex flex-wrap gap-2 items-center text-xs">
          <select data-testid="bulten-sinif" value={sinif} onChange={(e) => setSinif(e.target.value)} className="rounded-lg border border-slate-200 px-2 py-1">
            {SINIF_DURUMU.map((s) => <option key={s.sinifId} value={s.sinifId}>{s.sinifId}</option>)}
          </select>
          <button type="button" data-testid="bulten-uret" onClick={bultenUret} className="px-3 py-1.5 rounded-xl bg-indigo-600 text-white font-semibold hover:bg-indigo-700">Bülten taslağı üret</button>
        </div>
        {bulten && <textarea readOnly rows={9} value={bulten} data-testid="bulten-taslagi" className="w-full mt-2 rounded-xl border border-slate-300 p-3 text-xs font-mono" />}
        <p className="text-[11px] text-slate-500 mt-1">Gözlemlenebilir-sayılabilir dil (K-14); tanı/yargı yok (K-02). Aile-eğitimi içeriği SUPPORTA'dadır.</p>
      </div>

      <div className="rounded-2xl border border-slate-200 bg-white p-4">
        <h3 className="font-bold text-sm flex items-center gap-2"><CalendarClock className="w-4 h-4 text-indigo-600" /> Veli Görüşme — Randevu Defteri</h3>
        <div className="mt-2 grid md:grid-cols-4 gap-2 text-xs">
          <input type="date" data-testid="randevu-tarih" value={tarih} onChange={(e) => setTarih(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5" />
          <input type="time" data-testid="randevu-saat" value={saat} onChange={(e) => setSaat(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5" />
          <select data-testid="randevu-konu" value={konu} onChange={(e) => setKonu(e.target.value)} className="rounded-lg border border-slate-300 px-2 py-1.5">
            <option>Haftalık gözlem paylaşımı</option>
            <option>H-c kart-turu değerlendirme paylaşımı</option>
            <option>Gelişim-görüşmesi (gözlem-özetli)</option>
            <option>Diğer</option>
          </select>
          <input data-testid="randevu-not" value={not} onChange={(e) => setNot(e.target.value)} placeholder="görüşme-notu (isteğe bağlı)" className="rounded-lg border border-slate-300 px-2 py-1.5" />
        </div>
        <button type="button" data-testid="randevu-ekle" onClick={randevuEkle} className="mt-2 px-3 py-1.5 rounded-xl bg-indigo-600 text-white text-xs font-semibold hover:bg-indigo-700">Randevu kaydet</button>
        <div className="mt-3 space-y-1.5">
          {randevular.length === 0 ? (
            <p className="text-sm text-slate-500" data-testid="randevu-bos">Defter boş — randevu kaydedin.</p>
          ) : randevular.slice(0, 8).map((r) => (
            <div key={r.id} data-testid="randevu-satiri" className="flex items-center gap-2 text-xs rounded-xl border border-slate-200 px-3 py-2">
              <span className="font-semibold">{r.tarih} {r.saat}</span>
              <span className="text-slate-600">{r.konu}</span>
              {r.not && <span className="text-slate-400">· {r.not}</span>}
              <button type="button" onClick={() => durumDegistir(r.id)}
                className={`ml-auto px-2 py-0.5 rounded-full text-[10px] font-bold ${r.durum === 'planlandı' ? 'bg-amber-100 text-amber-700' : r.durum === 'gerçekleşti' ? 'bg-emerald-100 text-emerald-700' : 'bg-slate-100 text-slate-500'}`}>
                {r.durum}
              </button>
            </div>
          ))}
        </div>
        <p className="text-[11px] text-slate-500 mt-2">Yerel-defter (K-05); SMS/hatırlatma-otomasyonu YOK (K-334). Durum-etiketine tıklayınca döner: planlandı → gerçekleşti → ertelendi.</p>
      </div>
    </div>
  );
}

~~~~

### `data/kisitlar.ts`

470 B · SHA-256 `ffdee27378e251b0da741803394d6b4e31163e1b5e2bd443698cc8bbd7cc017f`

~~~~tsx
// VAMOLA EduLabs Scholaria v0.1.0 — Kısıtlar (K-334 idari-mali dışarı, MEB salt okunur)

export const KISITLAR = {
  idariMaliKapsamDisi: true, // K-334: e-fatura/MEBBİS/BKDS yok
  mebEbaSaltOkunur: true, // K-331: ödevler ve içerik sadece çağrılır, yazılmaz
  kvkkYerelMaskeleme: true, // EBA UID'ler cihazda maskelenir, sunucuda açık metin yok
  telifiSifir: true, // Ölçekler/MEB müfredatı paket içinde yer almaz
  surum: 'v0.1.0',
} as const;

~~~~

### `data/mock.ts`

1600 B · SHA-256 `5448f2287eb7aba775c98a6d0fd34dd9d7edda825f367acc9c2c995b5a11bce9`

~~~~tsx
// VAMOLA EduLabs Scholaria v0.1.0 — Mock Veri (K-05 ÖĞR-xxxx, gerçek veri yok)
import { Ogrenci, Sube, Gorev, SinifDurumu } from '../types';

export const SUBELER: Sube[] = [
  { id: 'SUB-2A', ad: '2. Sınıf A Şubesi', ogrenciSayisi: 24 },
  { id: 'SUB-2B', ad: '2. Sınıf B Şubesi', ogrenciSayisi: 22 },
  { id: 'SUB-4A', ad: '4. Sınıf A Şubesi', ogrenciSayisi: 25 },
];

export const GOREVLER: Gorev[] = [
  { id: 'PVC-101', baslik: 'Görsel Dikkat: Renk Eşleştirme', dersId: 'MAT-2', modul: 'M1' },
  { id: 'PVC-102', baslik: 'Motivasyon: Zaman Farkındalığı', dersId: 'HKM-2', modul: 'M2' },
  { id: 'PVC-103', baslik: 'Bölünmüş Dikkat: Çift Görev', dersId: 'TUR-2', modul: 'M3' },
];

export const OGRENCILER: Ogrenci[] = [
  { id: 'OGR-101', takmaAd: 'ARD-05', subeId: 'SUB-2A', gfi: 0.82, fslope: 0.03, aktifGorev: 'PVC-101' },
  { id: 'OGR-102', takmaAd: 'ARD-06', subeId: 'SUB-2A', gfi: 0.75, fslope: 0.05, aktifGorev: 'PVC-102' },
  { id: 'OGR-103', takmaAd: 'KRT-12', subeId: 'SUB-2B', gfi: 0.68, fslope: 0.07, aktifGorev: 'PVC-103' },
  { id: 'OGR-104', takmaAd: 'SRY-22', subeId: 'SUB-4A', gfi: 0.81, fslope: 0.04, aktifGorev: 'PVC-101' },
];

export const SINIF_DURUMU: SinifDurumu[] = [
  { sinifId: '2A', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-2A'), ortalamaFslope: 0.04, sonAlarm: 'Yok' },
  { sinifId: '2B', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-2B'), ortalamaFslope: 0.07, sonAlarm: 'Yorulma Uyarısı' },
  { sinifId: '4A', ogrenciler: OGRENCILER.filter(o => o.subeId === 'SUB-4A'), ortalamaFslope: 0.04, sonAlarm: 'Yok' },
];

~~~~

### `data/mufredatYonerge.ts`

12979 B · SHA-256 `29449f8aa3a170fdc3ae6b179ff4717a16f3ad27d016da1c038a68c55935210f`

~~~~tsx
/**
 * MEB 2. SINIF KAZANIM-AĞACI + DERS-İŞLEME YÖNERGELERİ (K-555 · SCHOLARIA öğretmen-katmanı).
 * Hizalama: kod/ad kümesi disk-kuralına göre MUH-haritaları + MEB_K3-URETIM ile aynıdır
 * (MAT 25 + TR 37 = 62 — PERSONA cocukmoduVeri K3_LIST ile birebir).
 * Telif-çizgisi (K-08/YASA-M1-deseni): kazanım-ADLARI kılavuz-olgudur; YÖNERGELER VAMOLA-ÖZGÜN
 * kompozisyondur — MEB kitap/kılavuz cümlesi KOPYALANMAZ; bu liste resmî-kılavuz yerini TUTMAZ.
 * Dil (K-14): gözlemlenebilir-sayılabilir sınıf-eylemleri; ölçme/evaluation-yargısı yok (K-02).
 */
export interface MufredatKayit { kod: string; ad: string; ders: 'MAT' | 'TR'; yonerge: string }

export const MUFREDAT_2: MufredatKayit[] = [
  // ── MATEMATİK-2 (25) ──
  { kod: 'MAT.2.1.1', ad: 'Sayı postası: oku-yaz-eşle', ders: 'MAT', yonerge: 'Rakam-kartlarıyla 10–100 arası sayıları okutup yazdırın; sayı-adı kartlarıyla eşleştirme oyunu kurun.' },
  { kod: 'MAT.2.1.2', ad: 'Onluk-birlik çantası', ders: 'MAT', yonerge: 'Nesneleri 10\'luk torbalara koydurarak onluk-birlik ayrımını somutlaştırın; tahtadaki tabloya birlikte işleyin.' },
  { kod: 'MAT.2.1.3', ad: 'Sayı doğrusu düellosu', ders: 'MAT', yonerge: 'Yer-matında sayı doğrusu çizip komşu-sayılar arasında yürüyerek yer-değiştirme oyunu oynatın.' },
  { kod: 'MAT.2.1.4', ad: 'Yüzlük tablo zıplaş', ders: 'MAT', yonerge: 'Yüzlük tabloda 1\'er ve 10\'ar atlamaları renkli-kalemle boyattırın; kuralı öğrenciye sözlü teyit ettirin.' },
  { kod: 'MAT.2.1.5', ad: 'Örüntü treni: kural-kur-devam-et', ders: 'MAT', yonerge: 'Şekil/sayı-kartlarıyla 2\'şer-5\'er-10\'ar örüntüler kurdurtun; kuralı sözlutturup sıradaki-halkayı tahmin ettirin.' },
  { kod: 'MAT.2.1.6', ad: 'Tahmin kavanozu: grupla-tahmin et', ders: 'MAT', yonerge: 'Kavanozdaki nesneleri önce 10\'luk gruplatıp tahmin yazdırın; sonra saydırarak tahmini doğrulatın.' },
  { kod: 'MAT.2.1.7', ad: 'Bütün-yarım-çeyrek pizza', ders: 'MAT', yonerge: 'Kâğıt-daireleri katlatıp keserek yarım/çeyrek/bütün ilişkisini yapıştırma-panosunda kurun.' },
  { kod: 'MAT.2.1.8', ad: 'Kasaba para turu', ders: 'MAT', yonerge: 'Sınıf-mağazası dramatizasyonu kurun; TL-banknot kopyalarıyla alışveriş yaptırıp harcama-çizelgesi doldurtun.' },
  { kod: 'MAT.2.1.9', ad: 'Tam saat, yarım saat: saat-avcısı', ders: 'MAT', yonerge: 'Kart-saatlerle tam/yarım-saat ayırımı yaptırın; gün-içi rutini saat-bilgisiyle eşleştirme-turu kurun.' },
  { kod: 'MAT.2.1.10', ad: 'Karış mı, cetvel mi?', ders: 'MAT', yonerge: 'Aynı uzunluğu karış, adım ve cetvel ile ölçtürüp sonuçları karşılaştırın; standart-ölçü gereğini tartıştırın.' },
  { kod: 'MAT.2.1.11', ad: 'Tahmin çubuğu: ölç-karşılaştır', ders: 'MAT', yonerge: 'Uzunlukları önce tahmin ettirip yazdırın; sonra cetveliyle ölçtürüp tahmin-ölçü tablosunu doldurtun.' },
  { kod: 'MAT.2.2.1', ad: 'Toplama ve çıkarma işlemleri gerektiren günlük yaşam problemlerini çözebilme', ders: 'MAT', yonerge: 'Sınıf-içi senaryolardan toplama-çıkarma problemleri kurdurtun; çözümü tek-cümleyle anlattırın.' },
  { kod: 'MAT.2.2.2', ad: 'Tahmin et, zihinden işle, tutarlılığı açıkla', ders: 'MAT', yonerge: 'İşlemi önce zihinden-tahmin ettirin; sonra yazıyla doğrulatıp tahminle-sonucu karşılaştırıp açıklattırın.' },
  { kod: 'MAT.2.2.3', ad: 'Toplama-çıkarma ters-ilişkisi', ders: 'MAT', yonerge: 'Toplamadan çıkarma ürettirtin (a+b=c → c−b=a); boşluklu-kartlarla eşleştirme-oyunuyla pekiştirin.' },
  { kod: 'MAT.2.2.4', ad: 'Çarpma = eş-öbekleri toplama · bölme = eş-paylaştırma', ders: 'MAT', yonerge: 'Eş-öbek dizilimleri kurdurtun; toplamanın-kısa-yolu olarak çarpma yazdırın (2+2+2 = 3×2).' },
  { kod: 'MAT.2.2.5', ad: 'Çarpan ve çarpım: bileşenler', ders: 'MAT', yonerge: '3×4 gibi işlemlerde parça-adlarını öğretin (çarpan-çarpan-çarpım); geriden-seçme oyunu oynatın.' },
  { kod: 'MAT.2.2.6', ad: 'Eşitliğin anlamları: denge', ders: 'MAT', yonerge: 'Terazi-deseninde boşluğa sayı yazdırarak eşitliği kurdurtun (5+3=□+2); dengeyi cümleyle açıklatın.' },
  { kod: 'MAT.2.3.1', ad: 'Geometri ayırma bandı', ders: 'MAT', yonerge: 'Şekil-kartlarını kenar ve köşe-özelliklerine göre sınıflandırma-bandına yerleştirtin; ayrımı sözlü gerekçelendirin.' },
  { kod: 'MAT.2.3.2', ad: 'Küp kule inşaatı', ders: 'MAT', yonerge: 'Küp-kule inşa ettirin; küp-sayısını önce-tahmin sonra-saydırarak karşılaştırma-satırı yazdırın.' },
  { kod: 'MAT.2.3.3', ad: 'Şekil mozaik atölyesi', ders: 'MAT', yonerge: 'Kare/üçgen mozaiklerle yeni-şekiller oluşturtun; hangi-şekillerden oluştuğunu anlattırın.' },
  { kod: 'MAT.2.3.4', ad: 'Döndür-karşılaştır: aynı mı, farklı mı?', ders: 'MAT', yonerge: 'Kesik-şekilleri döndürüp aynı/farklı ayırımı yaptırın; döndürünce adın-değişmediğini tartıştırın.' },
  { kod: 'MAT.2.3.5', ad: 'Bardak sorusu: tahmin-ölç', ders: 'MAT', yonerge: 'Aynı sıvıyı ince/geniş bardaklara döktürüp miktarın-değişmediğini gözlemletin (korunum-yargısı kurdurmadan).' },
  { kod: 'MAT.2.3.6', ad: 'Hedefe yol: planla-izle-analiz', ders: 'MAT', yonerge: 'Sınıf-planında A→B arası yolları çizdirtin; en-kısayı seçtirtin ve adım-adım plan-izle-analiz turu yapın.' },
  { kod: 'MAT.2.3.7', ad: 'Ayna avcısı', ders: 'MAT', yonerge: 'Harf ve şekil-kartlarını aynaya tutturtup simetrikleri avlattırın; simetri-çizgisini kendilerine bozdurtun.' },
  { kod: 'MAT.2.4.1', ad: 'İki grup, bir grafik', ders: 'MAT', yonerge: 'Basit sınıf-anketi yapılıp sonuçları resimli-grafiğe işlettirin; "kaç-fazla/kaç-az" soruları sordurtun.' },
  // ── TÜRKÇE-2 (37) ──
  { kod: 'T.D.1.1', ad: 'Dinleme/izlemeyi yönetebilme', ders: 'TR', yonerge: 'Dinleme-öncesi hedef-verin ("duyuruda ne-istendi?"); dinletip açık-uçlu soru sorun, gözlem-notunuzu düşün.' },
  { kod: 'T.D.1.2', ad: 'Dinlediklerinden anlam kurma: ana-fikir avcısı', ders: 'TR', yonerge: 'Kısa-hikâye dinlettirin; ana-fikri tek-cümleyle tahmin ettirip sınıfça tartışın.' },
  { kod: 'T.D.1.3', ad: 'Dinlediklerini/izlediklerini çözümleyebilme', ders: 'TR', yonerge: 'Sebep-sonuç içeren masal dinlettirin; "neden-bekledi?" sorularıyla çözümleme-tartışması kurun.' },
  { kod: 'T.D.1.4', ad: 'Dinleme/izleme sürecini değerlendirebilme', ders: 'TR', yonerge: 'Dinleme-sonu "ne-anladım" paylaşım-çemberi yaptırın; kendi-dinlemesine bakan cümle kurdurtun.' },
  { kod: 'T.D.2.1', ad: 'Dinleme/izlemeyi yönetebilme (2)', ders: 'TR', yonerge: 'Haber/duyuru dinlettin; kim-ne-zaman ipuçlarını dinlerken resimli-not aldırtın.' },
  { kod: 'T.D.2.2', ad: 'Dinledikleri/izledikleri ile ilgili anlam oluşturabilme', ders: 'TR', yonerge: 'Kurallar-metni dinlettirip dinlediklerinden tek-cümlelik anlam-özeti ürettirin.' },
  { kod: 'T.D.2.3', ad: 'Dinlediklerini/izlediklerini çözümleyebilme (2)', ders: 'TR', yonerge: 'Sıralı-olay anlatımı dinlettin; önce/sonra kartlarını doğru-sıraya dizdirtin.' },
  { kod: 'T.D.2.4', ad: 'Dinleme/izleme sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Gürültülü ve sessiz ortamda kısa-dinleme karşılaştırması yaptırın; farkı birlikte tartıştırın.' },
  { kod: 'T.D.2.5', ad: 'Dinleme/izleme sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Dinlediği-hikâyeyi özetlettirin; güçlü-dinleme belirtilerini birlikte listelettirin.' },
  { kod: 'T.K.1.1', ad: 'Konuşmalarını yönetebilme', ders: 'TR', yonerge: 'Toplantı-çemberinde söz-sırası kuralıyla kısa-konuşmalar yaptırın; el-kaldırma rutinini pekiştirin.' },
  { kod: 'T.K.1.2', ad: 'Konuşmalarında içerik oluşturabilme', ders: 'TR', yonerge: 'Kim/zaman/yer/olay ipuçlarını içeren olay-anlatımı görevi verin; ipuçlarını kullanma-adımını gözlemleyin.' },
  { kod: 'T.K.1.3', ad: 'Konuşma kurallarını uygulayabilme', ders: 'TR', yonerge: 'Göz-teması ve ses-şiddeti hedefleriyle rol-oyunu konuşmaları kurdurun.' },
  { kod: 'T.K.1.4', ad: 'Konuşma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Konuşma-sonu "anlatabildim-mi" öz-tartışma çemberi yaptırın.' },
  { kod: 'T.K.2.1', ad: 'Konuşmalarını yönetebilme (2)', ders: 'TR', yonerge: 'Sınıf-tartışmasında sıra-alma kartları kullanın; dinle-söyle rutini kurun.' },
  { kod: 'T.K.2.2', ad: 'Konuşmalarında içerik oluşturabilme (2)', ders: 'TR', yonerge: 'Gezi/gün-anlatısında önce-sonra-en-son bağlaçlarını kullanma-hedefi verin.' },
  { kod: 'T.K.2.3', ad: 'Konuşma kurallarını uygulayabilme (2)', ders: 'TR', yonerge: 'Telefon-dramatizasyonu kurdurtun; selam-amaç-kapanış üçlüsünü denettirin.' },
  { kod: 'T.K.2.4', ad: 'Konuşma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Ortam-seçiminin anlaşılırlığa etkisini oyunla gözlemletip tartıştırın.' },
  { kod: 'T.K.2.5', ad: 'Konuşma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Konuşma-sonu iki-güçlü-yön bir-gelişim-alanı paylaşımı yaptırın.' },
  { kod: 'T.O.1.1', ad: 'Okuma sürecini yönetebilme', ders: 'TR', yonerge: 'Sessiz-okuma rutini kurun; satır-takip kartıyla odaklanma davranışını gözlem-notuyla izleyin.' },
  { kod: 'T.O.1.2', ad: 'Okuduklarından anlam kurma', ders: 'TR', yonerge: 'Kısa-metin okutturup yanıtı metinde-bulunur sorular sorun; işaretlettirin.' },
  { kod: 'T.O.1.3', ad: 'Okuduklarını çözümleyebilme', ders: 'TR', yonerge: 'Karakter/yer-bilgisi isteyen çözümleme-sorularıyla metin-tartışması kurun.' },
  { kod: 'T.O.1.4', ad: 'Okuma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Okuma-ortamını birlikte düzenlettirin; gürültünün anlamaya-etkisini gözlemletin.' },
  { kod: 'T.O.1.5', ad: 'Okuma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Okuduğunu-yeniden-anlatma çifti kurun; kendi-anlamasını kontrol-cümlesiyle bağdattırın.' },
  { kod: 'T.O.2.1', ad: 'Okuma sürecini yönetebilme (2)', ders: 'TR', yonerge: 'Satır-takip kartı kullanımını modelleyip her-okurda uygulattırın.' },
  { kod: 'T.O.2.2', ad: 'Okudukları ile ilgili anlam oluşturabilme', ders: 'TR', yonerge: 'Yanıtı metinde-olan sorular sorun; buldukları-satırı gösterdirtin.' },
  { kod: 'T.O.2.3', ad: 'Okuduklarını çözümleyebilme (2)', ders: 'TR', yonerge: 'İleti-bulma sorusuyla kısa-hikâye tartışması yaptırın ("bu-hikâye ne-öğretti?").' },
  { kod: 'T.O.2.4', ad: 'Okuma sürecine etki eden durumları gözden geçirebilme (2)', ders: 'TR', yonerge: 'Bilinmeyen-kelime sözlük-köşesi kurun; bakma-adımını modelleyip uygulattın.' },
  { kod: 'T.O.2.5', ad: 'Okuma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Hikâye-özetini kendi-kelimeleriyle anlattırın; anlamasını gözden-geçirtin.' },
  { kod: 'T.Y.1.1', ad: 'Yazılı anlatım becerilerini yönetebilme', ders: 'TR', yonerge: 'Oturuş ve kalem-tutuş kontrol-listesiyle yazma-hazırlığı yaptırın; listeyi öğrenciyle birlikte doldurun.' },
  { kod: 'T.Y.1.2', ad: 'Yazılarında içerik oluşturma', ders: 'TR', yonerge: 'Gün-içi olayı üç-cümleyle yazdirtin; önce-sonra kelimelerini kullanma-hedefi verin.' },
  { kod: 'T.Y.1.3', ad: 'Yazma kurallarını uygulayabilme', ders: 'TR', yonerge: 'Cümle-başı büyük-harf ve nokta-avcılığı yaptırın; yazısını kendine-tarattırın.' },
  { kod: 'T.Y.1.4', ad: 'Yazma sürecini değerlendirebilme', ders: 'TR', yonerge: 'Yazıyı sesli-okuyarak-kontrol rutini kurup arkadaşa-okutma turu yapın.' },
  { kod: 'T.Y.2.1', ad: 'Yazılı anlatım becerilerini yönetebilme (2)', ders: 'TR', yonerge: 'Yazma-öncesi üç-kelimelik mini-plan yaptırıp taslağa geçirtin.' },
  { kod: 'T.Y.2.2', ad: 'Yazılarında içerik oluşturabilme (2)', ders: 'TR', yonerge: 'Tarih-hitap-ileti-imza şablonuyla sınıf-içi mektup yazdirtin.' },
  { kod: 'T.Y.2.3', ad: 'Yazma kurallarını uygulayabilme (2)', ders: 'TR', yonerge: 'Noktalama-kartlarıyla cümle-düzeltme yarışı kurun.' },
  { kod: 'T.Y.2.4', ad: 'Yazma sürecine etki eden durumları gözden geçirebilme', ders: 'TR', yonerge: 'Kalem-tutuşu düzeltme egzersizlerini kısa-turlarla yaptırın; yorgunluk-belirtisini gözlemleyin.' },
  { kod: 'T.Y.2.5', ad: 'Yazma sürecini değerlendirebilme (2)', ders: 'TR', yonerge: 'Yazım-noktalama-anlam üçlü-kontrol listesini birlikte doldurtun.' },
];

export const MUFREDAT_SINIF = '2. sınıf';
export const MUFREDAT_KAYNAK_NOTU =
  'Kazanım-kod/adları 2. sınıf MUH-haritası kümesiyle hizalıdır (MAT 25 + TR 37). Ders-işleme yönergeleri VAMOLA-özgün kompozisyondur; MEB kitabı/kılavuzu kopyalanmaz ve bu liste resmî kılavuzun yerini tutmaz (K-08).';

~~~~

### `data/seriler.ts`

1094 B · SHA-256 `02b9e2671aa6414d942e4eea36f58ff09b7735cc312a8cfcd5bd671ab08a28f9`

~~~~tsx
// VAMOLA EduLabs Scholaria v0.2.2 — Deterministik sentetik seriler (K-05 MOCK · K-554).
// Seed'li sin-dalga: her-açılışta-aynı; gerçek sensör-akışı DEĞİLDİR — yalnız gösterim-verisi (K-02).
export function seri(seed: number, n = 12, baz = 0.4, genlik = 0.14): number[] {
  return Array.from({ length: n }, (_, i) =>
    Math.round((baz + genlik * Math.sin(seed * 1.7 + i * 0.9) + (i / n) * 0.05) * 1000) / 1000
  );
}

export function gContrastSeri(sinifId: string): number[] {
  const seed = sinifId.split('').reduce((a, c) => a + c.charCodeAt(0), 0);
  return seri(seed, 12, 0.38, 0.12);
}

export function sdrtSeri(id: string): number[] {
  const seed = parseInt(id.replace(/\D/g, ''), 10) || 7;
  return seri(seed, 12, 0.05, 0.035);
}

/** Seriyi SVG-polyline 'x,y' noktalarına çevirir. */
export function noktalar(vals: number[], w = 240, h = 48): string {
  const min = Math.min(...vals);
  const max = Math.max(...vals);
  const ar = max - min || 1;
  return vals.map((v, i) => `${(i / (vals.length - 1)) * w},${h - ((v - min) / ar) * (h - 6) - 3}`).join(' ');
}

~~~~

### `main.tsx`

236 B · SHA-256 `14a10dee4aaa2130d9f57c136db7f16f95f524d60d77146b17776e91c2ab626c`

~~~~tsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';
import './index.css';

ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);

~~~~

### `types/index.ts`

599 B · SHA-256 `767b7b28b508f71deecfacc37e6530ba4274cb7fa8e62524ada975b7d2f671dc`

~~~~tsx
// VAMOLA EduLabs Scholaria v0.1.0 — Tipler
export interface Ogrenci {
  id: string;
  takmaAd: string;
  subeId: string;
  gfi: number;
  fslope: number;
  aktifGorev: string;
}

export interface Sube {
  id: string;
  ad: string;
  ogrenciSayisi: number;
}

export interface Gorev {
  id: string;
  baslik: string;
  dersId: string;
  modul: string;
}

export interface EBAAuth {
  accessToken: string;
  refreshToken: string;
  expiresIn: number;
  maskedUid: string;
}

export interface SinifDurumu {
  sinifId: string;
  ogrenciler: Ogrenci[];
  ortalamaFslope: number;
  sonAlarm: string;
}

~~~~

### `types/surum.d.ts`

99 B · SHA-256 `c7816811300c1ea2de941d4302b67a45099395f33cd75e58c144efd668f4a381`

~~~~tsx
declare const __SURUM__: string;
declare const __TAM__: boolean;
declare const __PILOT__: boolean;

~~~~

## Ek D — yeniden üretim ve giriş/çıkış kontrolü

Bu araçlar yalnız geçici çalışma dosyalarında koşuldu; kalıcı araç/kod değişikliği yapılmadı. Mevcut envanter aracı regex havuzu LEX232/SED230; AST havuzu farklı yöntemle LEX474/SED470 kayıttır. İkisi de hata/eksiksizlik ölçüsü değildir. Regex ön-taramasında emekli0/risk0 çıkması, yukarıdaki işlev/iddia adaylarını geçersiz kılmaz.

### scholaria-hazirlik.cjs

~~~~javascript
const fs=require('fs'),path=require('path'),crypto=require('crypto');
const R='/home/user/VAMOLA';const ts=require(R+'/VAMOLA - Seduva/SEDUVA_MENTORIA/node_modules/typescript');
const roots={LEX:'VAMOLA - Lexiva/LEXIVA_SCHOLARIA/SCHOLARIA_TAM',SED:'VAMOLA - Seduva/SEDUVA_SCHOLARIA'};
const out={};
function walk(d){return fs.readdirSync(d,{withFileTypes:true}).flatMap(e=>e.isDirectory()?walk(path.join(d,e.name)):[path.join(d,e.name)])}
for(const [key,rel] of Object.entries(roots)){
 const src=path.join(R,rel,'src'),files=walk(src).filter(f=>/\.tsx?$/.test(f)).sort();let rows=[];let meta=[];
 for(const f of files){
  const text=fs.readFileSync(f,'utf8'),name=path.relative(src,f);const sf=ts.createSourceFile(f,text,ts.ScriptTarget.Latest,true,f.endsWith('tsx')?ts.ScriptKind.TSX:ts.ScriptKind.TS);
  meta.push({file:name,bytes:Buffer.byteLength(text),sha256:crypto.createHash('sha256').update(text).digest('hex')});
  function visit(n){
   let value=null;if(ts.isJsxText(n)||ts.isStringLiteral(n)||ts.isNoSubstitutionTemplateLiteral(n)||ts.isTemplateHead(n)||ts.isTemplateMiddle(n)||ts.isTemplateTail(n))value=n.text;
   if(value){
    let skip=false;for(let p=n.parent;p;p=p.parent){if(ts.isImportDeclaration(p)||ts.isExportDeclaration(p))skip=true;if(ts.isJsxAttribute(p)&&['className','data-testid','id','key','type','value','name','htmlFor','viewBox','fill','stroke','width','height'].includes(p.name.getText(sf)))skip=true;}
    if(!skip&&/[\p{L}]/u.test(value)&&value.trim().length>=3&&(ts.isJsxText(n)||/\s|[ÇĞİÖŞÜçğıöşü]/.test(value)||/^[A-Z]{3,}$/.test(value))&&!/^(?:bg-|text-|border-|http|\.\/|\.\.\/)/.test(value.trim())){
     let pos=sf.getLineAndCharacterOfPosition(n.getStart(sf));rows.push({id:`SCH-${key}-${String(rows.length+1).padStart(4,'0')}`,file:name,line:pos.line+1,kind:ts.SyntaxKind[n.kind],text:value.trim(),reach:name.includes('FrictionMap')?'Bağlı değil: kaynak rezervi':'App/import bağlamında; koşullu görünürlük ayrıca DOM’da'});
    }
   }ts.forEachChild(n,visit);
  }visit(sf);
 }
 const shell=fs.readFileSync(path.join(src,'components/shell/Kabuk.tsx'),'utf8');
 const nav=[...shell.matchAll(/\{ id: '([^']+)', ad: '([^']+)'/g)].map(m=>({id:m[1],label:m[2]}));
 out[key]={root:rel,version:JSON.parse(fs.readFileSync(path.join(R,rel,'package.json'),'utf8')).version,files:meta,rows,nav};
}
fs.writeFileSync('/tmp/scholaria-kaynak.json',JSON.stringify(out,null,2));console.log(Object.fromEntries(Object.entries(out).map(([k,v])=>[k,{files:v.files.length,rows:v.rows.length,nav:v.nav.length}])));

~~~~

### scholaria-dom.cjs

~~~~javascript
const fs=require('fs');const R='/home/user/VAMOLA';const {chromium}=require(R+'/VAMOLA - Seduva/SEDUVA_MENTORIA/node_modules/playwright-core');
const jobs=[['LEX','VAMOLA - Lexiva/LEXIVA_SCHOLARIA/SCHOLARIA_TAM/LEXIVA-SCHOLARIA-v2.10.1.html'],['SED','VAMOLA - Seduva/SEDUVA_SCHOLARIA/SCHOLARIA-MVP-TAM-v0.2.7.html']];
(async()=>{const browser=await chromium.launch();const out={};for(const [key,file] of jobs){
 const c=await browser.newContext();const p=await c.newPage();p.setDefaultTimeout(5000);const r={file,errors:[],network:[],states:[],checks:[]};
 p.on('pageerror',e=>r.errors.push(e.message));p.on('console',m=>{if(m.type()==='error')r.errors.push(m.text())});p.on('request',q=>{if(/^https?:/.test(q.url()))r.network.push(q.url())});
 await c.route(/^https?:/,route=>route.abort());await p.goto('file://'+R+'/'+file);
 async function snap(name){r.states.push({name,text:await p.locator('main').innerText(),fields:await p.locator('main textarea').evaluateAll(es=>es.map(e=>({id:e.dataset.testid,readOnly:e.readOnly,value:e.value}))),buttons:await p.locator('main button').allTextContents()})}
 const ids=await p.locator('nav [data-testid]').evaluateAll(es=>es.map(e=>e.dataset.testid));r.nav=ids;r.role=await p.locator('aside').innerText();
 for(const id of ids){await p.getByTestId(id).click();await snap(id)}
 await p.getByTestId('nav-ogrenci').click();await p.locator('[data-testid^="ogrenci-gorev-"]').first().click();await snap('ogrenci-gorev-detay');
 await p.getByTestId('nav-transfer').click();await p.getByTestId('hc-davranis-0').click();await p.getByTestId('hc-not').fill('SENTETIK BRIEF TESTI — gerçek öğrenci değildir.');await p.getByTestId('hc-kaydet').click();await snap('transfer-kayitli');
 await p.getByTestId('nav-rapor').click();await snap('rapor-kayitli');r.checks.push({name:'H-c notu rapora taşındı',ok:(await p.getByTestId('rapor-not-ornegi').inputValue()).includes('SENTETIK BRIEF TESTI')});
 await p.getByTestId('nav-eba').click();await p.getByTestId('eba-taslagi-uret').click();await snap('eba-taslak');
 await p.getByTestId('nav-veli').click();await snap('veli-kayitli');
 await p.getByTestId('nav-ogretmen').click();await p.getByRole('button',{name:'YZ Önerisi İste',exact:true}).click();await snap('yz-oneri');const before=await p.getByTestId('oneri-notu').inputValue();await p.getByRole('button',{name:'✓ Onayla ve Yürürlüğe Al',exact:true}).click();const after=await p.getByTestId('oneri-notu').inputValue();r.approvalObservation={noteUnchanged:before===after,storageKeys:await p.evaluate(()=>Object.keys(localStorage))};
 await p.getByRole('button',{name:'✕ Reddet ve Gerekçelendir',exact:true}).click();await snap('yz-reddet');
 await p.getByTestId('nav-bep').click();await p.getByTestId('bep-sablon-uret').click();await p.getByTestId('bep-probe-ekle').click();await snap('bep-taslak-probe');
 await p.getByTestId('nav-ders').click();await p.getByTestId('atama-isle').click();await snap('ders-atamali');await p.getByTestId('ders-tr').click();await snap('ders-turkce');
 await p.getByTestId('nav-rapor').click();await snap('portfoy-atamali');
 r.checks.push({name:'14 menü açıldı',ok:ids.length===14},{name:'çalışma zamanı/konsol hatası yok',ok:r.errors.length===0},{name:'bu akışlarda HTTP/S girişimi yok',ok:r.network.length===0});out[key]=r;console.log(key,JSON.stringify({states:r.states.length,checks:r.checks,errors:r.errors,network:r.network,approval:r.approvalObservation}));await c.close();
}await browser.close();fs.writeFileSync('/tmp/scholaria-dom.json',JSON.stringify(out,null,2));if(Object.values(out).some(r=>r.checks.some(x=>!x.ok)))process.exit(1)})().catch(e=>{console.error(e);process.exit(2)});

~~~~

### LEX smoke (mevcut test, mevcut kanonik HTML)

~~~~text

SONUÇ: 12 geçti, 0 kaldı (toplam 12)

~~~~

### SED smoke (mevcut test, mevcut kanonik HTML)

~~~~text

SONUÇ: 12 geçti, 0 kaldı (toplam 12)

~~~~

**Koruma kapısı:** Mühür manifestinin tüm anahtarları başlangıç/çıkış SHA karşılaştırmasına alındı. Ürün/kanon/HTML değişmedi; yalnız bu yeni brief ve K-760 yönetim kayıtları oluştu. Mevcut v7.65.61 ZIP/manifest değiştirilmedi. Nihai disk farkı DEFTER K-760 ve devir §16’ya yazılır.
