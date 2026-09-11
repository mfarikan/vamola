# SUPPORTA — İKİ AYRI ÜRÜN İÇİN DIŞ GÖRÜŞ BRİEFİ v0.1

**Kayıt:** K-764 · **Tarih:** 11.09.2026 · **Durum:** kaynak/DOM hazırlığı tamam; dış görüş bekleniyor.
**Yetki:** Sahibin ayrı ask_user seçimi: SUPPORTA paketini hazırla. Salt-okunur inceleme ve brief; ürün/kanon/mühür değişikliği değil.
**Taban:** v7.65.62 mühürlü kaynak + mevcut TAM artefaktları. Bu yeni brief henüz mühür dışıdır. Dağıtımı sahibi yapar; ajan dışarıya göndermedi.

## 0. Değerlendiriciye görev — önce kapsam, sonra satır

Bu bir aile uygulaması incelemesi değildir. **SUPPORTA-SED ve SUPPORTA-LEX iki ayrı merkez/uzman ürünüdür.** Aile bilgilendirilen/çıktı alıcısı ve veri kaynağıdır; veli sistem rolü yoktur. İki ürünün benzer kabuğu, içerik ve kararlarının aynı olduğu anlamına gelmez. MENTORIA/SCHOLARIA kararları otomatik aktarılmaz.

1. Her ürün için ayrı `KAPSAM TAMAM` veya `KAPSAM EKSİK — eksik ekran/rol/çıktı/kaynak` yazın. Kabul bilimsel/hukuki/kanonik uygunluk sertifikası değildir.
2. Sonra ürün ve exact ID bazında `KORU / REVİZE ADAYI / İŞLEV-ROL DOĞRULAMASI / KAYNAK DOĞRULAMASI / GİZLE ADAYI` önerin. Dış öneri, uygulama yetkisi değildir.
3. Çocuk M-3/0-hit kurallarını yetişkin ekranına kör uygulamayın. Uzman teknik terim, eğitmen açıklamalı metrik, aile düz/jargonsuz çıktı ayrımı korunur. Şerh, desteklenmeyen sayı/çıkarım veya eksik yetki işlevini tek başına çözmez.
4. Mevcut onaylı adları değiştirmeyi otomatik düzeltme saymayın. Yeni sözlük/protokol, ürün sürümü veya hesaplama kararı bu paketin amacı değildir.

| Ürün | ID / dosya:satır / DOM durumu | Exact alıntı | Okur | Öneri sınıfı | Gerekçe ve dayanak | Minimum öneri | İşlev/kaynak bağımlılığı |
|---|---|---|---|---|---|---|---|
| SUPPORTA-SED / SUPPORTA-LEX | SUP-SED-… / SUP-LEX-… | Parçayı tam cümle sanmadan | uzman/eğitmen/kurum/aile | ürün-başı | URL+baskı/sürüm+sayfa veya yerel karar | uygulamasız | açıkça yazın |

## 1. Kanıtın kapsamı ve sınırı

- **13 menü ×2 rol ×2 ürün** gezildi. Her üründe uzman ve yönetici için ayrı yeni tarayıcı bağlamı kullanıldı. Veli rol düğmesi yok.
- Her ürün için **35 ekran/durum**; textarea içerikleri, öneri/red/onay sonrası durumlar dahil. Uzman rolünde **rapor + Aile A + Aile B =3 yazdırma önizlemesi**, ayrıca rapor CSV'si alındı; toplam6 önizleme/2 CSV. Gerçek yazıcı kullanılmadı (`window.print` testte susturuldu).
- Mevcut kalıcı smoke: **SED127/127, LEX127/127; konsol/sayfa hata0**. Ek DOM akışında gözlenen pageerror0 ve HTTP/S girişimi0. Ağ çıkışı test bağlamında engellendi. Bu, tüm güvenlik/onam/yetkilendirme davranışlarının doğrulanması değildir.
- Build/tsc yeniden yapılmadı. Mevcut kanonik HTML'ler incelendi; tam kaynak→build üretim eşdeğerliği yeniden derlemeyle kanıtlanmadı. Ürünler/sürümler/kalıcı testler/kanon değişmedi.
- AST havuzu: **SED903 / LEX916 kaynak kaydı**; benzersiz görünür cümle ya da hata sayısı değil. Koşullu/template/teknik parçalar içerir. Her ürünün16 TS/TSX dosyasının tam ham kaynağı ekte; yorum/rezerv kod canlı UI değildir. CSS metin havuzuna dahil edilmedi.
- Regex ön-tarama havuzu SED288/LEX289; emekli0/risk0. Dar regex sonucu aşağıdaki istatistik/rol/çıktı adaylarını aklamaz.
- Mevzuat, MEB kod/ad/saat, psikometri, telif ve pedagojik içerik kaynakları bu turda web üzerinden yeniden doğrulanmadı. Yerel belgelerin atıfları dış doğrulama diye sunulmaz.

## 2. Öncelikli kaynak/işlev inceleme adayları

Aşağıdaki benzer desenlere **iki ürün için ayrı karar** verin. Bunlar otomatik değişiklik listesi değildir.

| Aday | Kaynakla görülen durum | Sınır / sorulacak soru |
|---|---|---|
| Rapor YZ beyanı | Ekranlar/RaporAtolyesi: SED dikkat sürekliliğinde %20 varyans; LEX okuma görevi sürekliliğinde %20 varyans. İkisinde %82 güven aralığı ve Sembolik→Fiziksel destek önerisi sabit metin. Oturum/süre sayımı var; LEX girdi sayımı da ekli. | Sayım yapılması varyans/güven aralığı hesabı değildir. Öneri ve Support Fading teriminin yönü/kaynak dayanağı ayrıca incelenmeli. Gerçek model çağrısı kanıtlanmadı. |
| Veri kaynağı | Oturum sayısı/süre ve bazı girdi özetleri ithal MOCK sabitlerinden; diğer tablolar useKalici yerel state'inden okunuyor. | Güncel kullanıcı girdisiyle rapor/çizelge özetinin aynı veri hattından beslendiğini varsaymayın. |
| Red gerekçesi | Rapor red düğmesi sabit T2-yorgunluk verisi eksikliği gerekçesini metne ekliyor. | Uzmanın yazdığı gerekçe veya gerçekten saptanmış veri eksiği gibi sunulmamalı. |
| Rol/onay | ROLLER uzmanı taslak üretimiyle, yöneticiyi onayla tanımlıyor. App rolü etikete geçiriyor; RaporAtolyesi rol parametresi almıyor. DOM'da uzman da yönetici de R-1'i onaylayabildi. | Yerel rapor durum kilidi çalışıyor; ayrı yetki denetimi çalışıyor sonucu çıkarılamaz. Bu demo gözlemi gerçek sistem güvenlik olayı değildir. |
| İmza/tarih | onayKim='Yönetici', onayTarih='2026-09-03' sabit; 'Onayla ve İmzala' etiketi kullanılıyor. | Gerçek kimlik/imza/zaman izi yerine geçer mi? İmza güvence iddiası ayrıca doğrulanmalı. |
| Aile çıktısı onayı | Aile A/B yazdırma yolunda ayrı rapor onay state'i yok; çıktı damgası 'ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER'. | RaporAtolyesi taslak kilidini aile çıktısına genellemeyin. ONAYLI/TASLAK ve hangi nesnenin onaylandığı ayrılmalı. |
| B — Analize Göre | Kişisel havuz kartları div olarak gösteriliyor, seçim handler'ı yok; sabit uzman notu şablonu basılıyor. | 'Havuzdan seçin / uzman yazar' ile uygulama içi seçim/düzenleme işlevi aynı şey değildir; kağıt üzerinde kullanım niyeti ayrıca sorulmalı. |
| Çizelge | '+', 'Evet', '3' kayıtları 'Hedefe ulaşılan' sayılıyor. Bar yüksekliği kayıt sırasından `min(96,28+i*16)` ile geliyor. | Kodlama anlamları ve grafik yüksekliğinin temsil ettiği veri açıklanmalı; yükselen bar gerçek ilerleme değildir. |
| DEP/RAM/saat | Program/saat/form/tavan ve kayıt hattı sabitleri gösteriliyor. | Planlama sınırı, resmî formun yerine geçmeme ve tarih/sürüm/hukuki kapsam ayrı doğrulanmalı. 8+4 tarihî belge çerçevesi ile 12/4 ürün tavanları farklı kavramlar olabilir; kaynak okumadan çelişki ilan etmeyin. |
| Rezerv bileşen | EgitmenDestekPaneli.tsx'te başarı≥3 üzerinden fading ve recovery dili var, fakat App/Ekranlar importuna bağlı değil. | Aktif Eğitmen Kürsüsü bu dosya değildir. Kaynak rezervini canlı bulgu diye saymayın. RaporAtolyesi'ndeki aktif fading metni ise ayrı adaydır. |
| Çıktı güvenliği | Yazdırma HTML'i başlık/içeriği document.write şablonuna yerleştiriyor; rapor CSV'si de üretiliyor. | Girdi kaçışlama, formül enjeksiyonu, mahremiyet ve çıktı sanitizasyonu ayrı teknik inceleme gerektirir; bu tur saldırı testi yapılmadı. |

## 3. SUPPORTA-SED — ayrı ürün kapsamı

**0.8.8.** Merkez uzmanı/eğitmen ve yönetici; destek eğitim, DEP-2026 ve ayrı BGM-12 yürütücü işlev içerik katmanı. DEHB alanı, dikkat görevleri ve aile eğitim içeriği SED bağlamında okunmalıdır. Ölçüm/tedavi iddiası ile gözlem/şablon ayrımı ayrı değerlendirilir. LEX'in okuma/fonolojik kararları buraya taşınmaz.

**Kaynak kökü:** `VAMOLA - Seduva/SEDUVA_SUPPORTA/src`

**Kanonik:** `VAMOLA - Seduva/SEDUVA_SUPPORTA/SUPPORTA-TAM-v0.8.8.html` ·319040 B ·SHA `c276f5afd030b3bcb472d10728f27042e01136f422d0b65a35326167e6d29fca`

| Menü/id | Ekranlar.tsx fonksiyonu / bağlı bileşen | Okur | Sınır |
|---|---|---|---|
| Eğitmen Kürsüsü / `pano` | Pano | Uzman/eğitmen | Dosya/oturum/girdi özeti; aktif Eğitmen Kürsüsü, rezerv EgitmenDestekPaneli değil. |
| Dosyalar / `dosyalar` | Dosyalar | Uzman/yönetici | Sentetik dosya ve onam/izin alanları; kimlik/yetki güvencesi ayrıca. |
| Takvim / `takvim` | Takvim | Uzman/yönetici | Oturum planlama ve durum/çakışma; resmî yoklama/ödeme sistemi sayılmaz. |
| Oturum Atölyesi / `oturum` | OturumAtolyesi | Uzman/eğitmen | Etkinliğe bağlı x/+,0–3,E/H girdi ve ipucu gözlemi. |
| Etkinlik Kataloğu / `katalog` | EtkinlikKatalogu | Uzman/eğitmen | DEP/BGM etkinlik seçimi, yerel ekle/düzenle/sil. |
| İzleme Çizelgesi / `cizelge` | Cizelge | Uzman/eğitmen | Girdi sayımı, başarı etiketi, sıra tabanlı barlar; DEP/BGM filtresi. |
| Rapor Atölyesi / `rapor` | RaporAtolyesi | Üreten uzman/yönetici; alıcı aile/kurum | Taslak düzenleme, sabit YZ/red metni, onay durumu, yazdırma+CSV. |
| Program Hizalama / `hizalama` | Hizalama | Uzman/yönetici | MEB/DEP modül/saat referansları; resmî entegrasyon değil. |
| Bilişsel Geliştirme / `bgm` | BgmMenu | Uzman/eğitmen | Ürüne özgü 12 modül; sırayı uzman belirler; DEP ayrı. |
| RAM & BEP Takibi / `rambep` | RamBep | Uzman/yönetici | RAM/BEP/kayıt hattı ve form referansları; resmî belge yerine geçmez. |
| Ev Çalışmaları / `evodev` | EvOdevleri | Uzman/eğitmen; alıcı aile | Ev çalışması ve durum takibi; veli sistem rolü yok. |
| Aile & Öğretmen / `aile` | Aile + aile/AileEgitimMerkezi | Üreten uzman/yönetici; alıcı aile/öğretmen | Genel5 mini-modül, kişisel şablon havuzu, A/B yazdırma ve iletişim taslağı. |
| Ayarlar / `ayarlar` | Ayarlar | Uzman/yönetici | Yerel kayıt/silme ve kapsam dışı açıklamaları; idari-mali otomasyon değil. |

**Rol kanıtı:** Yeni uzman ve yönetici bağlamları aynı13 menüye erişti; ikisi de R-1 taslağını onayladı ve dışa aktarma düğmesini etkinleştirdi. Taslakta düğme disabled idi. Veli rolü bulunmadı. Bu iki farklı kontrolü (durum kilidi / rol yetkisi) karıştırmayın.

**Exact aday adresleri:**
- %20: SUP-SED-0125 (components/Ekranlar.tsx:390)
- %82: SUP-SED-0125 (components/Ekranlar.tsx:390)
- Hedefe ulaşılan: SUP-SED-0113 (components/Ekranlar.tsx:363)
- ONAYLI — K-02: SUP-SED-0317 (components/aile/AileEgitimMerkezi.tsx:14)
- Gerekçe:: SUP-SED-0126 (components/Ekranlar.tsx:398)
- uzmanlaştı: SUP-SED-0355 (components/egitmen/EgitmenDestekPaneli.tsx:81)

## 4. SUPPORTA-LEX — ayrı ürün kapsamı

**2.10.0.** Merkez uzmanı/eğitmen ve yönetici; K-700 okuma/fonolojik alan uyarlaması. Teknik dosya adının bgm.ts/BGM kalması SED DEHB modüllerinin devralındığı anlamına gelmez: içerik EQ kodlu okuma/fonolojik modüllerdir. Rapor önerisi okuma görevi sürekliliği metni taşır ve SED'den farklı olarak girdi sayısı da ekler. Bu farklar LEX'e özgü değerlendirilmelidir; şablondaki %20/%82 yine hesaplanmış sayılmaz.

K-700 veya “ÖÖG uyarlama” etiketi ölçüm geçerliği kanıtı değildir. Tarihî DEP planlayıcı v0.1 TASLAK belgesini güncel çalışan ürünün birebir özellik listesi saymayın.

**Kaynak kökü:** `VAMOLA - Lexiva/LEXIVA_SUPPORTA/SUPPORTA_TAM/src`

**Kanonik:** `VAMOLA - Lexiva/LEXIVA_SUPPORTA/SUPPORTA_TAM/LEXIVA-SUPPORTA-v2.10.0.html` ·320174 B ·SHA `e9dce2d0bdc4bb99e4298987dbd461f2ca8c8f76a5e14e15f0f91ca473e06280`

| Menü/id | Ekranlar.tsx fonksiyonu / bağlı bileşen | Okur | Sınır |
|---|---|---|---|
| Eğitmen Kürsüsü / `pano` | Pano | Uzman/eğitmen | Dosya/oturum/girdi özeti; aktif Eğitmen Kürsüsü, rezerv EgitmenDestekPaneli değil. |
| Dosyalar / `dosyalar` | Dosyalar | Uzman/yönetici | Sentetik dosya ve onam/izin alanları; kimlik/yetki güvencesi ayrıca. |
| Takvim / `takvim` | Takvim | Uzman/yönetici | Oturum planlama ve durum/çakışma; resmî yoklama/ödeme sistemi sayılmaz. |
| Oturum Atölyesi / `oturum` | OturumAtolyesi | Uzman/eğitmen | Etkinliğe bağlı x/+,0–3,E/H girdi ve ipucu gözlemi. |
| Etkinlik Kataloğu / `katalog` | EtkinlikKatalogu | Uzman/eğitmen | DEP/BGM etkinlik seçimi, yerel ekle/düzenle/sil. |
| İzleme Çizelgesi / `cizelge` | Cizelge | Uzman/eğitmen | Girdi sayımı, başarı etiketi, sıra tabanlı barlar; DEP/BGM filtresi. |
| Rapor Atölyesi / `rapor` | RaporAtolyesi | Üreten uzman/yönetici; alıcı aile/kurum | Taslak düzenleme, sabit YZ/red metni, onay durumu, yazdırma+CSV. |
| Program Hizalama / `hizalama` | Hizalama | Uzman/yönetici | MEB/DEP modül/saat referansları; resmî entegrasyon değil. |
| Bilişsel Geliştirme / `bgm` | BgmMenu | Uzman/eğitmen | Ürüne özgü 12 modül; sırayı uzman belirler; DEP ayrı. |
| RAM & BEP Takibi / `rambep` | RamBep | Uzman/yönetici | RAM/BEP/kayıt hattı ve form referansları; resmî belge yerine geçmez. |
| Ev Çalışmaları / `evodev` | EvOdevleri | Uzman/eğitmen; alıcı aile | Ev çalışması ve durum takibi; veli sistem rolü yok. |
| Aile & Öğretmen / `aile` | Aile + aile/AileEgitimMerkezi | Üreten uzman/yönetici; alıcı aile/öğretmen | Genel5 mini-modül, kişisel şablon havuzu, A/B yazdırma ve iletişim taslağı. |
| Ayarlar / `ayarlar` | Ayarlar | Uzman/yönetici | Yerel kayıt/silme ve kapsam dışı açıklamaları; idari-mali otomasyon değil. |

**Rol kanıtı:** Yeni uzman ve yönetici bağlamları aynı13 menüye erişti; ikisi de R-1 taslağını onayladı ve dışa aktarma düğmesini etkinleştirdi. Taslakta düğme disabled idi. Veli rolü bulunmadı. Bu iki farklı kontrolü (durum kilidi / rol yetkisi) karıştırmayın.

**Exact aday adresleri:**
- %20: SUP-LEX-0126 (components/Ekranlar.tsx:390)
- %82: SUP-LEX-0126 (components/Ekranlar.tsx:390)
- Hedefe ulaşılan: SUP-LEX-0113 (components/Ekranlar.tsx:363)
- ONAYLI — K-02: SUP-LEX-0320 (components/aile/AileEgitimMerkezi.tsx:14)
- Gerekçe:: SUP-LEX-0127 (components/Ekranlar.tsx:398)
- uzmanlaştı: SUP-LEX-0358 (components/egitmen/EgitmenDestekPaneli.tsx:81)

## 5. Mevcut karar ve kaynak disiplini

- **K-296:** Persona dışında veli oturumu yok; aile bilgilendirilen ve veri kaynağı. Aile ekranı/çıktısı uzman-kullanımlıdır. Bu, aile için içerik bulunmasını yasaklamaz.
- **K-700:** LEX BGM alan uyarlaması ve aile kartları; SED yürütücü işlev menüsü LEX'e otomatik devredilmez.
- **K-708/K-709:** Eğitmen Kürsüsü ve mevcut onaylı adlar. Önerilen yeni adlar kendiliğinden kanon olmaz.
- **K-651:** EgitmenDestekPaneli tasarım kaydı; bugün dosya bulunması aktif bağlantı kanıtı değildir.
- SHERHLER/YASA_1/2/3 ve mevcut README, etkinliğe bağlı girdi, girdiden çizelge, taslak/onay ve resmî form sınırını yazar. Bu ilkelerin hangi işlevde gerçekten zorlandığı ayrı incelenir.
- **Atıf uyarısı:** Kodda K-263 form sınırına atfediliyor; strateji defterindeki doğrudan K-263 başlığı başka bir ürün-ön-test erteleme/ürün odağı kararını anlatıyor. Bu numarayı tek başına asıl form-sınırı kanıtı saymayın. Güncel şerh/README'de sınır açıkça mevcut; ilk kararın iz sürümü ayrıca gerekir. Numara/kanon bu turda değiştirilmedi.
- Kaynakta yorum olarak geçen spec/_analiz yollarının bir kısmı bu ağaçta bulunmadı; bulunmayan belge okunmuş sayılmadı. Kanıt eksiği doğrudan ürünü kusursuz/kusurlu ilan etme gerekçesi değildir.

## 6. Dış görüşten sonra yapılacak iş

Sahip paketi paylaşır → iki ürün için ayrı kapsam kabulü ve exact satır önerileri gelir → kaynak/kanon/işlev karşılaştırması → ayrı sahip uygulama kararları. Uygulama onayı olmadan kaynak/HTML/kanon değişmez. Mühür ayrıca onaylanır.

**Şimdiki sonuç:** teknik olarak açılan/çalışan mevcut prototipler; tüm kanonik/rol/kaynak doğrulaması tamam değil. SUPPORTA için hiçbir düzeltme seçilmedi. MENTORIA/SCHOLARIA açıkları ve Vanderbilt bu turda ele alınmadı. v7.65.62 çifti korunur.

## Ek A — mevcut kanonun tam kopyası

Aşağıdaki yerel kanon dış bilimsel/hukuki sertifika değildir; tarihî sürüm atıfları sessizce düzeltilmedi.

### VAMOLA-STRATEJIK-HIZALAMA-VE-DIL-PROTOKOLU_v1.2.md
SHA `e9336cc78dcd45ca8eb3914be601003f7efb7cc6502522794affcc03dc2c3455`

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
SHA `aec734d82e9444b35e065b1d26654717d4cbcf918d1ce19783a20c67731c783e`

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

## Ek B — seçilmiş karar zinciri ve yaşayan/tarihî belge ayrımı

~~~~markdown
**K-296 (02.09 — VELİ-ERİŞİMİ-KURALI [kullanıcı-zip-incelemesi-sonrası-kararı: 'Persona dışındaki ürünlere veli erişimi olmayacak; veli bilgilendirilen ve veri kaynağı pozisyonunda']).**
Kapsam: **B2B-üçlü-(Scholaria/Supporta/Mentoria)'de veli-sistem-oturumu/rolü/ekranı-YOK**; veli=①bilgilendirilen-(yazılı-çıktı/görüşme-ile; çıktı-yalnız-onaylı-raporla) ②veri-kaynağı-(beyanlar-uzman-vekâleten-işler). Persona-(B2C)-değişmedi-(veli-ev-bacağı+onay).
Uygulama: çerçeve-**v0.1.2-eki**-(§1.2-rol-modeli-kilitli+§2.3-kural-satırı) · spec-v0.1-ekisi-(§3-'Veli'-satırı→YOK+§4-ekran-⑪→'aile-bilgilendirme-çıktısı'+§6-K-296-şerhi+§9-**KC7**+§11-'veli-kanalı'-açık-sorusu-KAPANDI: kanal-sistem-dışıdır) · **prototip-v0.1.0→v0.1.1**-(ROLLER-3→2-rol · eVeli/veli-sekmesi-SİLİNDİ → **eBilgilendirme/M7b-Aile-Bilgilendirmesi**-(uzman-kullanımlı-çıktı+vekâleten-beyan-girişi) · rol-seçim+footer-K-296-notu · dosya-adı-v0.1.1 · jüri-zip-v0.1.1-(eski-v0.1.0-SİLİNDİ-yerine)).
**TEST-KASKADI-TAM-YEŞİL:** node---check ✓ · smoke-2-rol×9-ekran-(KC1-neg/pos · KC2-neg/pos-(onaysıza-alert+kopya-yok→onay→2-kopya) · KC5) ✓ · KC7-yapı-(ROLLER-veli-siz · eVeli-undefined · 'Veli-bakışı'-0-hit) ✓ · dil-kapısı-(ms/NF/Berard/Tomatis=0; tedavi/terapi-yalnız-inkâr/şerh-bağlamı) ✓ · K-296/vekâleten/bilgilendirilen-ibareleri=8.
Not: K-290-listesinde-veli-kalemi-YOKTU-(uydurma-eklenmedi); firma-PRD'lerinde-veli-paneli-tespiti=firma-dönüş-turunda-(aday-madde). Ağaç-sayı-+0-(html+README-içerik-değişimi; ad-değişikliği). zip v6.45 (381; +0). EK 300.
~~~~

~~~~markdown
### K-651 — 09.09.2026 — SEDUVA GÜNCELLEMESİ 3. ADIM: SUPPORTA (MERKEZ) YÜZEYİ BAŞLATILDI
**Açıklama:** Kullanıcının "devam" onayı sonrasında, SEDUVA ailesinin 3. ayağı olan SUPPORTA (Merkez/Rehabilitasyon) modülünün geliştirilmesine geçilmiştir.
**İcra:** 
1. `SEDUVA_SUPPORTA/src/components/` dizini altında, rehabilitasyon eğitmenleri için "Support Fading" (Desteği Geri Çekme) ve "Recovery Profile" (Mola Sonrası Toparlanma) özelliklerini içeren `EgitmenDestekPaneli.tsx` bileşeni kodlanacaktır.
2. Bu sayede özel eğitim merkezi personelinin "Ne zaman ipucunu azaltmalıyım?" veya "Çocuğun moladan en verimli nasıl dönmesini sağlarım?" sorunlarına pedagojik (ve ölçülebilir) UX çözümleri sunulacaktır.
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
### K-708 — 10.09.2026 — SAHİBİN 3 PARÇALI TALİMATI: ① SEDUVA 12-MADDELİK İNCELEME KAPANIŞI ② BEP İKİ AİLE TESPİTİ ③ C-BULGULAR 1a/1b/1c
**Sahibin talebi (09.09, 3 parça):** (1) C-bulgular: 1a) F-1 K-598 Katman-1 CSV yeniden uygulansın (klon sonrası vaka.ts mimarisi) · 1b) F-2 yalnız ÖNERİ (otomatik geri-taşıma YOK) · 1c) plan v1.4 §8 bayat tablo + GORSEL-PARITE P-3 (TOSBİ→Kaptan Hece) doküman tazelemeleri onaylı; (2) "BEP hazırlık her iki ailede olmalı değil mi?"; (3) "12 maddelik SEDUVA incelemesinin önerileri uygulanmış mı?"
#### ③ SEDUVA 12-MADDELİK İNCELEME — DOĞRULAMA + TAMAMLAMA (kullanıcı-onaylı isimlerle yeniden uygulama)
**Doğrulama sonucu (ağaç kanıtlı):** defter K-659..667 "tamam+v7.64.31 teyitli" derdi; ağaçta uygulama **KISMİ** (src: Yaklaşım/Teknik ✓ · Gelişim Grafiği ✓ · Scholaria 5/5 ✓ · Supporta Eğitmen Kürsüsü ✓ · Persona ✓; EKSİK: Vaka Yönlendirici · Gözlem Kanıtları · Aile Bilgilendirme · MEB İle Uyumlama · Öğretmen Eşleme · Sistem Ayarları · Değerlendirme Ölçekleri · Gözlem İzleme · pano-kurum ×2 dup (pano ÖLÜ) · YASA-UI 18 string · default 'olcek') ve **4 build TAMAMİYLE STALE** (yeni adlar 0 · MENTORIA'da YASA-=19 · eski adlar canlı) · v7.64.x artefaktı diskte YOK (restore yolu kapalı → yerel yeniden-uygulama).
**Uygulanan (SEDUVA — src):**
- **MENTORIA:** 5 eksik nav adı + "Pedagojik Değerlendirme Bataryası"→"Değerlendirme Ölçekleri" · "Kanıt İzleme (T1/T2)"→"Gözlem İzleme" · ölü `pano` entry SİLİNDİ (Uzman Masası ×2 dup çözüldü; LayoutDashboard import temizliği) · açılış ekranı `'olcek'`→`'kurum'` (K-660; eski K-550 yorumu aşıldı) · **18 YASA- user-visible string temizlendi** (anlam korundu, kod düştü: 12+ dosya) · ölü `'uzman-masasi'` bloğu SİLİNDİ (15 satır — robotik metin kaynağı + tsc hatası) · "Guidance Navigator"→"Vaka Yönlendirici" (panel başlığı + 2 ekran başlığı + boş-durum metni + glossary) · "MEB Hizalama — Y2-A (salt-okunur)"→"MEB İle Uyumlama (salt-okunur)" · 2 UI string'de Z-12 kodu düştü ("üçgen gözlem").
- **SCHOLARIA:** "Hızlı-tur (PCV-brifing A–H)" bloğu Yardım sayfasından KALICI SİLİNDİ (K-665) · Portfoy'da "(Veli Köprüsü)"→"(Aile Bilgilendirme)".
- **SUPPORTA / PERSONA:** src dokunulmadı (uygulama zaten tam — yalnız build stale'idi).
**Rebuild + sürüm (build:tam; eski build K-88 kuralıyla silindi):** MENTORIA-TAM **v1.5.4** (438.858 B) · SCHOLARIA-MVP-TAM **v0.2.6** (299.772 B) · SUPPORTA-TAM **v0.8.8** (319.040 B) · package.json sürümleri + `__SURUM__` define ile build içi string'ler uyumlu.
**Doğrulama:** tsc --noEmit **3/3 TEMİZ** (3 mevcut-olmayan hata kapatıldı: ölü karşılaştırma + 2 kullanılmayan import) · SCHOLARIA smoke **12/12** · SUPPORTA smoke **127/127** (0 konsol) — SUPPORTA smoke'un 2 bayat beklentisi mevcut UI'a uyarlandı (rozet→surum-modu K-368 · oneri- akışı→"Kanıtı İncele ve YZ Önerisi Al" butonu + YZ EĞİTİMSEL DESTEK ÖNERİSİ textarea doğrulaması) · MENTORIA build içeriği: YASA-=0 · Navigator=0 · uzman-masasi-testid=0 · "Uzman Masası"=1 (tek entry) · yeni adların tümü >0 · SCHOLARIA: Hızlı-tur=0 · Veli Köprüsü=0 · 5 yeni ad ✓ · BEP=7 (korundu) · SUPPORTA: Eğitmen Kürsüsü=1 · Pano=0.
**Kalıntı şerhi:** Z-12/Z-17/FSI/TB/G_growth = açıklanamalı ALAN TERİMLERİ olarak KORUNDU (glossary'de tanımlı; menü YASA/Z kodu 0) · demo-profil varyantları (SCHOLARIA-MVP-v0.2.5.html · SUPPORTA-MVP-v0.8.7.html) pre-UX build olarak yerinde (inceleme kapsamı TAM ürünlerdi; tek komutla tazelenebilir) · MENTORIA smoke bu ağaçta yok (grep+tsc kanıtı yeterli görüldü; yeni smoke önerisi kuyrukta).
#### ② BEP HAZIRLIK — İKİ AİLEDE DE VAR (kullanıcı sorusu "değil mi?" → EVET)
- **LEXIVA Scholaria:** 10 src hit (App.tsx · **bep/BepHedef.tsx** K-558: kazanım→hedef-şablonu + gözlem-probu · portfoy/Portfoy.tsx · shell/Kabuk.tsx) · "resmî-BEP-DEĞİL" şerhli.
- **SEDUVA Scholaria:** build'de `{id:"bep",ad:"BEP Hazırlık"}` sekmesi + "Bu ekran resmî BEP belgesi ÜRETMEZ — sınıf-öncesi gözlem-hazırlaması" şerhi + 11 src hit.
- **SONUÇ:** 1:1 ayna doktriniyle tutarlı — **port gerekmez**; final raporda onay cümlesi.
#### ① C-BULGULAR
**1a) F-1 (K-598 Katman-1 CSV) — YENİDEN UYGULANDI (vaka.ts mimarisi; v7.64.21'deki uygulama klonla kaybolmuştu):**
- `src/data/vaka.ts`: `Katman1Oturumu` (9-kolon donuk şema — alan adları L4-1 §2/§5-① birebir) + `KATMAN1_CSV_KOLONLAR` (kilitli; ek-kolon AÇILMAZ) + `KATMAN1_OTURUMLARI` 12 MOCK satır (ÖĞR-4417: 7 akıcılık 42→74 + 3 yazma hata-sınıfı · ÖĞR-2903: 2 — TELEMETRI_TOHUM ile tutarlı; uyum H1-H2 flag'li) + logEvent muadili yerel sayaç (bu ağaçta telemetri busu YOK — şeffaf not).
- `ResmiSonuclar.tsx`: Katman-1 bölümüne **"Katman-1 CSV indir"** butonu (testid `l4-csv-indir` + `data-csv-adi`) → istemci-içi Blob `LEXIVA-L4-katman1-<vaka>.csv` (UTF-8 · virgüllü · başlık satırı şema-birebir · tırnaklı-virgül escape) · dosya cihazdan çıkmaz (K-05) · CSV veri-ürünü YOK (ihracat kullanıcıda).
- **LEXIVA Mentoria v2.10.0 → v2.11.0** (özellik-artışı; dosya adı politikasıyla; jüri paketi v2.10.0 etkilenmez — teslim edilmişti).
- **Yeni smoke** (`LEXIVA_MENTORIA/MENTORIA_TAM/smoke-test.cjs`; ağacın ilk Mentoria smoke'u): **12/12** — kabuk/sürüm(K-368) · buton görünürlüğü · GERÇEK indirme yakalama (dosya adı + başlık şema-birebir + veri ≥10 satır + her satır 9-alan + tırnaklı virgül + H1-H2 flag) · 0 konsol hatası.
**1b) F-2 (klon sürekliliği) — YALNIZ ÖNERİ (sahip kararı: otomatik uygulama YOK):**
- **Bulgu (disk kanıtlı):** (a) LEXIVA-L2 fork **v0.6.0** (P0-8: sınıf cetveli + dikkat sinyali + Dönem Özeti + sınıf özet CSV) build'i diskte YOK (LEXIVA_DEMO K-685/686'da silindi); mevcut Scholaria kendi okul yüzlerini taşıyor (BEP Hazırlık K-558 · izleme/rapor/veli · H-c transfer) ama P0-8'in cetvel/dönem-özet ekleri o isimlerle YOK (grep 0) — P0-8 dokümanı ORTAK-BELGELER'de geçerli. (b) Persona mevcut build'de 6 L1 yüzü VAR (Harf Dedektifi ×13 · Sözcük Çantası ×8 · Sayı Blokları ×13 · Odak Ritüeli ×3 · Kilometre ×2 · Yaş Bandı ×1); **4 isimli yüz YOK: Kelime Küpleri (E4) · Duygu Kartları (E5) · Matematik Merdiveni · Tekrar Turu/G11** (klon kendi görev seti + adaptif motorla geldi).
- **ÖNERİ (lean):** Kapanış/mühür turuna karıştırma — ayrı ürün turları, sahibin onayıyla: ① **jüri sonrası 1. ürün turu = P0-8 sınıf-operasyonu geri-taşıma** (LEXIVA L2/Scholaria aynası; B2B değeri yüksek — sınıf cetveli operasyonel merkez; K-524 donuk spec'i + 48/48 smoke tanımı checklist'te hazır — geri-taşıma = spec'ten yeniden-uygulama, artefakt diskte YOK). ② **4 L1 yüzü → pilot-sonrası içerik kuyruğu** (L1-6a/6b disipliniyle uyumlu); istisna önerisi: **Duygu Kartları (E5)** L1-6a kapı kararına (K-469) sahip → plandan sapma istenmezse diğerlerinden ÖNCE çekilebilir.
**1c) DOKÜMAN TAZELEMELERİ — UYGULANDI:**
- `LEXIVA-AILE-GELISTIRME-PLANI_v1.4.md` §8: bayat tablo senkronize (P0-5 ⏳→✅ v1.0 9-alan/V7/30-30 (K-517/518) · P0-4 ✅ 7-kriter/16-16 (K-519) · P0-2 ✅ 23/23 (K-520) · P0-6 ✅ 15×10/122-122 (K-521) · P0-7 ✅ 32/32 (K-522) · P0-3 ✅ 24/24 + K-05 dış-önşart (K-523) · P0-8 ✅ L2 v0.6.0 48/48 (K-524) + klon-süreklilik notu) + "§8-durum-güncellemesi (10.09 — K-708)" şerhi (F-1/F-2/GORSEL-PARITE çapraz referanslı).
- `LEXIVA-GORSEL-PARITE-DEGERLENDIRMESI_v1.0.md` → **v1.0.1**: P-3 + §3'teki 3 TOSBİ referansı → **Kaptan Hece** (K-701/K-703: kahraman = Kaptan Hece dost-robot — anten + ekran-göz; TOSBİ terk; teal/ÖGG palet + hece-dalgası korunur) + revizyon şerhi.
**Kalan küçük bulgular (sahip kararı beklemeye devam):** F-5 (L4-2/L4-3 v0.1 tasarımları eski mimariyi hedefler — tasarım-tarihi değeri korunur) · F-6 (a: "THE BRIEF" etiketi — öneri "SAHA GÖREVİ" · b: `cpts` değişken adı kalıntısı, yüzeye yansıma YOK).
**Mühür:** v7.65.22 çifti tarama ÖNCE silindi (K-706 kuralı; SHA zincirde) → **v7.65.23** (TESLIM-KAYDI'da).
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

### `VAMOLA - Seduva/SEDUVA_SUPPORTA/README.md` — belge bağlamı (tarihî envanter satırları güncel işlev kanıtı değil)
SHA `2abf7800c5bb0d491561af96019a94d48fe0f185a5f37159a8fa8576523c9ac5`

~~~~markdown
# SEDUVA Supporta — MVP Prototipi

**Sürüm:** v0.8.8 (K-708 yeniden-derleme; K-571 zenginleştirme-batch'i: A4 ipucu-kademesi · A2 görüşme-defteri · A1 DEP saat-izleri · A3 rapor-önerisi-TASLAĞI) — canonical `SUPPORTA-TAM-v0.8.8.html` (tek-dosya; çevrimdışı; kurulum-yok). K-710 notu: eski v0.8.7/PILOT/TAM SHA çapaları (K-571 seti) tarihseldir; K-708 build'inin SHA'sı mühür zincirindedir.
**v0.8.6→v0.8.7 (K-570/571):** ×3-künye + zarf-03-v0.8.7 + brifing-v1.1 — ayrıntı DEVAM-LOG_v0.8.7 · **v0.8.5→v0.8.6 (K-528):** artefakt + package.json v0.8.6 — README künyesi K-540'ta diske hizalandı (AUDIT v1.1 N-A).
**v0.2.0→v0.8.5 (03–05.09; K-313..K-408 özeti):** DEHB BGM yürütücü menüsü **BGM-12 canlı** (K-398) · **Aile Eğitim Merkezi** (K-407; `aile-sekme-*`/`aile-genel-*`/`aile-yazdir-*`) · 13 ekran · K-408 domain düzenlemesi (`SUPPORTA_*` klasörleri; eski `SEDUVA-SUPPORTA` adları tarihî) · K-02/K-08/K-14/K-15 TASLAK kalemler **bilinçli-erteli** (şirket sonrası tek paket). Ayrıntı: Strateji Defteri K-313..K-408. *(Başlık K-474 denetiminde tazelendi; aşağıdaki 0.1.x bölüm zinciri tarihî değerdedir.)*
**v0.1.6→v0.1.7 (K-312):** **Haftalık Ritim & Destek** ekranı-(11.) eklendi — Persona-7c-konseptinin-(K-305/307)-Supporta-uyarlaması: ①M2-haftalık-ritim-şablonu-(5-gün; haftada-1-hafif-gün; takvimle-uyum) ②kural-tabanlı-destek-önerileri-(yalnız-dosyanın-kendi-girdilerinden-zaman-iç; akran-karşılaştırması-yok; KC1/boş-durum-guard'lı) ③okul-ev-not-hattı-(DRC-tipi-haftalık-kart-taslağı; kopyala/yazdır; e-ileti-ÜRETİLMEZ; KC11-izin-notu-dosya-bazlı; veli/öğretmen=rapor-alıcısı-K-296) — şerhli; uygulama-kararı-ve-dozu-uzmanda.
**v0.1.5-jüri-dönüşü (K-304):** kullanıcı-v0.1.5'i-denedi — **'başarılı'**-(02.09); değişiklik-talebi-yok.
**v0.1.5→v0.1.6 (K-303):** çoklu-uzman/çakışma-senaryosu — kurgusal-kadro-(Uzman A/B; dosya-sorumlu-uzman-satırı) · oturumlara-uzman-ataması · **KC12:** aynı-uzman+aynı-saatte-ikinci-oturum-planı-takvimde-⚠'Çakışma-uyarısı'-(neg/pos-testli; uzman-değişince-uyarı-kalkar) · plan-çıktısına-'Uzman'-kolonu.
**Saklama-tablosu (K-302):** `_analiz/kvkk-saklama-sureleri-tablosu_v0.1.md`-(KVKK-m.4/2+İmha-Yön.-180g/6ay/3yıl; MEB-cetveli-süresiz vs rehab-10-yıl-çapası; avukat-onayı-AÇIK).
**v0.1.4→v0.1.5 (K-301):** terminoloji-düzeltmesi-(kullanıcı-uyarısı) — M7=**'Aile & Öğretmen İşbirliği'** · program-alanı='aile-bileşeni' · 'Ev ödevi + seans-başı izleme ritüeli'. Ekran-fonksiyonları-değişmedi.
**v0.1.3→v0.1.4 (K-300):** M1-dosya-kartına-bileşik-'**Onam & İzin**'-bloğu-(süreç-sözleşmesi · KVKK-aydınlatma+açık-rıza · veli-muvafakat-(EK-12-karşılığı) · e-ileti-izni) + **KC11:** e-ileti-izni-olmayan-dosyaya-hatırlatma/e-posta-taslağı-ÜRETİLMEZ-(mock-dosya-2=izinsiz-örnek; neg/pos-testli). Set-şablonları: `_analiz/supporta-onam-izin-seti_v0.1.md`-(K2/K3/K4+EK-12-karşılığı; avukat-onayı-AÇIK).
**v0.1.2→v0.1.3 (K-298):** 'Rapor Atölyesi'-sekmesi → **'Raporlar'**-(görünürlük-düzeltmesi; ekran-fonksiyonu-aynı). Form/evrak-envanteri: `_analiz/supporta-form-ve-evrak-envanteri_v0.1.md`-(3-katman: K/R/S; ÖEHY-EK-11/EK-12 · Aylık-PKT · Dönem-sonu-BPF kanıtları).
**v0.1.0→v0.1.1 (K-296):** veli-erişimi-KALDIRILDI — Persona-dışı-ürünlerde-veli-sistem-oturumu-yoktur; veli **bilgilendirilen + veri-kaynağı** pozisyonundadır. Eski-'Veli-bakışı'-ekranı → 'Aile-Bilgilendirmesi'-(uzman/yönetici-kullanımlı-çıktı + vekâleten-beyan-işleme). Rol-modeli-2-(uzman+yönetici).
**v0.1.1→v0.1.2 (K-297):** **Çıkış-&-İletişim-ekranı** eklendi — ①haftalık-çalışma-planı-çıktısı-(Yazdır+print-CSS; şerh+mühür-baskıda-kalır) ②randevu-hatırlatma-metni-taslağı-(hizmet-ileti-kalıbı; çocuk-adı/tanı-yok; taşıyıcı-SMS=FAZ-2) ③e-posta-taslağı-(yalnız-onaylı-rapor; maskeli-UID+VMPAK-parola-notu+İYS-promosyon-yok) ④M1'e-'elektronik-bilgilendirme-izni'-alanı. Süreç-sözleşmesi-şablonu: `_analiz/supporta-surec-sozlesmesi-sablonu_v0.1.md`-(avukat-onayı-AÇIK).
**Kapsam-mührü (D2-kararı — K-334 düzeltmesi 05.09):** İZLEME + İÇERİK + TEMEL-İŞLETME. **Kapsam dışı (kurum otomasyonu): MEBBİS/e-Okul entegrasyonu + e-fatura / idari-mali (K-334, K-331).** Faz-2 (prototipte-YOK, iletişim/teknik): SMS hatırlatma taslağı (≤160, yerel-önce) · donanım-telemetri (opsiyonel) · çoklu-şube (C-2).
**Kaynak-spec:** `VAMOLA/_analiz/supporta-mvp-spec_v0.1.md` (K-291; K-296/297-ekileri) ← `seduva-4urun-icerik-cercevesi_v0.1.md` (K-289; K-295/296-ekileri) · form/evrak-envanteri: `supporta-form-ve-evrak-envanteri_v0.1.md` (K-298) · iletişim: `supporta-operasyon-cikti-ve-iletisim-katmani_v0.1.md` (K-297).

## Modüller (M1–M7)
M1 Dosya&Kayıt-(EDİF-referans-alanlar+rıza+UID; veli-iletişim-bloğu=kurum-kayıt-verisi) · M2 Takvim/Oturum-(4-durum; çakışma; 40-dk) · M3 Oturum-atölyesi · M4 Etkinlik&Hedef-kataloğu-(SP-kod-şeması) · M5 Girdi&Çizelge-motoru-(x+/0–3/Evet-Hayır) · M6 Rapor-atölyesi-(6-tür; taslak-mührü; onay; 2-kopya) · M7 Aile&Öğretmen-İşbirliği-(öneri-bloğu; **ritim-(v0.1.7): haftalık-ritim-şablonu+kural-tabanlı-öneri+okul-ev-not-hattı**; ödev+seans-başı-izleme; vekâleten-veli-beyanı; K-301-ad-değişikliği) · **M7b Aile-Bilgilendirmesi-(K-296: onaylı-rapor-çıktısı + vekâleten-beyan-girişi; veli-oturumu-yok)**.

## Kabul-kriterleri (test-kaskadı-02.09-KANITLI)
| KC | Kural | Sonuç |
|---|---|---|
| KC1 | etkinliksiz-girdi-GİRELEMEZ (ekran+kod-guard) | ✓-(neg/pos-çift-koşu) |
| KC2 | onaysız-rapor-'geçerli-belge-değildir'mührü; aktarılamaz (alert-kanıtlı) | ✓-(neg/pos-çift-koşu) |
| KC3 | şerh-blokları-silinemez/kapatılamaz (data-sherh; sabit-kütüphane) | ✓ |
| KC4 | akran-karşılaştırması-YOK (şerh + sıralama-kodu-0-hit) | ✓ |
| KC5 | 2-kopya-deseni-(kurum-kopyası + maskeli-UID-iletişim-kopyası) | ✓ |
| KC6 | yalnız-kurgusal-mock-'Öğrenci/2. Sınıf/8–10'-(K-270); gerçek-çocuk-verisi-yok | ✓ |
| **KC7-YENİ** | **veli-erişimi-YOK: ROLLER'da-veli-yok-(2-rol) · eVeli/'Veli-bakışı'-yok · beyan-vekâleten-(uzman-işler) · bilgilendirme-çıktısı-uzman-kullanımlı** | ✓ |
| **KC8-YENİ** | yazdırma-çıktısında-şerh+TASLAK/Uzman-onaylı-mührü-görünür-(print-CSS-gizlemez) | ✓ |
| **KC9-YENİ** | hatırlatma/e-posta-metninde-çocuk-adı+tanı-0-hit; SMS-taslağı-≤160-karakter | ✓-(131-karakter-kanıtlı) |
| **KC10-YENİ** | onaysız-raporla-e-posta-ek-hazırlığı-OLMAZ-(alert+bos-taslak); onaylıda-UID+İYS-promosyon-yok-ibaresi | ✓-(neg/pos-çift-koşu) |
| **KC11-YENİ** | e-ileti-izni-olmayan-dosyaya-hatırlatma/e-posta-taslağı-üretilmez-(M1-onam-bloğu-esas; izinsiz-mock-dosya-kanıtı) | ✓-(neg/pos-çift-koşu) |
| **KC12-YENİ** | aynı-uzman+aynı-saatte-ikinci-oturum → takvimde-⚠'Çakışma-uyarısı'; uzman-değişince-uyarı-kalkar; plan-çıktısında-'Uzman'-kolonu | ✓-(neg/pos-çift-koşu) |

Dil-kapısı (K-281/282-uyum): riskli-terimler-yalnız-şerh-cümlelerinde; **milisaniye/nörofeedback/Berard/Tomatis=0-hit**; meta-disclaimer-'tanı/tedavi içermez'. Test-yöntemi: `node --check` + DOM-stub-smoke-(11-ekran ×2-rol; KC1/KC2/KC10-negatif+pozitif-çift-koşu) + statik-grep — 02.09-koşusu-tam-yeşil.

## Daimî-kurallar
Şerh-kütüphanesi-sabit-(6-blok) · K-263-form-yerine-geçme-YOK · K-88-içerik-kopyası-YOK-(MEB-SDB/DEP=yapı-referans) · K-05-prototipte-gerçek-çocuk-verisi-YOK · rapor-onayı-yalnız-yöneticide-(uzman-kendi-raporunu-onaylayamaz) · **K-296-veli-oturumu-YOK-(Persona-dışı-ürün-kuralı; veli=bilgilendirilen+veri-kaynağı)** · sürüm-adı-yalnız-rol-seçim-ekranında ('Prototip v0.1.1').

## Açık-maddeler (sonraki-turlar)
saha-fiyat-kanıtı · MEBBİS-teknik-yolu-(faz-2-on-inceleme) · sözleşme-şablonu-avukat-onayı-(K-297) · İYS-kayıt/3.parti-SMS-taşıyıcı-seçimi-(FAZ-2) · KVKK-saklama-politikasının-kurum-onayı-(tablo-K-302'yle-çapa). *(KAPANDI: 'veli-bakışı-kanalı'-(K-296) · 'çoklu-uzman-çakışma-senaryoları'-(K-303; v0.1.6) · 'jüri-geri-bildirim-döngüsü'-(K-304; v0.1.5-denendi-başarılı) · 'M7-Haftalık-Ritim-inşası'-(K-312; v0.1.7).)*

~~~~

### `VAMOLA - Lexiva/LEXIVA_SUPPORTA/SUPPORTA_TAM/README.md` — belge bağlamı (tarihî envanter satırları güncel işlev kanıtı değil)
SHA `b9863a4f842e96ba0506d0606b523884dfd55f9629cd1089661bd403833d6c8c`

~~~~markdown
# LEXIVA Supporta — Yapılandırılmış Özel Eğitim Destek Ortamı (MVP)

**Sürüm:** v2.10.0 — tek-dosya çevrimdışı build: `LEXIVA-SUPPORTA-v2.10.0.html` · kurulum-yok · DEMO/PILOT/TAM setleri `SUPPORTA_DEMO/PILOT/TAM` outDir'lerinde (build-zamanlı; dist* mühür-dışı)

## Konumlandırma (K-683 / K-700)
LEXIVA Supporta, **yapılandırılmış özel eğitim destek ortamıdır**: uzman (özel eğitim öğretmeni / psikolojik danışman) için dosya-kayıt, takvim/oturum atölyesi, etkinlik kataloğu (DEP + okuma menüsü), girdi/çizelge motoru ve rapor atölyesi. Tanı koymaz, tedavi iddiası taşımaz (K-02); **uygulama içi test UYGULANMAZ** (OLCUM-ARACLARI v0.2). SEDUVA'daki DEHB yürütücü-işlev BGM-12 menüsü devredilmez; yerini **EQ kodlu okuma/fonolojik içerik menüsü** (müfredat matrisi v0.3 + 2021 DEP hiza) alır.

## Modüller (M1–M7)
M1 Dosya&Kayıt (EDİF referans alanları + rıza + UID; veli iletişim bloğu = kurum kayıt verisi) · M2 Takvim/Oturum (4 durum; çakışma; 40 dk) · M3 Oturum atölyesi · M4 Etkinlik&Hedef kataloğu (DEP + BGM okuma menüsü; SP kod şeması) · M5 Girdi&Çizelge motoru (x+/0–3/Evet-Hayır) · M6 Rapor atölyesi (6 tür; taslak mührü; onay; 2 kopya) · M7 Aile&Öğretmen İşbirliği (öneri bloğu; haftalık ritim + kural tabanlı öneri; okul-ev not hattı; ödev + seans başı izleme; vekâleten veli beyanı) · M7b Aile Bilgilendirmesi (onaylı rapor çıktısı + vekâleten beyan; veli oturumu yok).

## Okuma menüsü (BGM katmanı — EQ-01..12)
EQ-01 Ses Merdiveni · EQ-02 Ses Birimi Ayırt Etme · EQ-03 Hece ve Parçalar · EQ-04 Harf Tanıma ve Çizim · EQ-05 Söyleneni Yaz · EQ-06 Akıcı Okuma (M-4) · EQ-07 Sözcük Çantası · EQ-08 Anlama Kartı · EQ-09 Sayı Blokları · EQ-10 Süre Algısı · EQ-11 Transfer ve Serbest Okuma · EQ-12 Okuma Özerkliği. Sıralı modül YOKTUR — seçim uzmanındadır (MODUL_SECIM_SERBEST).

## Kabul kriterleri (spec §9, KC1–KC15)
eylemsiz girdi giremez · onaysız rapor "geçerli belge değildir" mührü · şerh blokları silinemez · akran karşılaştırması yok · 2 kopya deseni · yalnız kurgusal mock veri (K-05/K-270) · veli erişimi YOK (2 rol) · e-ileti izni yoksa hatırlatma/taşıyıcı üretilmez · SMS taslağında çocuk adı/tanı yok (≤160, yerel-önce).

## Kapsam mührü
İZLEME + İÇERİK + TEMEL-İŞLETME. Kapsam dışı: MEBBİS/e-Okul entegrasyonu, e-fatura/idari-mali. Faz-2 (prototipte yok): SMS taşıyıcı, donanım telemetri (opsiyonel), çoklu şube.

## Notlar
- K-02: bant/eşik/normalite dili yok; uygulama içi test yok — ölçüm = kendi telemetrisi + resmî sonuç aktarımı + gözlem taksonomisi.
- K-08: MEB cümleleri kopyalanmaz, kavram taşınır (aile kartları ÖGG Aile Rehberi kaynaklı).
- Aile Eğitim Merkezi: `AILE_EGITIM/` + `src/data/aile/` + `src/components/aile/` (AG-1..5 önleyici kartlar + baskı şablonları).
- Smoke: `node smoke-test.cjs [html|url]` (playwright-core; EQ kodlu BGM akışı dahil).

~~~~

### `VAMOLA - Lexiva/LEXIVA_SUPPORTA/LEXIVA-SUPPORTA-DEP-PLANLAYICI-KAPSAM_v0.1.md` — belge bağlamı (tarihî envanter satırları güncel işlev kanıtı değil)
SHA `77ddebd7fd28fa2ac0a8fd14fa4e80f2a6b5b1eea00644f0c34c37cfd6973cd9`

~~~~markdown
# LEXIVA·SUPPORTA — DEP PLANLAYICI KAPSAM BELGESİ v0.1 (P-1 · K-589) — TASLAK (kuyruk-önerisiyle-P-2'ye-geçer)

**VAMOLA EduLabs** (D-1) · 08.09.2026 · **Konum:** `LEXIVA_SUPPORTA/` 2. belge · **Yürütme:** kuyruk-v4 **P-1** (kullanıcı-K-588-ilkesi + "kuyruk-öneriye-göre-ilerlesin" duran-kuralı).
**K-588 şerhi:** Bu belge **kanon-temelli** yazıldı — saha-doğrulaması (L3-1'in-2-3-kurum-görüşmesi) LEXIVA-PCV **L3-üye-zarfının dönüşüne** devredildi; saha-bloğu-kaldırıldı.
**Zemin kanonları:** L3-1 Saha Turu Planı v1.0 KİLİT (K-448; 22-soru-seti → §7'de-yeni-rol) · Y-1 Kart-Bazlı Rakip Taraması v2.0 §3 (MEB **Özel Eğitim Modülü** keşfi [K6] · todi-COGNİT/APAMER [K7] · yerel-yazılım-boşluğu-hipotezi) · DERS-ENTEGRASYONU-VE-BEP-KÖPRÜSÜ v2.0 (K-369) · **BEP FORM EŞLEMESİ v1.0 (K-370: EK-1…EK-7)** · ÖEKY çerçevesi (RAM-yönlendirmeli **aylık 8 bireysel + 4 grup** saat; md.3-merkezî-modül; md.16-"destekleyici dijital eğitim materyalleri"/"destekleyici mahiyette") · Ürün-Kartı-L3 (BECERİ-MİMARİSİ-URUN-KARTLARI v1.1): **DEP modül-saat hizalı planlama + eğitmen koltuğu + kurum paneli** · Klasör Düzeni v1.0.
**Kurallar:** K-02 (ölçen-değil-gözlemleyen) · K-04 (firma-verisi-ayrımı) · K-05 (sunucusuz) · K-08 (alıntı-yok) · K-263 (resmî-formun-yerine-geçmez) · Z-15 (akran-sıralaması-yok).

---

## §1 — Değer önerisi (Kart L3'ün-üye-konumlandırması)

- **Kim:** MEB onaylı **özel eğitim ve rehabilitasyon merkezleri** (Profil-A) + çocuk gelişim/özel eğitim merkezleri (Profil-B) — kullanıcı: **merkez uzmanı/eğitmen** + kurum yönetimi (satın-alıcı).
- **Ne:** L3 = merkez-hattı-üye; **üç yüz**:
  1. **DEP Planlayıcı** — modül×bölüm×saat hizalı oturum-planı (8+4-çerçeve-görselleştirmesi; RAM-rapor-girdisi-MOCK-alanı).
  2. **Eğitmen Koltuğu** — oturum-içi-yüzey (plan + zaman-çizelgesi + destek-hatırlatıcıları; L2-OturumPlanı-deseni-ama-merkez-bakışı).
  3. **Kurum Paneli** — çoklu-vaka-tablosu (MOCK; anonim-kodlu) + ilerleme-özeti (yargısız-dil).
- **Resmî dayanak:** ÖEKY-destek-eğitim-saatleri-çerçevesi (8+4) · mevzuatın-2024-"destekleyici dijital eğitim materyalleri"-cümlesi · DEP-uygulama-akışı (merkez-profilinde-DEP-2021; resmî-form-kesitleri-kanonu: DEP-2026-öğrenme-güçlüğü-ekleri — şerh: sürüm-ayrımı-PCV-L3-dönüşünde-netleşir).
- **L2-ile-çizgi:** L2-okul-içi (öğretmen; ders-istasyonu-+BEP-kanıt) · L3-kurumsal-merkez (eğitmen; vaka-portföyü-+DEP-saat-planı). Üç-bağlam-tablosundaki-"destek eğitim odası"-hizası-L2'de-kalır; L3-bu-tabloya-girmez, ÖEKY-çerçevesiyle-ayrışır.

## §2 — "Özel Eğitim Modülü DOSTU" ilkesi (Y-1-keşfi-K6'dan-bu-belgeye)

MEB-Özel-Eğitim-Modülü (ÖEKY md.3): kayıtlı-birey/personel/kurum-verisinin-**merkezî-veri-tabanında**-toplandığı-zorunlu-yazılım. **L3-bu-modülün-veri-ikizi-DEĞİL.** Üç-çakışma-yasağı:
1. Kayıtlı-birey/personel/kurum-sicil-verisi-DEPOLAMAZ (modülün-alanı).
2. Yoklama/devamsızlık/resmî-işlem-İŞLEMEZ.
3. Resmî-form-DOLDURMAZ (K-263-deseni; §4'teki-kanıt-yalnız-"hazırlayıcı-özet").
**Değer-katmanı** (modülün-değindiği-yer): DEP-modül-saat-planlama · eğitmen-oturum-koltuğu · ilerleme-özeti. Her-yüzeyde-md.16-türü-bilgi-notu: *"destekleyici mahiyette; resmî kayıt/belgenin yerine geçmez."*

## §3 — Yüz-yüzeyleri (P-2-fork-iskelet-girdisi)

| Yüz | Bileşenler (MOCK + K-05-etiketi) | Telemetri-adayları |
|---|---|---|
| DEP Planlayıcı | modül×bölüm×saat-ızgarası · 8+4-saat-sayacı (çerçeve-gösterimi; denetim-DEĞİL) · RAM-raporu-girdi-alanı-mock | `l3_plan_degisiklik` · `l3_plan_oturum_kuruldu` |
| Eğitmen Koltuğu | günün-planı · oturum-akış-hatırlatıcısı · görev-bağlantısı-gösterimi (L1-içerik-köprüsü-görünüm) | `l3_koltuk_oturum` |
| Kurum Paneli | vaka-tablosu (A/B/C-anonim-kod) · ilerleme-özeti-bandı (destek-kullanımı-sıklığı; puan-yok) | `l3_panel_goruntuleme` |

**Fork-profili:** K-466-deseni — tek-src + `__L3_PROFIL__` derleme-bayrağı; çocuk-akışı-değişmez, **öğretmen-yüzü-→-merkez-yüzü**; sürüm-hattı: **LEXIVA-L3-v0.1.0** (L2-v0.6.2-paralel-üye-hattı).

## §4 — DEP kanıt ihracı (K-370-eşlemesinin-merkez-uyarlaması)

- L2-deseniyle-**ortak-bileşen**: EK-4/EK-5-sütun-başlıklarıyla-tek-sayfa-kanıt-özeti (oturum-sayısı · tekrar · hata-matrisi-"ne-oldu"-kayıtları) + CSV/Yazdır.
- K-370-çevirisi: hata-matrisi→**EK-5 "Ulaşılamama Nedenleri"/"Öneriler"** 🟢 · resmî-bant→**EK-3 performans-düzeyi** 🟡 (uzman-yorumuyla) · **EK-6-portfolyo-çapası** (merkez-farkı): kurum+RAM-onay-akışına-giden-portfolyo-klasörünün-**kanıt-eklerini-hazırlar**, formu-işaretlemez.
- Ekran-dili: bant/düzey-çocuğa-GÖSTERİLMEZ (K-02); uzman-eğitmen-görünümünde-kalır.

## §5 — Veri-sözleşmesi (K-05)

Yerel-localStorage · çocuk-gerçek-verisi-YOK (MOCK A1..A8) · dışa-aktarım-yalnız-yerel-JSON/CSV · bulut-hesap-yok · kayıt-süresi/audit-ilkeleri-G12'de (uzun-vade-şerhi).

## §6 — Rakip-ayrışması (Y-1-§3'ten)

| Rakip/desen | Ayrışma-dili |
|---|---|
| **todi-COGNİT/APAMER** (K7; FİRMA VERİSİ) | onlar: CHC-bilişsel-müdahale + ücretli-uygulayıcı-eğitimi-paketi; **L3: resmî-DEP-taksonomisi + beceri-inşası + eğitmen-koltuğu** (eğitim-paketi-satışı-kapsam-DIŞI) |
| **MEB-Özel-Eğitim-Modülü** | §2-dostu-ilkesi (tamamlayıcı; veri-ikisi-değil) |
| Yerel-kurum-yazılımı | taramada-görünmedi → boşluk-hipotezi; doğrulaması **PCV-L3-dönüşünde** (K-276: beyan-tarama-sınırlı-şerhi) |

## §7 — L3-1'in-22-soru-setinin-yeni-rolü (K-588)

Soru-seti-KİLİT-korunur; **LEXIVA-PCV-L3-üye-zarfının-değerlendirme-çerçevesi** olur: merkez-uzmanı-L3'ü-blok-A..F-merceğinden-değerlendirir (A-kurum-profiline-uygunluk · B-planlama-ihtiyacını-karşılar-mı · C-koltuk/panel · D-modül-dostluğu+güven · E-model · F-KVKK-çekincesi). K-04-firma-verisi-kuralları-dönüş-işlemede-aynen.

## §8 — Açık kalemler (P-2/PCV-sonrası)

1. `l3_*`-olay-adlarının-omurga-şemasına-kayıtı (OM-3-disiplini; P-2'de).
2. Kurum-paneli-vaka-sayısı-bandı (8-çekirdek? genişletilebilir-mock?) — P-2-derleme-kararı.
3. Eğitmen-Koltuğu'nun-L2-OturumPlanı-ile-bileşen-paylaşımı (ortak-src-bileşen-vs-ayrık) — P-2-kod-kararı.
4. DEP-2021/2026-sürüm-ayrımı-dili — PCV-L3-dönüşünde-kesinleşir.

## §9 — ONAY MATRİSİ (duran-kural: kuyruk-önerisi-default; kullanıcı-veto-hakkı-daimî)

| # | Karar | Öneri (P-2-bununla-açılır) |
|---|---|---|
| 1 | P-2-kapsamı: üç-yüz-minimal (§3) | ✅ hepsi-tek-fork-turunda |
| 2 | Veri: MOCK+yerel (§5) | ✅ K-05-aynen |
| 3 | EK-4/5-kanıt-bileşeni-L2-deseniyle-ortak | ✅ paylaş |
| 4 | Sürüm: L3-v0.1.0-bağımsız-üye-hattı | ✅ |

---
*VAMOLA EduLabs — L3-2 (P-1) kanon-temelli-taslak; saha-değerlendirmesi-LEXIVA-PCV-L3-zarfı-dönüşünde (K-588). Sıradaki: P-2 L3-fork-iskeleti.*

~~~~

# Ek C-SED — SUPPORTA-SED bağımsız kanıt havuzu

## DOM35 durum / seçilmiş akışlar

### SUP-SED-DOM-uzman-rol-secimi

~~~~text
S
SEDUVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)

Özel eğitim merkezi uzman kokpiti · v0.8.8

Devam etmek için rolünüzü seçin.

Yönetici
Tüm dosyalar · rapor onayı · dışa aktarma
Uzman / Eğitimci
Kendi dosyaları · oturum · girdi · rapor taslağı

Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
~~~~

### SUP-SED-DOM-uzman-nav-pano

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif

Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.

T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)
2026-09-10 10:00 — ÖĞR-4417 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
2026-09-03 10:00 — ÖĞR-2903 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
Onay Bekleyen Raporlar (Human-Accountable AI)
4
• Seans Özeti — 03.09.2026
• Dönem Sonu Değerlendirme — 2026 Güz
• BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
• RAM İzleme Paketi Hazırlığı

YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).
~~~~

### SUP-SED-DOM-uzman-nav-dosyalar

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Dosya listesi
ÖĞR-4417
ÖĞR-2903
Dosya kartı — ÖĞR-4417
Ad (maskeli)
Öğrenci A. (2. Sınıf)
Doğum
2018-04-12
Okul / Sınıf
Atatürk İlkokulu / 2-B
Devamsızlık
Son ayda 2 gün
Veli
Veli A. · 05xx xxx 41 17
Rıza kaydı
2026-08-20
Geçmiş BEP
RAM eğitsel değerlendirme mevcut (2025)
Program kartı
Seans sayısı
24
Sıklık
Haftada 1 (40 dk)
Aile bileşeni
Var
RAM rapor ref.
RAM-2025/1184
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-SED-DOM-uzman-nav-takvim

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Oturum takvimi
2026-09-03 haftası
Çakışma: 2026-09-03 10:00 UZM-1 (KC12)
Tarih	Saat	Dosya	Uzman	Durum
2026-09-03	10:00	ÖĞR-4417	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

2026-09-03	10:00	ÖĞR-2903	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

Durumlar: planlandı · tamamlandı · iptal · gelmedi · değişiklikler bu cihazda saklanır.

Veli görüşme-randevu defteri (K-571/A2)
hatırlatma gönderilmez — K-334
Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
Tarih
Konu
Deftere ekle

Defter boş — ilk görüşme kaydını ekleyin.

Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).
~~~~

### SUP-SED-DOM-uzman-nav-oturum

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Oturum kartı — OT-101

Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı

Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)

Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
ⓘ
Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)
Bu oturumda seçili BGM modülleri
ÖĞR-4417 · sıra uzmanın
FS-1 · Odak Kararlılığı BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M1
CA-4 · Bilgi Mimarisi BGM
5 dk · girdi: 0-3 · DEP köprüsü M1
II-6 · Dürtü Engelleme BGM
6 dk · girdi: Evet / Hayır · DEP köprüsü M6

BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez.

Hızlı girdi paneli
YASA-1 etkin
Etkinlik *zorunlu
— etkinlik seçin —
Hece ayırma çalışması (3.1.2)
Sesli okuma — tekrarlı (3.3.1)
Görsel dikkat eşleme (1.1.3)
İşitsel bellek dizisi (1.2.1)
Sözcük dağarcığı — nesne adlandırma (2.2.1)
Nesne niteliği ayırt etme (4.1.2)
Ritmik sayma (100 içinde) (5.1.4)
Sıra alma ve bekleme (6.2.3)
Sürdürülebilir dikkat — nesne takibi (1.3.2)
Yönerge izleme (2 adımlı) (1.4.1)
Dinlediğini anlama — kısa öykü (2.1.3)
Sözel ifade — cümle kurma (2.3.2)
Karşılıklı konuşma sürdürme (2.4.1)
Harf-ses eşleme (3.2.1)
Yazma — harf dikte (3.4.2)
Gruplama / sınıflama (4.2.3)
Birebir eşleştirme (4.3.1)
Sıralama (büyük-küçük) (4.4.2)
Sayı doğrusu ile toplama (5.2.2)
Çıkarma (nesne ile) (5.2.4)
Günlük yaşam problemi kurma (5.3.1)
Duygu tanıma (6.1.2)
İş birliği oyunu (6.3.1)
Kurala uyma (oyun) (6.3.3)
BGM — Odak Kararlılığı (Hedefi Yakala) (BGM-FS-1)
BGM — Zaman Algısı (Kum Saati Tahmini) (BGM-TPM-2)
BGM — Parçalama (Üç Kart) (BGM-CC-3)
BGM — Bilgi Mimarisi (Sayı Dedektifi) (BGM-CA-4)
BGM — Bilişsel Esneklik (Renk mi Şekil mi?) (BGM-CS-5)
BGM — Dürtü Engelleme (Işık Yakala + 3 Adım) (BGM-II-6)
BGM — Düzenleme Desteği (Nefes Halkası) (BGM-SR-7)
BGM — Önceliklendirme (Önce Hangisi?) (BGM-SP-8)
BGM — Sosyal İpucu (Sıra Çubuğu) (BGM-SR-9)
BGM — Çift Kanal (Çift Görev) (BGM-DS-10)
BGM — Yüksek Yük (Karışık Tur) (BGM-CM-11)
BGM — Kendini Yönetme (Kendi Planım) (BGM-TM-12)
[BGM] FS-1 · Odak Kararlılığı
[BGM] CA-4 · Bilgi Mimarisi
[BGM] II-6 · Dürtü Engelleme
Kodlama
x / +
0-3
Evet / Hayır
Değer
Gözlenen ipucu-kademesi (K-571/A4)
— seçilmeyebilir —
Model
Sözel
Bağımsız
Girdi kaydet

Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.

• Hece ayırma çalışması → + (x / +)
• Sesli okuma — tekrarlı → 2 (0-3)
• Görsel dikkat eşleme → Evet (Evet / Hayır)
~~~~

### SUP-SED-DOM-uzman-nav-katalog

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Etkinlik ve hedef davranış kataloğu
36 / 36 etkinlik · DEP 24 · BGM 12
Tümü (36)
DEP-2026 (24)
BGM-12 (12)
Tümü
Öğrenmeye Destek
Dil ve İletişim
Okuma ve Yazma
Erken Matematik
Matematik
Sosyal Etkileşim
Yeni etkinlik ekle · kayıt bu cihazda saklanır
DEP-2026
BGM-12
M1 · Öğrenmeye Destek
M2 · Dil ve İletişim
M3 · Okuma ve Yazma
M4 · Erken Matematik
M5 · Matematik
M6 · Sosyal Etkileşim
Ekle
Varsayılana sıfırla
Hece ayırma çalışması
3.1.2
Okuma ve Yazma · DEP
İpucu kademesi: Sözel ipucu → model → bağımsız
Malzeme: hece kartları · çalışma yaprağı
Düzenle
Sil
Sesli okuma — tekrarlı
3.3.1
Okuma ve Yazma · DEP
İpucu kademesi: Eşli okuma → bağımsız
Malzeme: kısa metin · kronometre
Düzenle
Sil
Görsel dikkat eşleme
1.1.3
Öğrenmeye Destek · DEP
İpucu kademesi: İşaret → sözel → bağımsız
Malzeme: eşleme kartları
Düzenle
Sil
İşitsel bellek dizisi
1.2.1
Öğrenmeye Destek · DEP
İpucu kademesi: Model → gecikmeli model → bağımsız
Malzeme: ses kartları
Düzenle
Sil
Sözcük dağarcığı — nesne adlandırma
2.2.1
Dil ve İletişim · DEP
İpucu kademesi: Fiziksel ipucu → sözel → bağımsız
Malzeme: nesne resimleri
Düzenle
Sil
Nesne niteliği ayırt etme
4.1.2
Erken Matematik · DEP
İpucu kademesi: Model → kısmi ipucu → bağımsız
Malzeme: blok seti
Düzenle
Sil
Ritmik sayma (100 içinde)
5.1.4
Matematik · DEP
İpucu kademesi: Birlikte sayma → bağımsız
Malzeme: sayı doğrusu
Düzenle
Sil
Sıra alma ve bekleme
6.2.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → sözel hatırlatma → bağımsız
Malzeme: sıra kartı · kum saati
Düzenle
Sil
Sürdürülebilir dikkat — nesne takibi
1.3.2
Öğrenmeye Destek · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: renkli toplar · tepsi
Düzenle
Sil
Yönerge izleme (2 adımlı)
1.4.1
Öğrenmeye Destek · DEP
İpucu kademesi: Fiziksel rehber → sözel → bağımsız
Malzeme: yönerge kartları
Düzenle
Sil
Dinlediğini anlama — kısa öykü
2.1.3
Dil ve İletişim · DEP
İpucu kademesi: Sözel ipucu → soru-cevap → bağımsız
Malzeme: öykü kartı · soru listesi
Düzenle
Sil
Sözel ifade — cümle kurma
2.3.2
Dil ve İletişim · DEP
İpucu kademesi: Model cümle → tamamlama → bağımsız
Malzeme: kelime kartları
Düzenle
Sil
Karşılıklı konuşma sürdürme
2.4.1
Dil ve İletişim · DEP
İpucu kademesi: Sözel başlatma → sıra alma → bağımsız
Malzeme: konu kartları · kum saati
Düzenle
Sil
Harf-ses eşleme
3.2.1
Okuma ve Yazma · DEP
İpucu kademesi: Model → eşleme → bağımsız
Malzeme: harf kartları · ses kutusu
Düzenle
Sil
Yazma — harf dikte
3.4.2
Okuma ve Yazma · DEP
İpucu kademesi: Noktalı iz → kopya → bağımsız
Malzeme: dikte yaprağı · kalem
Düzenle
Sil
Gruplama / sınıflama
4.2.3
Erken Matematik · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: sınıflama kutuları · nesneler
Düzenle
Sil
Birebir eşleştirme
4.3.1
Erken Matematik · DEP
İpucu kademesi: Fiziksel rehber → bağımsız
Malzeme: eş kartları
Düzenle
Sil
Sıralama (büyük-küçük)
4.4.2
Erken Matematik · DEP
İpucu kademesi: Model → deneme-yanılma → bağımsız
Malzeme: sıralama şeridi
Düzenle
Sil
Sayı doğrusu ile toplama
5.2.2
Matematik · DEP
İpucu kademesi: Model → rehberli → bağımsız
Malzeme: sayı doğrusu · pul
Düzenle
Sil
Çıkarma (nesne ile)
5.2.4
Matematik · DEP
İpucu kademesi: Nesne desteği → zihinden
Malzeme: sayma pulları
Düzenle
Sil
Günlük yaşam problemi kurma
5.3.1
Matematik · DEP
İpucu kademesi: Sözel senaryo → model → bağımsız
Malzeme: problem kartları
Düzenle
Sil
Duygu tanıma
6.1.2
Sosyal Etkileşim · DEP
İpucu kademesi: Görsel ipucu → eşleme → bağımsız
Malzeme: duygu kartları
Düzenle
Sil
İş birliği oyunu
6.3.1
Sosyal Etkileşim · DEP
İpucu kademesi: Eşli oyun → sıra alma → bağımsız
Malzeme: kutu oyunu
Düzenle
Sil
Kurala uyma (oyun)
6.3.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → hatırlatma → bağımsız
Malzeme: kural kartı
Düzenle
Sil
BGM — Odak Kararlılığı (Hedefi Yakala) BGM
BGM-FS-1
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: tarama kart seti · kum saati
Düzenle
Sil
BGM — Zaman Algısı (Kum Saati Tahmini) BGM
BGM-TPM-2
BGM-12 · BGM
İpucu kademesi: Görsel sayaç açık → yarı kapalı → kapalı
Malzeme: kum saati · tahmin kartı
Düzenle
Sil
BGM — Parçalama (Üç Kart) BGM
BGM-CC-3
BGM-12 · BGM
İpucu kademesi: Model (uzman böler) → sözel → bağımsız
Malzeme: çalışma yaprağı · 3 boş kart · kalem
Düzenle
Sil
BGM — Bilgi Mimarisi (Sayı Dedektifi) BGM
BGM-CA-4
BGM-12 · BGM
İpucu kademesi: Görsel destek açık → kademeli kalkar
Malzeme: sayı/nesne kartları · küçük tahta
Düzenle
Sil
BGM — Bilişsel Esneklik (Renk mi Şekil mi?) BGM
BGM-CS-5
BGM-12 · BGM
İpucu kademesi: Geçişte model → sözel → bağımsız
Malzeme: renk-şekil kartları
Düzenle
Sil
BGM — Dürtü Engelleme (Işık Yakala + 3 Adım) BGM
BGM-II-6
BGM-12 · BGM
İpucu kademesi: Kart açık → kapalı hatırlatma → bağımsız
Malzeme: yeşil/kırmızı kartlar · strateji kartı
Düzenle
Sil
BGM — Düzenleme Desteği (Nefes Halkası) BGM
BGM-SR-7
BGM-12 · BGM
İpucu kademesi: Birlikte → sözel → çocuk kendi başlatır
Malzeme: nefes halkası kartı
Düzenle
Sil
BGM — Önceliklendirme (Önce Hangisi?) BGM
BGM-SP-8
BGM-12 · BGM
İpucu kademesi: Uzman gerekçeyi modeller → sorar → çocuk kendisi
Malzeme: 3 görev kartı · kum saati
Düzenle
Sil
BGM — Sosyal İpucu (Sıra Çubuğu) BGM
BGM-SR-9
BGM-12 · BGM
İpucu kademesi: Çubuk görünür → sözel → bağımsız
Malzeme: sıra çubuğu · zil
Düzenle
Sil
BGM — Çift Kanal (Çift Görev) BGM
BGM-DS-10
BGM-12 · BGM
İpucu kademesi: Tek kanal → çift kanal → normal
Malzeme: izlek kartı · sayı listesi
Düzenle
Sil
BGM — Yüksek Yük (Karışık Tur) BGM
BGM-CM-11
BGM-12 · BGM
İpucu kademesi: Uzman yükü kademeli açar
Malzeme: önceki tur kartları
Düzenle
Sil
BGM — Kendini Yönetme (Kendi Planım) BGM
BGM-TM-12
BGM-12 · BGM
İpucu kademesi: İstek üzerine → yok
Malzeme: 3 kutulu plan kartı · çocuğun kendi işi
Düzenle
Sil
Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.
~~~~

### SUP-SED-DOM-uzman-nav-cizelge

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz
Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil
DEP saat-izleri — girdilerden türetilmiş (K-571/A1)
YASA-2 deseni: elle çizilmez
Dosya	Tamamlanan oturum	Toplam süre	DEP girdisi
ÖĞR-4417	1	40 dk	3
ÖĞR-2903	0	0 dk	0

Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).

İzleme çizelgesi
girdilerden türetildi
Tümü
DEP-2026
BGM-12 (0)
+
2
Evet

Toplam girdi: 3 · Hedefe ulaşılan: 2

Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.

Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.

Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.
~~~~

### SUP-SED-DOM-uzman-nav-rapor

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-SED-DOM-uzman-nav-hizalama

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
MEB destek eğitim programı modülleriyle hizalı çıktı
M1 · Öğrenmeye Destek (150 sa)
M2 · Dil ve İletişim (150 sa)
M3 · Okuma ve Yazma (300 sa)
M4 · Erken Matematik (200 sa)
M5 · Matematik (200 sa)
M6 · Sosyal Etkileşim (100 sa)

Seçili: Okuma ve Yazma — 6 bölüm · önerilen 300 ders saati

Toplam program: 1100 ders saati · 6 modül · giriş yalnız ELLE yapılır.

Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.

Resmî tavan (ÖEK Yön. md.24/4): aylık 12 bireysel · 4 grup · haftalık 4/2 · günlük toplam 3 saat.

Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
~~~~

### SUP-SED-DOM-uzman-nav-bgm

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Bilişsel Geliştirme Modülleri (BGM-12)
12 modül · menü
İki katman. BGM-12, DEP-2026'nın yerine geçmez. DEP = BEP/RAM saat hizası; BGM = yürütücü işlev menüsü. Uzman ikisinden de seçer.
Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. Persona sarmalı dayatılmaz.
TASLAK. BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez. Tam kartlar: SEDUVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md.
ÖĞR-4417
ÖĞR-2903

Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): FS-1 → II-6 → CA-4

Grup I — bilişsel kararlılık (sıra değil)
FS-1 · Odak Kararlılığı
Görevi sürdürme · Sürdürülebilir dikkat
çekirdek
Programdan çıkar
Kart
Tanım: Kısa süreli bir görevi, çeldirici varken bile bırakmadan sürdürme alıştırması.
Amaç: Seans içinde kesintisiz çalışma süresini gözlemek; uzman hedefi BEP satırına taşır.
Ölçüm: Kesintisiz odak süresi (dk) · isabet / yanlış basış (CPT deseni). Yüzdelik ve tanı YOK.
Etkinlik: Kısa görsel tarama turu: hedef şekil belirdiğinde dokun, diğerlerinde bekle. (5–7 dk)
Malzeme: tarama kart seti · kum saati · İpucu: model → sözel ("hedefi bekle") → bağımsız · Girdi: 0-3
Ödev: Evde 5 dk tek görev (kitap/çalışma yaprağı). Puanlanmaz.
Önlem: Masada yalnız o anki materyal; ekran ve televizyon görüş alanında olmasın.
Öneri: Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.
DEP köprüsü: M1 — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)
Dayanak: CPT görev ailesi · PMC 5-küme ⑤ çevre kontrolü (literatür atfı; SEDUVA sonucu değil)
TPM-2 · Zaman Algısı
Süre tahmini · Zamanı ayarlama
çekirdek
Programa al
Kart
CC-3 · Parçalama (Chunking)
İşi bölme · Göreve başlama
Programa al
Kart
CA-4 · Bilgi Mimarisi
Çalışma belleği · Çalışma belleği
çekirdek
Programdan çıkar
Kart
Grup II — esneklik ve düzenleme (sıra değil)
CS-5 · Bilişsel Esneklik
Kural değiştirme · Set değiştirme
Programa al
Kart
II-6 · Dürtü Engelleme
Dur–bekle–yap · İnhibitör kontrol
çekirdek
Programdan çıkar
Kart
SR-7 · Düzenleme Desteği
Nefes / mola · Duygu ve uyarılma
çekirdek
Programa al
Kart
SP-8 · Önceliklendirme
Önemli / acil · Planlama
Programa al
Kart
Grup III — uygulama ve otonomi (sıra değil)
SR-9 · Sosyal İpucu
Sıra / dinleme · Sosyal dikkat
Programa al
Kart
DS-10 · Çift Kanal
İki iş birden · Bölünmüş dikkat
Programa al
Kart
CM-11 · Yüksek Yük
Baskıda sakin kalma · Yük altında sürdürme
Programa al
Kart
TM-12 · Kendini Yönetme
Dış iskeleti solma · Üstbiliş / otonomi
Programa al
Kart
SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.
~~~~

### SUP-SED-DOM-uzman-nav-rambep

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
RAM raporu ve kayıt hattı
ÖĞR-4417
ÖĞR-2903
Kayıt hattı: (a) Ücreti Bakanlıkça karşılanan
RAM raporu: ZORUNLU (rapor + ÖEDK planı + BKDS onamı) · Planlama: ÖEDK eğitim planı ekseninde
Rapor no
RAM-2025/1184
Rapor tarihi
2025-10-14
Geçerlilik
2026-10-14
EDİF durumu
İlk İnceleme tamamlandı (e-Rehberlik)
Sonraki izleme
2026-09-30
Portfolyo
Hazır
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
Resmî form ailesi — hangi girdi neyi besler
DEP-2026 EK-1…EK-7
Ek	Form	Doldurma anı	Supporta katkısı
EK-1	Ölçüt Bağımlı Test (ÖBT)	ilk / ara / son değ.	Tekrar ve deneme sayısı → Ölçüt alanı
EK-2	Kontrol Listesi	ilk / ara / son değ.	Evet/Hayır girdileri → Açıklamalar sütunu
EK-3	Dereceli Puanlama Anahtarı	değerlendirme	0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)
EK-4	Performans Kayıt Formu	her modülün başı ve sonu	x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)
EK-5	BEP Gelişimi İzleme Özet Formu	süreç + yıl sonu	Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler
EK-6	Portfolyo Kontrol Listesi	modül sonu / yıl sonu	Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)
EK-7	Portfolyo Dereceli Puanlama Anahtarı	portfolyo değ.	—
Sınır: Supporta bu formları DOLDURMAZ. x/+ işaretini, performans düzeyini ve “ulaşılamama nedenini” uzman belirler; portfolyo RAM onayına gider. Model: Supporta kanıt üretir · uzman karar verir · RAM onaylar.
Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
~~~~

### SUP-SED-DOM-uzman-nav-evodev

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Ev çalışmaları ve seans dışı görevler
kim · ne · ne zaman
Mutfakta hece avı (5 nesne)
ÖĞR-4417 · Veli · Hafta içi 3 gün · 10 dk
Not: Çocuk istekliydi; 4 nesne bağımsız heceledi.
verildi
yapıldı
yapılmadı
Gazete başlığı okuma
ÖĞR-4417 · Veli · Hafta sonu · 1 kez
verildi
yapıldı
yapılmadı
Sayı kartlarıyla eşleme
ÖĞR-2903 · Veli · Hafta içi 2 gün
Not: Aile yoğunluk bildirdi; süre kısaltıldı.
verildi
yapıldı
yapılmadı
Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz.
Seans başı izleme ritüeli
Ev çalışması gözden geçirilir (yapıldı/yapılmadı — yargı değil gözlem).
Bir önceki oturumun hedef davranışı hatırlatılır.
Bugünün etkinliği ve ipucu kademesi belirlenir.
Oturum sonunda veli için tek satırlık jargonsuz not yazılır.
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-SED-DOM-uzman-nav-aile

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-SED-DOM-uzman-nav-ayarlar

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Şerh kütüphanesi ve roller
OTURUM
Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
CİZELGE
Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.
RAPOR
TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).
AİLE
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
HİZALİ
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
K02
SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).

Kapsam dışı (bilinçli sınırlar)
Devam/yoklama takibi — BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.
Ödeme · fatura · idari-mali işleyiş — K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.
Resmî form üretimi — K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.
Yerel veri

Girdiler, oturum durumları ve rapor onayları yalnız bu cihazda saklanır (KVKK yerel-önce). Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: 7

Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
~~~~

### SUP-SED-DOM-uzman-rapor-yz-oneri

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-SED-DOM-uzman-rapor-reddet

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-SED-DOM-uzman-rapor-onayli

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=True, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-SED-DOM-uzman-aile-A

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-SED-DOM-uzman-aile-sekme-A

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-SED-DOM-uzman-aile-sekme-B

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Analize Göre Aile Görevi (Uzman Seçer)
İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu
Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02).
Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme)
Tetik: Çizelgede kopma > eşik
Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev
Tetik: Ev Çalışmaları “yapılmadı” >2
Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme
Tetik: Girdi “0/3” yoğun
[UZMAN DOLDURUR — K-02]
Gözlem/Rapor bulgusu (tarihli, sayılabilir): ...
Aileye önerilen tek görev (1 cümle, bağlamlı): ...
İpucu kademesi (model/sözel/bağımsız): ...
Kayıt biçimi (tik/süre): ...
Sonraki izleme tarihi: ...

Aileye görev örneği: Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.
Ölçüm: Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.
Şablonu Yazdır

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-SED-DOM-yonetici-rol-secimi

~~~~text
S
SEDUVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)

Özel eğitim merkezi uzman kokpiti · v0.8.8

Devam etmek için rolünüzü seçin.

Yönetici
Tüm dosyalar · rapor onayı · dışa aktarma
Uzman / Eğitimci
Kendi dosyaları · oturum · girdi · rapor taslağı

Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
~~~~

### SUP-SED-DOM-yonetici-nav-pano

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif

Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.

T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)
2026-09-10 10:00 — ÖĞR-4417 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
2026-09-03 10:00 — ÖĞR-2903 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
Onay Bekleyen Raporlar (Human-Accountable AI)
4
• Seans Özeti — 03.09.2026
• Dönem Sonu Değerlendirme — 2026 Güz
• BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
• RAM İzleme Paketi Hazırlığı

YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).
~~~~

### SUP-SED-DOM-yonetici-nav-dosyalar

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Dosya listesi
ÖĞR-4417
ÖĞR-2903
Dosya kartı — ÖĞR-4417
Ad (maskeli)
Öğrenci A. (2. Sınıf)
Doğum
2018-04-12
Okul / Sınıf
Atatürk İlkokulu / 2-B
Devamsızlık
Son ayda 2 gün
Veli
Veli A. · 05xx xxx 41 17
Rıza kaydı
2026-08-20
Geçmiş BEP
RAM eğitsel değerlendirme mevcut (2025)
Program kartı
Seans sayısı
24
Sıklık
Haftada 1 (40 dk)
Aile bileşeni
Var
RAM rapor ref.
RAM-2025/1184
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-SED-DOM-yonetici-nav-takvim

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Oturum takvimi
2026-09-03 haftası
Çakışma: 2026-09-03 10:00 UZM-1 (KC12)
Tarih	Saat	Dosya	Uzman	Durum
2026-09-03	10:00	ÖĞR-4417	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

2026-09-03	10:00	ÖĞR-2903	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

Durumlar: planlandı · tamamlandı · iptal · gelmedi · değişiklikler bu cihazda saklanır.

Veli görüşme-randevu defteri (K-571/A2)
hatırlatma gönderilmez — K-334
Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
Tarih
Konu
Deftere ekle

Defter boş — ilk görüşme kaydını ekleyin.

Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).
~~~~

### SUP-SED-DOM-yonetici-nav-oturum

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Oturum kartı — OT-101

Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı

Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)

Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
ⓘ
Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)
Bu oturumda seçili BGM modülleri
ÖĞR-4417 · sıra uzmanın
FS-1 · Odak Kararlılığı BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M1
CA-4 · Bilgi Mimarisi BGM
5 dk · girdi: 0-3 · DEP köprüsü M1
II-6 · Dürtü Engelleme BGM
6 dk · girdi: Evet / Hayır · DEP köprüsü M6

BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez.

Hızlı girdi paneli
YASA-1 etkin
Etkinlik *zorunlu
— etkinlik seçin —
Hece ayırma çalışması (3.1.2)
Sesli okuma — tekrarlı (3.3.1)
Görsel dikkat eşleme (1.1.3)
İşitsel bellek dizisi (1.2.1)
Sözcük dağarcığı — nesne adlandırma (2.2.1)
Nesne niteliği ayırt etme (4.1.2)
Ritmik sayma (100 içinde) (5.1.4)
Sıra alma ve bekleme (6.2.3)
Sürdürülebilir dikkat — nesne takibi (1.3.2)
Yönerge izleme (2 adımlı) (1.4.1)
Dinlediğini anlama — kısa öykü (2.1.3)
Sözel ifade — cümle kurma (2.3.2)
Karşılıklı konuşma sürdürme (2.4.1)
Harf-ses eşleme (3.2.1)
Yazma — harf dikte (3.4.2)
Gruplama / sınıflama (4.2.3)
Birebir eşleştirme (4.3.1)
Sıralama (büyük-küçük) (4.4.2)
Sayı doğrusu ile toplama (5.2.2)
Çıkarma (nesne ile) (5.2.4)
Günlük yaşam problemi kurma (5.3.1)
Duygu tanıma (6.1.2)
İş birliği oyunu (6.3.1)
Kurala uyma (oyun) (6.3.3)
BGM — Odak Kararlılığı (Hedefi Yakala) (BGM-FS-1)
BGM — Zaman Algısı (Kum Saati Tahmini) (BGM-TPM-2)
BGM — Parçalama (Üç Kart) (BGM-CC-3)
BGM — Bilgi Mimarisi (Sayı Dedektifi) (BGM-CA-4)
BGM — Bilişsel Esneklik (Renk mi Şekil mi?) (BGM-CS-5)
BGM — Dürtü Engelleme (Işık Yakala + 3 Adım) (BGM-II-6)
BGM — Düzenleme Desteği (Nefes Halkası) (BGM-SR-7)
BGM — Önceliklendirme (Önce Hangisi?) (BGM-SP-8)
BGM — Sosyal İpucu (Sıra Çubuğu) (BGM-SR-9)
BGM — Çift Kanal (Çift Görev) (BGM-DS-10)
BGM — Yüksek Yük (Karışık Tur) (BGM-CM-11)
BGM — Kendini Yönetme (Kendi Planım) (BGM-TM-12)
[BGM] FS-1 · Odak Kararlılığı
[BGM] CA-4 · Bilgi Mimarisi
[BGM] II-6 · Dürtü Engelleme
Kodlama
x / +
0-3
Evet / Hayır
Değer
Gözlenen ipucu-kademesi (K-571/A4)
— seçilmeyebilir —
Model
Sözel
Bağımsız
Girdi kaydet

Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.

• Hece ayırma çalışması → + (x / +)
• Sesli okuma — tekrarlı → 2 (0-3)
• Görsel dikkat eşleme → Evet (Evet / Hayır)
~~~~

### SUP-SED-DOM-yonetici-nav-katalog

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Etkinlik ve hedef davranış kataloğu
36 / 36 etkinlik · DEP 24 · BGM 12
Tümü (36)
DEP-2026 (24)
BGM-12 (12)
Tümü
Öğrenmeye Destek
Dil ve İletişim
Okuma ve Yazma
Erken Matematik
Matematik
Sosyal Etkileşim
Yeni etkinlik ekle · kayıt bu cihazda saklanır
DEP-2026
BGM-12
M1 · Öğrenmeye Destek
M2 · Dil ve İletişim
M3 · Okuma ve Yazma
M4 · Erken Matematik
M5 · Matematik
M6 · Sosyal Etkileşim
Ekle
Varsayılana sıfırla
Hece ayırma çalışması
3.1.2
Okuma ve Yazma · DEP
İpucu kademesi: Sözel ipucu → model → bağımsız
Malzeme: hece kartları · çalışma yaprağı
Düzenle
Sil
Sesli okuma — tekrarlı
3.3.1
Okuma ve Yazma · DEP
İpucu kademesi: Eşli okuma → bağımsız
Malzeme: kısa metin · kronometre
Düzenle
Sil
Görsel dikkat eşleme
1.1.3
Öğrenmeye Destek · DEP
İpucu kademesi: İşaret → sözel → bağımsız
Malzeme: eşleme kartları
Düzenle
Sil
İşitsel bellek dizisi
1.2.1
Öğrenmeye Destek · DEP
İpucu kademesi: Model → gecikmeli model → bağımsız
Malzeme: ses kartları
Düzenle
Sil
Sözcük dağarcığı — nesne adlandırma
2.2.1
Dil ve İletişim · DEP
İpucu kademesi: Fiziksel ipucu → sözel → bağımsız
Malzeme: nesne resimleri
Düzenle
Sil
Nesne niteliği ayırt etme
4.1.2
Erken Matematik · DEP
İpucu kademesi: Model → kısmi ipucu → bağımsız
Malzeme: blok seti
Düzenle
Sil
Ritmik sayma (100 içinde)
5.1.4
Matematik · DEP
İpucu kademesi: Birlikte sayma → bağımsız
Malzeme: sayı doğrusu
Düzenle
Sil
Sıra alma ve bekleme
6.2.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → sözel hatırlatma → bağımsız
Malzeme: sıra kartı · kum saati
Düzenle
Sil
Sürdürülebilir dikkat — nesne takibi
1.3.2
Öğrenmeye Destek · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: renkli toplar · tepsi
Düzenle
Sil
Yönerge izleme (2 adımlı)
1.4.1
Öğrenmeye Destek · DEP
İpucu kademesi: Fiziksel rehber → sözel → bağımsız
Malzeme: yönerge kartları
Düzenle
Sil
Dinlediğini anlama — kısa öykü
2.1.3
Dil ve İletişim · DEP
İpucu kademesi: Sözel ipucu → soru-cevap → bağımsız
Malzeme: öykü kartı · soru listesi
Düzenle
Sil
Sözel ifade — cümle kurma
2.3.2
Dil ve İletişim · DEP
İpucu kademesi: Model cümle → tamamlama → bağımsız
Malzeme: kelime kartları
Düzenle
Sil
Karşılıklı konuşma sürdürme
2.4.1
Dil ve İletişim · DEP
İpucu kademesi: Sözel başlatma → sıra alma → bağımsız
Malzeme: konu kartları · kum saati
Düzenle
Sil
Harf-ses eşleme
3.2.1
Okuma ve Yazma · DEP
İpucu kademesi: Model → eşleme → bağımsız
Malzeme: harf kartları · ses kutusu
Düzenle
Sil
Yazma — harf dikte
3.4.2
Okuma ve Yazma · DEP
İpucu kademesi: Noktalı iz → kopya → bağımsız
Malzeme: dikte yaprağı · kalem
Düzenle
Sil
Gruplama / sınıflama
4.2.3
Erken Matematik · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: sınıflama kutuları · nesneler
Düzenle
Sil
Birebir eşleştirme
4.3.1
Erken Matematik · DEP
İpucu kademesi: Fiziksel rehber → bağımsız
Malzeme: eş kartları
Düzenle
Sil
Sıralama (büyük-küçük)
4.4.2
Erken Matematik · DEP
İpucu kademesi: Model → deneme-yanılma → bağımsız
Malzeme: sıralama şeridi
Düzenle
Sil
Sayı doğrusu ile toplama
5.2.2
Matematik · DEP
İpucu kademesi: Model → rehberli → bağımsız
Malzeme: sayı doğrusu · pul
Düzenle
Sil
Çıkarma (nesne ile)
5.2.4
Matematik · DEP
İpucu kademesi: Nesne desteği → zihinden
Malzeme: sayma pulları
Düzenle
Sil
Günlük yaşam problemi kurma
5.3.1
Matematik · DEP
İpucu kademesi: Sözel senaryo → model → bağımsız
Malzeme: problem kartları
Düzenle
Sil
Duygu tanıma
6.1.2
Sosyal Etkileşim · DEP
İpucu kademesi: Görsel ipucu → eşleme → bağımsız
Malzeme: duygu kartları
Düzenle
Sil
İş birliği oyunu
6.3.1
Sosyal Etkileşim · DEP
İpucu kademesi: Eşli oyun → sıra alma → bağımsız
Malzeme: kutu oyunu
Düzenle
Sil
Kurala uyma (oyun)
6.3.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → hatırlatma → bağımsız
Malzeme: kural kartı
Düzenle
Sil
BGM — Odak Kararlılığı (Hedefi Yakala) BGM
BGM-FS-1
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: tarama kart seti · kum saati
Düzenle
Sil
BGM — Zaman Algısı (Kum Saati Tahmini) BGM
BGM-TPM-2
BGM-12 · BGM
İpucu kademesi: Görsel sayaç açık → yarı kapalı → kapalı
Malzeme: kum saati · tahmin kartı
Düzenle
Sil
BGM — Parçalama (Üç Kart) BGM
BGM-CC-3
BGM-12 · BGM
İpucu kademesi: Model (uzman böler) → sözel → bağımsız
Malzeme: çalışma yaprağı · 3 boş kart · kalem
Düzenle
Sil
BGM — Bilgi Mimarisi (Sayı Dedektifi) BGM
BGM-CA-4
BGM-12 · BGM
İpucu kademesi: Görsel destek açık → kademeli kalkar
Malzeme: sayı/nesne kartları · küçük tahta
Düzenle
Sil
BGM — Bilişsel Esneklik (Renk mi Şekil mi?) BGM
BGM-CS-5
BGM-12 · BGM
İpucu kademesi: Geçişte model → sözel → bağımsız
Malzeme: renk-şekil kartları
Düzenle
Sil
BGM — Dürtü Engelleme (Işık Yakala + 3 Adım) BGM
BGM-II-6
BGM-12 · BGM
İpucu kademesi: Kart açık → kapalı hatırlatma → bağımsız
Malzeme: yeşil/kırmızı kartlar · strateji kartı
Düzenle
Sil
BGM — Düzenleme Desteği (Nefes Halkası) BGM
BGM-SR-7
BGM-12 · BGM
İpucu kademesi: Birlikte → sözel → çocuk kendi başlatır
Malzeme: nefes halkası kartı
Düzenle
Sil
BGM — Önceliklendirme (Önce Hangisi?) BGM
BGM-SP-8
BGM-12 · BGM
İpucu kademesi: Uzman gerekçeyi modeller → sorar → çocuk kendisi
Malzeme: 3 görev kartı · kum saati
Düzenle
Sil
BGM — Sosyal İpucu (Sıra Çubuğu) BGM
BGM-SR-9
BGM-12 · BGM
İpucu kademesi: Çubuk görünür → sözel → bağımsız
Malzeme: sıra çubuğu · zil
Düzenle
Sil
BGM — Çift Kanal (Çift Görev) BGM
BGM-DS-10
BGM-12 · BGM
İpucu kademesi: Tek kanal → çift kanal → normal
Malzeme: izlek kartı · sayı listesi
Düzenle
Sil
BGM — Yüksek Yük (Karışık Tur) BGM
BGM-CM-11
BGM-12 · BGM
İpucu kademesi: Uzman yükü kademeli açar
Malzeme: önceki tur kartları
Düzenle
Sil
BGM — Kendini Yönetme (Kendi Planım) BGM
BGM-TM-12
BGM-12 · BGM
İpucu kademesi: İstek üzerine → yok
Malzeme: 3 kutulu plan kartı · çocuğun kendi işi
Düzenle
Sil
Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.
~~~~

### SUP-SED-DOM-yonetici-nav-cizelge

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz
Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil
DEP saat-izleri — girdilerden türetilmiş (K-571/A1)
YASA-2 deseni: elle çizilmez
Dosya	Tamamlanan oturum	Toplam süre	DEP girdisi
ÖĞR-4417	1	40 dk	3
ÖĞR-2903	0	0 dk	0

Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).

İzleme çizelgesi
girdilerden türetildi
Tümü
DEP-2026
BGM-12 (0)
+
2
Evet

Toplam girdi: 3 · Hedefe ulaşılan: 2

Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.

Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.

Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.
~~~~

### SUP-SED-DOM-yonetici-nav-rapor

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-SED-DOM-yonetici-nav-hizalama

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
MEB destek eğitim programı modülleriyle hizalı çıktı
M1 · Öğrenmeye Destek (150 sa)
M2 · Dil ve İletişim (150 sa)
M3 · Okuma ve Yazma (300 sa)
M4 · Erken Matematik (200 sa)
M5 · Matematik (200 sa)
M6 · Sosyal Etkileşim (100 sa)

Seçili: Okuma ve Yazma — 6 bölüm · önerilen 300 ders saati

Toplam program: 1100 ders saati · 6 modül · giriş yalnız ELLE yapılır.

Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.

Resmî tavan (ÖEK Yön. md.24/4): aylık 12 bireysel · 4 grup · haftalık 4/2 · günlük toplam 3 saat.

Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
~~~~

### SUP-SED-DOM-yonetici-nav-bgm

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Bilişsel Geliştirme Modülleri (BGM-12)
12 modül · menü
İki katman. BGM-12, DEP-2026'nın yerine geçmez. DEP = BEP/RAM saat hizası; BGM = yürütücü işlev menüsü. Uzman ikisinden de seçer.
Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. Persona sarmalı dayatılmaz.
TASLAK. BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez. Tam kartlar: SEDUVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md.
ÖĞR-4417
ÖĞR-2903

Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): FS-1 → II-6 → CA-4

Grup I — bilişsel kararlılık (sıra değil)
FS-1 · Odak Kararlılığı
Görevi sürdürme · Sürdürülebilir dikkat
çekirdek
Programdan çıkar
Kart
Tanım: Kısa süreli bir görevi, çeldirici varken bile bırakmadan sürdürme alıştırması.
Amaç: Seans içinde kesintisiz çalışma süresini gözlemek; uzman hedefi BEP satırına taşır.
Ölçüm: Kesintisiz odak süresi (dk) · isabet / yanlış basış (CPT deseni). Yüzdelik ve tanı YOK.
Etkinlik: Kısa görsel tarama turu: hedef şekil belirdiğinde dokun, diğerlerinde bekle. (5–7 dk)
Malzeme: tarama kart seti · kum saati · İpucu: model → sözel ("hedefi bekle") → bağımsız · Girdi: 0-3
Ödev: Evde 5 dk tek görev (kitap/çalışma yaprağı). Puanlanmaz.
Önlem: Masada yalnız o anki materyal; ekran ve televizyon görüş alanında olmasın.
Öneri: Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.
DEP köprüsü: M1 — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)
Dayanak: CPT görev ailesi · PMC 5-küme ⑤ çevre kontrolü (literatür atfı; SEDUVA sonucu değil)
TPM-2 · Zaman Algısı
Süre tahmini · Zamanı ayarlama
çekirdek
Programa al
Kart
CC-3 · Parçalama (Chunking)
İşi bölme · Göreve başlama
Programa al
Kart
CA-4 · Bilgi Mimarisi
Çalışma belleği · Çalışma belleği
çekirdek
Programdan çıkar
Kart
Grup II — esneklik ve düzenleme (sıra değil)
CS-5 · Bilişsel Esneklik
Kural değiştirme · Set değiştirme
Programa al
Kart
II-6 · Dürtü Engelleme
Dur–bekle–yap · İnhibitör kontrol
çekirdek
Programdan çıkar
Kart
SR-7 · Düzenleme Desteği
Nefes / mola · Duygu ve uyarılma
çekirdek
Programa al
Kart
SP-8 · Önceliklendirme
Önemli / acil · Planlama
Programa al
Kart
Grup III — uygulama ve otonomi (sıra değil)
SR-9 · Sosyal İpucu
Sıra / dinleme · Sosyal dikkat
Programa al
Kart
DS-10 · Çift Kanal
İki iş birden · Bölünmüş dikkat
Programa al
Kart
CM-11 · Yüksek Yük
Baskıda sakin kalma · Yük altında sürdürme
Programa al
Kart
TM-12 · Kendini Yönetme
Dış iskeleti solma · Üstbiliş / otonomi
Programa al
Kart
SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.
~~~~

### SUP-SED-DOM-yonetici-nav-rambep

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
RAM raporu ve kayıt hattı
ÖĞR-4417
ÖĞR-2903
Kayıt hattı: (a) Ücreti Bakanlıkça karşılanan
RAM raporu: ZORUNLU (rapor + ÖEDK planı + BKDS onamı) · Planlama: ÖEDK eğitim planı ekseninde
Rapor no
RAM-2025/1184
Rapor tarihi
2025-10-14
Geçerlilik
2026-10-14
EDİF durumu
İlk İnceleme tamamlandı (e-Rehberlik)
Sonraki izleme
2026-09-30
Portfolyo
Hazır
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
Resmî form ailesi — hangi girdi neyi besler
DEP-2026 EK-1…EK-7
Ek	Form	Doldurma anı	Supporta katkısı
EK-1	Ölçüt Bağımlı Test (ÖBT)	ilk / ara / son değ.	Tekrar ve deneme sayısı → Ölçüt alanı
EK-2	Kontrol Listesi	ilk / ara / son değ.	Evet/Hayır girdileri → Açıklamalar sütunu
EK-3	Dereceli Puanlama Anahtarı	değerlendirme	0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)
EK-4	Performans Kayıt Formu	her modülün başı ve sonu	x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)
EK-5	BEP Gelişimi İzleme Özet Formu	süreç + yıl sonu	Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler
EK-6	Portfolyo Kontrol Listesi	modül sonu / yıl sonu	Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)
EK-7	Portfolyo Dereceli Puanlama Anahtarı	portfolyo değ.	—
Sınır: Supporta bu formları DOLDURMAZ. x/+ işaretini, performans düzeyini ve “ulaşılamama nedenini” uzman belirler; portfolyo RAM onayına gider. Model: Supporta kanıt üretir · uzman karar verir · RAM onaylar.
Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
~~~~

### SUP-SED-DOM-yonetici-nav-evodev

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Ev çalışmaları ve seans dışı görevler
kim · ne · ne zaman
Mutfakta hece avı (5 nesne)
ÖĞR-4417 · Veli · Hafta içi 3 gün · 10 dk
Not: Çocuk istekliydi; 4 nesne bağımsız heceledi.
verildi
yapıldı
yapılmadı
Gazete başlığı okuma
ÖĞR-4417 · Veli · Hafta sonu · 1 kez
verildi
yapıldı
yapılmadı
Sayı kartlarıyla eşleme
ÖĞR-2903 · Veli · Hafta içi 2 gün
Not: Aile yoğunluk bildirdi; süre kısaltıldı.
verildi
yapıldı
yapılmadı
Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz.
Seans başı izleme ritüeli
Ev çalışması gözden geçirilir (yapıldı/yapılmadı — yargı değil gözlem).
Bir önceki oturumun hedef davranışı hatırlatılır.
Bugünün etkinliği ve ipucu kademesi belirlenir.
Oturum sonunda veli için tek satırlık jargonsuz not yazılır.
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-SED-DOM-yonetici-nav-aile

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-SED-DOM-yonetici-nav-ayarlar

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Şerh kütüphanesi ve roller
OTURUM
Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
CİZELGE
Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.
RAPOR
TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).
AİLE
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
HİZALİ
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
K02
SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).

Kapsam dışı (bilinçli sınırlar)
Devam/yoklama takibi — BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.
Ödeme · fatura · idari-mali işleyiş — K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.
Resmî form üretimi — K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.
Yerel veri

Girdiler, oturum durumları ve rapor onayları yalnız bu cihazda saklanır (KVKK yerel-önce). Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: 7

Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
~~~~

### SUP-SED-DOM-yonetici-rapor-onayli

~~~~text
S
SEDUVA Supporta™
Uzman Kokpiti · v0.8.8
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

SEDUVA Supporta: SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.

v0.8.8 · TAM — MEB dersleri aktif
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=True, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

## Yazdırma ve CSV çıktıları

Gerçek yazıcı kullanılmadı; metinler mevcut sentetik kayıtlarla üretildi.

### rapor / rol=uzman

~~~~text
Seans özeti — Seans Özeti — 03.09.2026
ONAYLI — Yönetici 2026-09-03
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v0.8.8
~~~~

### aile-A / rol=uzman

~~~~text
Nasihat ve Kıyas Yok — Gözlem Dili — ÖĞR-4417
ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.

“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
- “Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
- Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).

Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v0.8.8 · Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### aile-B / rol=uzman

~~~~text
Analize Göre Aile Görevi (Uzman Seçer) — ÖĞR-4417
ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER
[UZMAN DOLDURUR — K-02]
Gözlem/Rapor bulgusu (tarihli, sayılabilir): ...
Aileye önerilen tek görev (1 cümle, bağlamlı): ...
İpucu kademesi (model/sözel/bağımsız): ...
Kayıt biçimi (tik/süre): ...
Sonraki izleme tarihi: ...


Görev: Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.
Ölçüm: Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v0.8.8 · Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### CSV: R-1-seans.csv

~~~~csv
tur,baslik,durum,icerik
seans,"Seans Özeti — 03.09.2026",ONAYLI,"Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır."
~~~~

## AST kaynak adayları

ID kaynak anının satırına bağlıdır; JSX/template parçaları tek başına tam cümle değildir. Exact bağlam için ham dosya ve DOM birlikte okunur.

| ID | Dosya:satır | Tür | Ham parça (↵=satır sonu) | Görünürlük |
|---|---|---|---|---|
| SUP-SED-0001 | `App.tsx:17` | JsxText | SEDUVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0002 | `App.tsx:18` | JsxText | Özel eğitim merkezi uzman kokpiti · v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0003 | `App.tsx:20` | JsxText | Devam etmek için rolünüzü seçin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0004 | `App.tsx:31` | JsxText | Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0005 | `App.tsx:39` | StringLiteral | PILOT — kısıtlı (takma ad, sunucusuz) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0006 | `App.tsx:39` | StringLiteral | TAM — MEB dersleri aktif | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0007 | `App.tsx:39` | StringLiteral | DEMO — jüri tanıtım | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0008 | `components/Ekranlar.tsx:25` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0009 | `components/Ekranlar.tsx:32` | JsxText | Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0010 | `components/Ekranlar.tsx:33` | JsxText | Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0011 | `components/Ekranlar.tsx:38` | StringLiteral | T1/T2 Transfer Kanıtı İzleme (Günün Oturumları) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0012 | `components/Ekranlar.tsx:42` | JsxText | dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0013 | `components/Ekranlar.tsx:44` | JsxText | T1 Merkezi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0014 | `components/Ekranlar.tsx:45` | JsxText | T2 Okul Bekleniyor | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0015 | `components/Ekranlar.tsx:51` | StringLiteral | Onay Bekleyen Raporlar (Human-Accountable AI) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0016 | `components/Ekranlar.tsx:53` | JsxText | YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0017 | `components/Ekranlar.tsx:67` | StringLiteral | Dosya listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0018 | `components/Ekranlar.tsx:77` | TemplateHead | Dosya kartı — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0019 | `components/Ekranlar.tsx:79` | StringLiteral | Ad (maskeli) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0020 | `components/Ekranlar.tsx:79` | StringLiteral | Doğum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0021 | `components/Ekranlar.tsx:79` | StringLiteral | Okul / Sınıf | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0022 | `components/Ekranlar.tsx:80` | StringLiteral | Devamsızlık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0023 | `components/Ekranlar.tsx:81` | StringLiteral | Rıza kaydı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0024 | `components/Ekranlar.tsx:81` | StringLiteral | Geçmiş BEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0025 | `components/Ekranlar.tsx:86` | StringLiteral | Program kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0026 | `components/Ekranlar.tsx:88` | JsxText | Seans sayısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0027 | `components/Ekranlar.tsx:89` | JsxText | Sıklık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0028 | `components/Ekranlar.tsx:90` | JsxText | Aile bileşeni | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0029 | `components/Ekranlar.tsx:91` | JsxText | RAM rapor ref. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0030 | `components/Ekranlar.tsx:125` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0031 | `components/Ekranlar.tsx:125` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0032 | `components/Ekranlar.tsx:133` | StringLiteral | Oturum takvimi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0033 | `components/Ekranlar.tsx:137` | JsxText | haftası | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0034 | `components/Ekranlar.tsx:143` | JsxText | Çakışma: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0035 | `components/Ekranlar.tsx:143` | JsxText | (KC12) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0036 | `components/Ekranlar.tsx:148` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0037 | `components/Ekranlar.tsx:148` | JsxText | Saat | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0038 | `components/Ekranlar.tsx:148` | JsxText | Dosya | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0039 | `components/Ekranlar.tsx:148` | JsxText | Uzman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0040 | `components/Ekranlar.tsx:148` | JsxText | Durum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0041 | `components/Ekranlar.tsx:165` | JsxText | Bu haftada oturum yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0042 | `components/Ekranlar.tsx:168` | JsxText | Durumlar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0043 | `components/Ekranlar.tsx:168` | JsxText | · değişiklikler bu cihazda saklanır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0044 | `components/Ekranlar.tsx:170` | StringLiteral | Veli görüşme-randevu defteri (K-571/A2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0045 | `components/Ekranlar.tsx:170` | JsxText | hatırlatma gönderilmez — K-334 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0046 | `components/Ekranlar.tsx:172` | JsxText | Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0047 | `components/Ekranlar.tsx:175` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0048 | `components/Ekranlar.tsx:177` | JsxText | Konu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0049 | `components/Ekranlar.tsx:178` | StringLiteral | örn. B yarı-dönem değerlendirme paylaşımı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0050 | `components/Ekranlar.tsx:180` | JsxText | Deftere ekle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0051 | `components/Ekranlar.tsx:183` | JsxText | Defter boş — ilk görüşme kaydını ekleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0052 | `components/Ekranlar.tsx:184` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0053 | `components/Ekranlar.tsx:184` | JsxText | Konu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0054 | `components/Ekranlar.tsx:184` | JsxText | Durum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0055 | `components/Ekranlar.tsx:184` | JsxText | Not | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0056 | `components/Ekranlar.tsx:189` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0057 | `components/Ekranlar.tsx:189` | StringLiteral | gerçekleşti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0058 | `components/Ekranlar.tsx:190` | StringLiteral | kısa not (yapılandırılmamış) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0059 | `components/Ekranlar.tsx:192` | JsxText | Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0060 | `components/Ekranlar.tsx:206` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0061 | `components/Ekranlar.tsx:206` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0062 | `components/Ekranlar.tsx:214` | StringLiteral | Oturum kartı — OT-101 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0063 | `components/Ekranlar.tsx:215` | JsxText | Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0064 | `components/Ekranlar.tsx:217` | JsxText | Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0065 | `components/Ekranlar.tsx:222` | JsxText | Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0066 | `components/Ekranlar.tsx:225` | StringLiteral | Bu oturumda seçili BGM modülleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0067 | `components/Ekranlar.tsx:225` | JsxText | · sıra uzmanın | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0068 | `components/Ekranlar.tsx:227` | JsxText | Bu dosya için BGM seçilmedi (Bilişsel Geliştirme ekranından alınır). DEP etkinlikleri yine kullanılabilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0069 | `components/Ekranlar.tsx:232` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0070 | `components/Ekranlar.tsx:233` | JsxText | · girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0071 | `components/Ekranlar.tsx:233` | TemplateHead | · DEP köprüsü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0072 | `components/Ekranlar.tsx:239` | JsxText | Etkinlik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0073 | `components/Ekranlar.tsx:240` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0074 | `components/Ekranlar.tsx:240` | JsxText | İpucu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0075 | `components/Ekranlar.tsx:241` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0076 | `components/Ekranlar.tsx:246` | StringLiteral | Hızlı girdi paneli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0077 | `components/Ekranlar.tsx:246` | JsxText | YASA-1 etkin | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0078 | `components/Ekranlar.tsx:249` | JsxText | Etkinlik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0079 | `components/Ekranlar.tsx:249` | JsxText | *zorunlu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0080 | `components/Ekranlar.tsx:252` | JsxText | — etkinlik seçin — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0081 | `components/Ekranlar.tsx:253` | StringLiteral | DEP-2026 etkinlikleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0082 | `components/Ekranlar.tsx:257` | StringLiteral | BGM-12 (bu dosya için seçili) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0083 | `components/Ekranlar.tsx:258` | JsxText | [BGM] | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0084 | `components/Ekranlar.tsx:264` | JsxText | Kodlama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0085 | `components/Ekranlar.tsx:271` | JsxText | Değer | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0086 | `components/Ekranlar.tsx:276` | JsxText | Gözlenen ipucu-kademesi (K-571/A4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0087 | `components/Ekranlar.tsx:279` | JsxText | — seçilmeyebilir — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0088 | `components/Ekranlar.tsx:280` | JsxText | Model | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0089 | `components/Ekranlar.tsx:281` | JsxText | Sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0090 | `components/Ekranlar.tsx:282` | JsxText | Bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0091 | `components/Ekranlar.tsx:287` | JsxText | Planlı ipucu-kademesi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0092 | `components/Ekranlar.tsx:287` | JsxText | · gözlem kaydı uzmanın teyididir (K-02: ölçüm-değil-gözlem). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0093 | `components/Ekranlar.tsx:294` | JsxText | Girdi kaydet | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0094 | `components/Ekranlar.tsx:304` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0095 | `components/Ekranlar.tsx:306` | JsxText | · ipucu(gözlenen): | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0096 | `components/Ekranlar.tsx:306` | StringLiteral | Sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0097 | `components/Ekranlar.tsx:306` | StringLiteral | Bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0098 | `components/Ekranlar.tsx:328` | JsxText | Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0099 | `components/Ekranlar.tsx:329` | JsxText | Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0100 | `components/Ekranlar.tsx:331` | StringLiteral | DEP saat-izleri — girdilerden türetilmiş (K-571/A1) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0101 | `components/Ekranlar.tsx:331` | JsxText | YASA-2 deseni: elle çizilmez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0102 | `components/Ekranlar.tsx:333` | JsxText | Dosya | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0103 | `components/Ekranlar.tsx:333` | JsxText | Tamamlanan oturum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0104 | `components/Ekranlar.tsx:333` | JsxText | Toplam süre | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0105 | `components/Ekranlar.tsx:333` | JsxText | DEP girdisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0106 | `components/Ekranlar.tsx:335` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0107 | `components/Ekranlar.tsx:341` | JsxText | Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0108 | `components/Ekranlar.tsx:344` | StringLiteral | İzleme çizelgesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0109 | `components/Ekranlar.tsx:344` | JsxText | girdilerden türetildi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0110 | `components/Ekranlar.tsx:349` | StringLiteral | Tümü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0111 | `components/Ekranlar.tsx:349` | TemplateHead | BGM-12 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0112 | `components/Ekranlar.tsx:363` | JsxText | Toplam girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0113 | `components/Ekranlar.tsx:363` | JsxText | · Hedefe ulaşılan: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0114 | `components/Ekranlar.tsx:364` | JsxText | Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0115 | `components/Ekranlar.tsx:374` | StringLiteral | Seans özeti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0116 | `components/Ekranlar.tsx:374` | StringLiteral | Aylık özet | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0117 | `components/Ekranlar.tsx:374` | StringLiteral | Dönem sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0118 | `components/Ekranlar.tsx:375` | StringLiteral | BEP ilerleme taslağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0119 | `components/Ekranlar.tsx:375` | StringLiteral | RAM izleme paketi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0120 | `components/Ekranlar.tsx:376` | StringLiteral | Aile bilgilendirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0121 | `components/Ekranlar.tsx:381` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0122 | `components/Ekranlar.tsx:385` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0123 | `components/Ekranlar.tsx:387` | TemplateHead | — YZ EĞİTİMSEL DESTEK ÖNERİSİ — ↵ (Kanıt Kaynağı: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0124 | `components/Ekranlar.tsx:390` | TemplateMiddle | T1 seansı, | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0125 | `components/Ekranlar.tsx:390` | LastTemplateToken | dk aktif izlem) ↵ Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir. ↵  ↵ ⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0126 | `components/Ekranlar.tsx:398` | FirstTemplateToken | — YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ — ↵ Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0127 | `components/Ekranlar.tsx:407` | TemplateHead | <!doctype html><title> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0128 | `components/Ekranlar.tsx:407` | TemplateMiddle | </title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:16px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0129 | `components/Ekranlar.tsx:407` | TemplateMiddle | </h1><div class=muhur>ONAYLI — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0130 | `components/Ekranlar.tsx:407` | TemplateMiddle | </pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;\|&nbsp; Kopya 2/2 — Kurum arşivi · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0131 | `components/Ekranlar.tsx:407` | TemplateMiddle | · Supporta v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0132 | `components/Ekranlar.tsx:409` | TemplateHead | tur,baslik,durum,icerik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0133 | `components/Ekranlar.tsx:419` | JsxText | UZMAN ONAYI BEKLİYOR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0134 | `components/Ekranlar.tsx:419` | JsxText | UZMAN ONAYLI | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0135 | `components/Ekranlar.tsx:432` | JsxText | Human-Accountable AI (YZ Destek Asistanı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0136 | `components/Ekranlar.tsx:436` | JsxText | Kanıtı İncele ve YZ Önerisi Al | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0137 | `components/Ekranlar.tsx:439` | JsxText | Öneriyi Reddet ve Gerekçelendir | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0138 | `components/Ekranlar.tsx:442` | JsxText | YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0139 | `components/Ekranlar.tsx:447` | JsxText | ✓ Değişiklikleri Onayla ve İmzala | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0140 | `components/Ekranlar.tsx:448` | JsxText | Dışa aktar (2 kopya) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0141 | `components/Ekranlar.tsx:449` | JsxText | Onaysız rapor dışa aktarılamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0142 | `components/Ekranlar.tsx:464` | StringLiteral | MEB destek eğitim programı modülleriyle hizalı çıktı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0143 | `components/Ekranlar.tsx:469` | JsxText | sa) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0144 | `components/Ekranlar.tsx:473` | JsxText | Seçili: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0145 | `components/Ekranlar.tsx:473` | JsxText | bölüm · önerilen | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0146 | `components/Ekranlar.tsx:473` | JsxText | ders saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0147 | `components/Ekranlar.tsx:474` | JsxText | Toplam program: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0148 | `components/Ekranlar.tsx:474` | JsxText | ders saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0149 | `components/Ekranlar.tsx:474` | JsxText | · 6 modül · giriş yalnız ELLE yapılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0150 | `components/Ekranlar.tsx:476` | JsxText | Modül seçimi serbesttir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0151 | `components/Ekranlar.tsx:479` | JsxText | Resmî tavan (ÖEK Yön. md.24/4): aylık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0152 | `components/Ekranlar.tsx:479` | JsxText | bireysel · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0153 | `components/Ekranlar.tsx:479` | JsxText | grup · ↵         haftalık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0154 | `components/Ekranlar.tsx:480` | JsxText | · günlük toplam | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0155 | `components/Ekranlar.tsx:480` | JsxText | saat. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0156 | `components/Ekranlar.tsx:492` | StringLiteral | Aile & Öğretmen İşbirliği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0157 | `components/Ekranlar.tsx:493` | JsxText | Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0158 | `components/Ekranlar.tsx:496` | StringLiteral | Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0159 | `components/Ekranlar.tsx:496` | JsxText | K-407 · 5+1 · TASLAK | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0160 | `components/Ekranlar.tsx:505` | StringLiteral | Bilgilendirme çıktısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0161 | `components/Ekranlar.tsx:506` | JsxText | Yalnız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0162 | `components/Ekranlar.tsx:506` | JsxText | onaylı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0163 | `components/Ekranlar.tsx:506` | JsxText | raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0164 | `components/Ekranlar.tsx:508` | JsxText | Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0165 | `components/Ekranlar.tsx:518` | StringLiteral | Şerh kütüphanesi ve roller | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0166 | `components/Ekranlar.tsx:524` | JsxText | Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0167 | `components/Ekranlar.tsx:526` | JsxText | Kapsam dışı (bilinçli sınırlar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0168 | `components/Ekranlar.tsx:536` | JsxText | Yerel veri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0169 | `components/Ekranlar.tsx:538` | JsxText | Girdiler, oturum durumları ve rapor onayları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0170 | `components/Ekranlar.tsx:538` | JsxText | yalnız bu cihazda | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0171 | `components/Ekranlar.tsx:538` | JsxText | saklanır (KVKK yerel-önce). ↵           Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0172 | `components/Ekranlar.tsx:544` | JsxText | Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0173 | `components/Ekranlar.tsx:560` | StringLiteral | RAM raporu ve kayıt hattı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0174 | `components/Ekranlar.tsx:568` | JsxText | Kayıt hattı: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0175 | `components/Ekranlar.tsx:568` | JsxText | RAM raporu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0176 | `components/Ekranlar.tsx:568` | JsxText | · Planlama: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0177 | `components/Ekranlar.tsx:571` | StringLiteral | Rapor no | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0178 | `components/Ekranlar.tsx:571` | StringLiteral | Rapor tarihi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0179 | `components/Ekranlar.tsx:571` | StringLiteral | Geçerlilik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0180 | `components/Ekranlar.tsx:572` | StringLiteral | EDİF durumu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0181 | `components/Ekranlar.tsx:572` | StringLiteral | Sonraki izleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0182 | `components/Ekranlar.tsx:573` | StringLiteral | Hazır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0183 | `components/Ekranlar.tsx:573` | StringLiteral | Hazır değil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0184 | `components/Ekranlar.tsx:579` | StringLiteral | Resmî form ailesi — hangi girdi neyi besler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0185 | `components/Ekranlar.tsx:580` | JsxText | DEP-2026 EK-1…EK-7 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0186 | `components/Ekranlar.tsx:583` | JsxText | Form | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0187 | `components/Ekranlar.tsx:583` | JsxText | Doldurma anı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0188 | `components/Ekranlar.tsx:583` | JsxText | Supporta katkısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0189 | `components/Ekranlar.tsx:596` | JsxText | Sınır: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0190 | `components/Ekranlar.tsx:596` | JsxText | Supporta bu formları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0191 | `components/Ekranlar.tsx:596` | JsxText | DOLDURMAZ | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0192 | `components/Ekranlar.tsx:596` | JsxText | . x/+ işaretini, performans düzeyini ve ↵           “ulaşılamama nedenini” | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0193 | `components/Ekranlar.tsx:597` | JsxText | uzman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0194 | `components/Ekranlar.tsx:597` | JsxText | belirler; portfolyo | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0195 | `components/Ekranlar.tsx:597` | JsxText | RAM onayına | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0196 | `components/Ekranlar.tsx:597` | JsxText | gider. ↵           Model: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0197 | `components/Ekranlar.tsx:598` | JsxText | Supporta kanıt üretir · uzman karar verir · RAM onaylar. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0198 | `components/Ekranlar.tsx:601` | JsxText | Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0199 | `components/Ekranlar.tsx:615` | StringLiteral | Ev çalışmaları ve seans dışı görevler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0200 | `components/Ekranlar.tsx:616` | JsxText | kim · ne · ne zaman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0201 | `components/Ekranlar.tsx:624` | JsxText | Not: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0202 | `components/Ekranlar.tsx:632` | JsxText | verildi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0203 | `components/Ekranlar.tsx:632` | JsxText | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0204 | `components/Ekranlar.tsx:632` | JsxText | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0205 | `components/Ekranlar.tsx:638` | StringLiteral | Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0206 | `components/Ekranlar.tsx:640` | StringLiteral | Seans başı izleme ritüeli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0207 | `components/Ekranlar.tsx:642` | JsxText | Ev çalışması gözden geçirilir (yapıldı/yapılmadı — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0208 | `components/Ekranlar.tsx:642` | JsxText | yargı değil gözlem | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0209 | `components/Ekranlar.tsx:643` | JsxText | Bir önceki oturumun hedef davranışı hatırlatılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0210 | `components/Ekranlar.tsx:644` | JsxText | Bugünün etkinliği ve ipucu kademesi belirlenir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0211 | `components/Ekranlar.tsx:645` | JsxText | Oturum sonunda veli için tek satırlık jargonsuz not yazılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0212 | `components/Ekranlar.tsx:656` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0213 | `components/Ekranlar.tsx:656` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0214 | `components/Ekranlar.tsx:660` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0215 | `components/Ekranlar.tsx:660` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0216 | `components/Ekranlar.tsx:660` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0217 | `components/Ekranlar.tsx:661` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0218 | `components/Ekranlar.tsx:663` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0219 | `components/Ekranlar.tsx:666` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0220 | `components/Ekranlar.tsx:666` | StringLiteral | Model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0221 | `components/Ekranlar.tsx:669` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0222 | `components/Ekranlar.tsx:671` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0223 | `components/Ekranlar.tsx:671` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0224 | `components/Ekranlar.tsx:671` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0225 | `components/Ekranlar.tsx:675` | StringLiteral | Etkinlik ve hedef davranış kataloğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0226 | `components/Ekranlar.tsx:675` | JsxText | etkinlik · DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0227 | `components/Ekranlar.tsx:675` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0228 | `components/Ekranlar.tsx:675` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0229 | `components/Ekranlar.tsx:675` | JsxText | · BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0230 | `components/Ekranlar.tsx:675` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0231 | `components/Ekranlar.tsx:677` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0232 | `components/Ekranlar.tsx:677` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0233 | `components/Ekranlar.tsx:680` | TemplateHead | Tümü ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0234 | `components/Ekranlar.tsx:680` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0235 | `components/Ekranlar.tsx:680` | TemplateHead | DEP-2026 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0236 | `components/Ekranlar.tsx:680` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0237 | `components/Ekranlar.tsx:680` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0238 | `components/Ekranlar.tsx:680` | TemplateHead | BGM-12 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0239 | `components/Ekranlar.tsx:680` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0240 | `components/Ekranlar.tsx:689` | StringLiteral | Tümü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0241 | `components/Ekranlar.tsx:694` | StringLiteral | Etkinliği düzenle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0242 | `components/Ekranlar.tsx:694` | StringLiteral | Yeni etkinlik ekle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0243 | `components/Ekranlar.tsx:694` | JsxText | · kayıt bu cihazda saklanır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0244 | `components/Ekranlar.tsx:696` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0245 | `components/Ekranlar.tsx:696` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0246 | `components/Ekranlar.tsx:696` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0247 | `components/Ekranlar.tsx:697` | JsxText | DEP-2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0248 | `components/Ekranlar.tsx:697` | JsxText | BGM-12 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0249 | `components/Ekranlar.tsx:699` | StringLiteral | Etkinlik adı * | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0250 | `components/Ekranlar.tsx:700` | StringLiteral | Hedef kod (örn 3.1.2 / BGM-FS-1) * | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0251 | `components/Ekranlar.tsx:701` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0252 | `components/Ekranlar.tsx:702` | StringLiteral | İpucu kademesi (örn Model→bağımsız) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0253 | `components/Ekranlar.tsx:703` | StringLiteral | Malzeme (virgülle ayır) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0254 | `components/Ekranlar.tsx:706` | StringLiteral | Güncelle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0255 | `components/Ekranlar.tsx:707` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0256 | `components/Ekranlar.tsx:707` | JsxText | İptal | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0257 | `components/Ekranlar.tsx:708` | JsxText | Varsayılana sıfırla | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0258 | `components/Ekranlar.tsx:715` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0259 | `components/Ekranlar.tsx:715` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0260 | `components/Ekranlar.tsx:718` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0261 | `components/Ekranlar.tsx:719` | JsxText | İpucu kademesi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0262 | `components/Ekranlar.tsx:720` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0263 | `components/Ekranlar.tsx:722` | JsxText | Düzenle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0264 | `components/Ekranlar.tsx:723` | JsxText | Sil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0265 | `components/Ekranlar.tsx:728` | JsxText | Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0266 | `components/Ekranlar.tsx:728` | JsxText | — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0267 | `components/Ekranlar.tsx:738` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0268 | `components/Ekranlar.tsx:739` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0269 | `components/Ekranlar.tsx:748` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0270 | `components/Ekranlar.tsx:751` | StringLiteral | Bilişsel Geliştirme Modülleri (BGM-12) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0271 | `components/Ekranlar.tsx:752` | JsxText | modül · menü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0272 | `components/Ekranlar.tsx:754` | JsxText | İki katman. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0273 | `components/Ekranlar.tsx:757` | JsxText | Modül seçimi serbesttir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0274 | `components/Ekranlar.tsx:757` | JsxText | Persona sarmalı dayatılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0275 | `components/Ekranlar.tsx:760` | JsxText | TASLAK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0276 | `components/Ekranlar.tsx:760` | JsxText | Tam kartlar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0277 | `components/Ekranlar.tsx:760` | JsxText | SEDUVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0278 | `components/Ekranlar.tsx:771` | JsxText | Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0279 | `components/Ekranlar.tsx:772` | StringLiteral | henüz seçilmedi — 1-2-3 atlanabilir | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0280 | `components/Ekranlar.tsx:789` | JsxText | çekirdek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0281 | `components/Ekranlar.tsx:794` | JsxText | Programdan çıkar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0282 | `components/Ekranlar.tsx:796` | JsxText | Programa al | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0283 | `components/Ekranlar.tsx:798` | JsxText | Kart | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0284 | `components/Ekranlar.tsx:802` | JsxText | Tanım: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0285 | `components/Ekranlar.tsx:803` | JsxText | Amaç: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0286 | `components/Ekranlar.tsx:804` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0287 | `components/Ekranlar.tsx:805` | JsxText | Etkinlik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0288 | `components/Ekranlar.tsx:806` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0289 | `components/Ekranlar.tsx:806` | JsxText | İpucu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0290 | `components/Ekranlar.tsx:806` | JsxText | Girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0291 | `components/Ekranlar.tsx:807` | JsxText | Ödev: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0292 | `components/Ekranlar.tsx:808` | JsxText | Önlem: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0293 | `components/Ekranlar.tsx:809` | JsxText | Öneri: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0294 | `components/Ekranlar.tsx:810` | JsxText | DEP köprüsü: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0295 | `components/Ekranlar.tsx:810` | LastTemplateToken | — kanıt satırı önerisi; BEP birimi kararı değildir (K-263) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0296 | `components/Ekranlar.tsx:810` | StringLiteral | yok (bütünleştirme turu) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0297 | `components/Ekranlar.tsx:811` | JsxText | Dayanak: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0298 | `components/Kabuk.tsx:7` | StringLiteral | Eğitmen Kürsüsü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0299 | `components/Kabuk.tsx:10` | StringLiteral | Oturum Atölyesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0300 | `components/Kabuk.tsx:11` | StringLiteral | Etkinlik Kataloğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0301 | `components/Kabuk.tsx:12` | StringLiteral | İzleme Çizelgesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0302 | `components/Kabuk.tsx:13` | StringLiteral | Rapor Atölyesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0303 | `components/Kabuk.tsx:14` | StringLiteral | Program Hizalama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0304 | `components/Kabuk.tsx:15` | StringLiteral | Bilişsel Geliştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0305 | `components/Kabuk.tsx:16` | StringLiteral | RAM & BEP Takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0306 | `components/Kabuk.tsx:17` | StringLiteral | Ev Çalışmaları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0307 | `components/Kabuk.tsx:18` | StringLiteral | Aile & Öğretmen | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0308 | `components/Kabuk.tsx:32` | JsxText | SEDUVA Supporta™ | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0309 | `components/Kabuk.tsx:33` | JsxText | Uzman Kokpiti · v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0310 | `components/Kabuk.tsx:50` | JsxText | Rol: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0311 | `components/Kabuk.tsx:50` | JsxText | · Sentetik demo verisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0312 | `components/Kabuk.tsx:63` | JsxText | SEDUVA Supporta: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0313 | `components/Sherh.tsx:3` | StringLiteral | nötr | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0314 | `components/Sherh.tsx:3` | StringLiteral | nötr | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0315 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateHead | <!doctype html><title> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0316 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px;border:1px solid #e2e8f0;padding:12px;border-radius:10px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:12px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0317 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </h1><div class=muhur>ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER</div><pre> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0318 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;\|&nbsp; Kopya 2/2 — Kurum arşivi · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0319 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | · Supporta v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0320 | `components/aile/AileEgitimMerkezi.tsx:28` | JsxText | A — Genel (5 mini-modül) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0321 | `components/aile/AileEgitimMerkezi.tsx:36` | JsxText | B — Analize Göre (uzman seçer) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0322 | `components/aile/AileEgitimMerkezi.tsx:52` | JsxText | dk · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0323 | `components/aile/AileEgitimMerkezi.tsx:64` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0324 | `components/aile/AileEgitimMerkezi.tsx:70` | TemplateMiddle | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0325 | `components/aile/AileEgitimMerkezi.tsx:73` | JsxText | Yazdır / PDF | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0326 | `components/aile/AileEgitimMerkezi.tsx:81` | StringLiteral | Kopyalandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0327 | `components/aile/AileEgitimMerkezi.tsx:86` | JsxText | Kopyala | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0328 | `components/aile/AileEgitimMerkezi.tsx:90` | JsxText | · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0329 | `components/aile/AileEgitimMerkezi.tsx:97` | JsxText | Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0330 | `components/aile/AileEgitimMerkezi.tsx:102` | JsxText | Tetik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0331 | `components/aile/AileEgitimMerkezi.tsx:108` | JsxText | Aileye görev örneği: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0332 | `components/aile/AileEgitimMerkezi.tsx:110` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0333 | `components/aile/AileEgitimMerkezi.tsx:115` | TemplateMiddle | Görev: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0334 | `components/aile/AileEgitimMerkezi.tsx:115` | TemplateMiddle | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0335 | `components/aile/AileEgitimMerkezi.tsx:118` | JsxText | Şablonu Yazdır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0336 | `components/aile/AileEgitimMerkezi.tsx:121` | JsxText | · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0337 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Can B. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0338 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Görsel İpucu | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0339 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Düşük Uyaranlı Görev | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0340 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Ali Y. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0341 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Görev Parçalama | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0342 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Sözel Yönerge | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0343 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Elif S. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0344 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Zamanlayıcı | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0345 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Hareketli Mola | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0346 | `components/egitmen/EgitmenDestekPaneli.tsx:29` | JsxText | Eğitmen Destek Paneli (Supporta) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0347 | `components/egitmen/EgitmenDestekPaneli.tsx:35` | JsxText | Öğrenci Listesi | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0348 | `components/egitmen/EgitmenDestekPaneli.tsx:59` | JsxText | Destek Profili | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0349 | `components/egitmen/EgitmenDestekPaneli.tsx:60` | JsxText | Şu an uygulanan destek stratejisi ve performansı. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0350 | `components/egitmen/EgitmenDestekPaneli.tsx:65` | JsxText | Aktif Destek (Müdahale) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0351 | `components/egitmen/EgitmenDestekPaneli.tsx:69` | JsxText | İstikrarlı Başarı Serisi | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0352 | `components/egitmen/EgitmenDestekPaneli.tsx:70` | JsxText | Görev | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0353 | `components/egitmen/EgitmenDestekPaneli.tsx:79` | JsxText | Desteği Geri Çekme Önerisi (Support Fading) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0354 | `components/egitmen/EgitmenDestekPaneli.tsx:81` | JsxText | Bu öğrenci | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0355 | `components/egitmen/EgitmenDestekPaneli.tsx:81` | JsxText | stratejisinde uzmanlaştı. Bağımsızlığı artırmak adına,  ↵                     sonraki seansta desteği bir alt seviyeye indirmeyi (Fading) deneyebilirsiniz. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0356 | `components/egitmen/EgitmenDestekPaneli.tsx:85` | JsxText | Desteği Azalt / Kaldır | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0357 | `components/egitmen/EgitmenDestekPaneli.tsx:94` | JsxText | Toparlanma (Recovery) Zekası | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0358 | `components/egitmen/EgitmenDestekPaneli.tsx:95` | JsxText | Öğrencinin moladan veya kriz anından sonra en hızlı toparlandığı koşullar. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0359 | `components/egitmen/EgitmenDestekPaneli.tsx:99` | JsxText | En Verimli Dönüş (Transition) Aracı: | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0360 | `components/egitmen/EgitmenDestekPaneli.tsx:105` | JsxText | Öneri: Mola dönüşlerinde yüksek uyaranlı veya zor görevlerden kaçının. Başlangıçta | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0361 | `components/egitmen/EgitmenDestekPaneli.tsx:105` | JsxText | vererek bilişsel geçişi (transition) kolaylaştırın. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-SED-0362 | `data/aile/genel.ts:19` | StringLiteral | Nasihat ve Kıyas Yok — Gözlem Dili | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0363 | `data/aile/genel.ts:20` | StringLiteral | Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0364 | `data/aile/genel.ts:22` | StringLiteral | “Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0365 | `data/aile/genel.ts:23` | StringLiteral | “Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0366 | `data/aile/genel.ts:24` | StringLiteral | Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0367 | `data/aile/genel.ts:27` | StringLiteral | A4 gözlem kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0368 | `data/aile/genel.ts:28` | StringLiteral | Yorum/değer yargısı yok — yalnızca gözlem. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0369 | `data/aile/genel.ts:32` | StringLiteral | Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0370 | `data/aile/genel.ts:33` | StringLiteral | Yazılı planla öngörülebilirlik sağlamak (Z-1). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0371 | `data/aile/genel.ts:35` | StringLiteral | Akşam rutinini 5 soruyla duvara asın: ne yapılacak · ne zaman · nerede · ne kadar · sonra ne var (Tablo 9/10 kavramı). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0372 | `data/aile/genel.ts:36` | StringLiteral | Resimli/renkli kartta her adım tek satır, tik kutusu ekleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0373 | `data/aile/genel.ts:37` | StringLiteral | Planı çocukla birlikte hazırlayın, her gün aynı yerde tutun. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0374 | `data/aile/genel.ts:40` | StringLiteral | rutin şablonu (A4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0375 | `data/aile/genel.ts:40` | StringLiteral | renkli kalem | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0376 | `data/aile/genel.ts:44` | StringLiteral | Görsel Ortam — Uyaran Yalıtımı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0377 | `data/aile/genel.ts:45` | StringLiteral | Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-7 görsel). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0378 | `data/aile/genel.ts:47` | StringLiteral | Masada yalnızca o derste gerekli materyal kalsın, fazlası kutuya. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0379 | `data/aile/genel.ts:48` | StringLiteral | Dersten önce yüzey toplama ritüeli: 1 dk birlikte toplayın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0380 | `data/aile/genel.ts:49` | StringLiteral | Duvarlarda hareketli/ışıklı uyaranı çalışma anında kaldırın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0381 | `data/aile/genel.ts:52` | StringLiteral | toplama kutusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0382 | `data/aile/genel.ts:56` | StringLiteral | İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0383 | `data/aile/genel.ts:57` | StringLiteral | İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + Z-7 işitsel). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0384 | `data/aile/genel.ts:59` | StringLiteral | Çalışma anında TV/arka plan sesini kapatın, kapıyı kapalı tutun. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0385 | `data/aile/genel.ts:60` | StringLiteral | Yönergeyi göz hizasında, tek cümle, 2 adımı geçmeden söyleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0386 | `data/aile/genel.ts:61` | StringLiteral | Gerekirse söze değil, hafif dokunarak (omuz) dikkat toplayın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0387 | `data/aile/genel.ts:68` | StringLiteral | Pekiştireç ve Kayıt — Hedef Davranış + İpucu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0388 | `data/aile/genel.ts:69` | StringLiteral | Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 uyumlu çerçeve, Z-2). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0389 | `data/aile/genel.ts:71` | StringLiteral | Tek hedef seçin: “ödevin ilk 10 dk’sında masada kalma”. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0390 | `data/aile/genel.ts:72` | StringLiteral | İpucu kademesi: model → sözel hatırlatma → bağımsız; ipucunu kademeli çekin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0391 | `data/aile/genel.ts:73` | StringLiteral | Her gün “yaptı / yapmadı” tik kartına işleyin, haftalık uzmana getirin (dijital puan yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0392 | `data/aile/genel.ts:76` | StringLiteral | hedef kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0393 | `data/aile/genel.ts:76` | StringLiteral | tik tablosu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0394 | `data/aile/genel.ts:77` | StringLiteral | Pekiştireç maddi değil, etkinlik/övgü temelli olabilir — uzman belirler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0395 | `data/aile/kisisel.ts:18` | StringLiteral | İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0396 | `data/aile/kisisel.ts:19` | StringLiteral | Analize Göre Aile Görevi (Uzman Seçer) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0397 | `data/aile/kisisel.ts:20` | FirstTemplateToken | [UZMAN DOLDURUR — K-02] ↵ Gözlem/Rapor bulgusu (tarihli, sayılabilir): ... ↵ Aileye önerilen tek görev (1 cümle, bağlamlı): ... ↵ İpucu kademesi (model/sözel/bağımsız): ... ↵ Kayıt biçimi (tik/süre): ... ↵ Sonraki izleme tarihi: ... | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0398 | `data/aile/kisisel.ts:21` | StringLiteral | Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0399 | `data/aile/kisisel.ts:22` | StringLiteral | Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0400 | `data/aile/kisisel.ts:27` | StringLiteral | Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0401 | `data/aile/kisisel.ts:27` | StringLiteral | Çizelgede kopma > eşik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0402 | `data/aile/kisisel.ts:28` | StringLiteral | Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0403 | `data/aile/kisisel.ts:28` | StringLiteral | Ev Çalışmaları “yapılmadı” >2 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0404 | `data/aile/kisisel.ts:29` | StringLiteral | Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0405 | `data/aile/kisisel.ts:29` | StringLiteral | Girdi “0/3” yoğun | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0406 | `data/bgm.ts:15` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0407 | `data/bgm.ts:47` | StringLiteral | Grup I — bilişsel kararlılık (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0408 | `data/bgm.ts:48` | StringLiteral | Grup II — esneklik ve düzenleme (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0409 | `data/bgm.ts:49` | StringLiteral | Grup III — uygulama ve otonomi (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0410 | `data/bgm.ts:54` | StringLiteral | Odak Kararlılığı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0411 | `data/bgm.ts:54` | StringLiteral | Görevi sürdürme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0412 | `data/bgm.ts:55` | StringLiteral | Sürdürülebilir dikkat | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0413 | `data/bgm.ts:56` | StringLiteral | Kısa süreli bir görevi, çeldirici varken bile bırakmadan sürdürme alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0414 | `data/bgm.ts:57` | StringLiteral | Seans içinde kesintisiz çalışma süresini gözlemek; uzman hedefi BEP satırına taşır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0415 | `data/bgm.ts:58` | StringLiteral | Kesintisiz odak süresi (dk) · isabet / yanlış basış (CPT deseni). Yüzdelik ve tanı YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0416 | `data/bgm.ts:59` | StringLiteral | Kısa görsel tarama turu: hedef şekil belirdiğinde dokun, diğerlerinde bekle. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0417 | `data/bgm.ts:60` | StringLiteral | Evde 5 dk tek görev (kitap/çalışma yaprağı). Puanlanmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0418 | `data/bgm.ts:61` | StringLiteral | Masada yalnız o anki materyal; ekran ve televizyon görüş alanında olmasın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0419 | `data/bgm.ts:62` | StringLiteral | Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0420 | `data/bgm.ts:64` | StringLiteral | 5–7 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0421 | `data/bgm.ts:65` | StringLiteral | tarama kart seti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0422 | `data/bgm.ts:65` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0423 | `data/bgm.ts:66` | StringLiteral | model → sözel ("hedefi bekle") → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0424 | `data/bgm.ts:68` | StringLiteral | CPT görev ailesi · PMC 5-küme ⑤ çevre kontrolü (literatür atfı; SEDUVA sonucu değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0425 | `data/bgm.ts:71` | StringLiteral | Zaman Algısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0426 | `data/bgm.ts:71` | StringLiteral | Süre tahmini | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0427 | `data/bgm.ts:72` | StringLiteral | Zamanı ayarlama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0428 | `data/bgm.ts:73` | StringLiteral | Bir işin ne kadar süreceğini tahmin etme ve gerçek süreyle karşılaştırma. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0429 | `data/bgm.ts:74` | StringLiteral | “Az kaldı / çok kaldı” hissini sayılabilir süreyle eşlemek (takvim “hafta” değil, seans içi süre). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0430 | `data/bgm.ts:75` | StringLiteral | Tahmin − gerçek süre farkı (sn). Persona “İç Saat” ile aynı aile. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0431 | `data/bgm.ts:76` | StringLiteral | Kum saati tahmini: uzman 30/60/90 sn tutar, çocuk işaretler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0432 | `data/bgm.ts:77` | StringLiteral | Akşam rutininin bir adımına süre koyun (ör. çanta hazırlığı). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0433 | `data/bgm.ts:78` | StringLiteral | Görünür analog saat veya kum saati; sözel “acele et” yerine süre göstergesi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0434 | `data/bgm.ts:79` | StringLiteral | Geçiş uyarısı (Z-13) seans bitimine 5 ve 1 dk kala — utançsız dil. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0435 | `data/bgm.ts:81` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0436 | `data/bgm.ts:82` | StringLiteral | kum saati / analog kronometre | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0437 | `data/bgm.ts:82` | StringLiteral | tahmin kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0438 | `data/bgm.ts:83` | StringLiteral | görsel sayaç açık → yarı kapalı → kapalı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0439 | `data/bgm.ts:85` | StringLiteral | TMT-A / süre tahmini görev ailesi · PMC 5-küme ③ rutin-zamanlama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0440 | `data/bgm.ts:88` | StringLiteral | Parçalama (Chunking) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0441 | `data/bgm.ts:88` | StringLiteral | İşi bölme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0442 | `data/bgm.ts:89` | StringLiteral | Göreve başlama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0443 | `data/bgm.ts:90` | StringLiteral | Büyük işi tek adımlık parçalara bölme; ilk adımı görünür kılma (Z-15). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0444 | `data/bgm.ts:91` | StringLiteral | Başlayamamayı “tembellik” diye değil, ilk-adım eksikliği olarak ele almak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0445 | `data/bgm.ts:92` | StringLiteral | İlk eyleme kadar geçen süre · tamamlanan parça sayısı. Ölçüm yorumunu uzman yazar. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0446 | `data/bgm.ts:93` | StringLiteral | Görevi 3 karta böl: 1) bak 2) ilk satır 3) bırak. Kart 1 bitmeden 2 açılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0447 | `data/bgm.ts:94` | StringLiteral | Yarınki ödevi velinin yanında 3 kutuya yazın. Sistem puanlamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0448 | `data/bgm.ts:95` | StringLiteral | Yönerge en fazla 2 adım (Z-8); üçüncü adım ayrı cümle. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0449 | `data/bgm.ts:96` | StringLiteral | İpucu kademesi: model → sözel → bağımsız; silikleştirme notu uzmanda. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0450 | `data/bgm.ts:98` | StringLiteral | 6–8 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0451 | `data/bgm.ts:99` | StringLiteral | çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0452 | `data/bgm.ts:99` | StringLiteral | 3 boş kart | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0453 | `data/bgm.ts:100` | StringLiteral | model (uzman böler) → sözel → bağımsız (çocuk böler) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0454 | `data/bgm.ts:102` | StringLiteral | PMC 5-küme ① hedef-koçluk + ④ basit geri bildirim · MEB DEHB Bülteni "küçük parçalara bölme" (kavram atfı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0455 | `data/bgm.ts:105` | StringLiteral | Bilgi Mimarisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0456 | `data/bgm.ts:105` | StringLiteral | Çalışma belleği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0457 | `data/bgm.ts:106` | StringLiteral | Çalışma belleği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0458 | `data/bgm.ts:107` | StringLiteral | Kısa süreli tutulan bilgiyi sırayla geri çağırma alıştırması (Digit Span / N-Back deseni). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0459 | `data/bgm.ts:108` | StringLiteral | Antrenman + dış araç (liste, görsel plan) birlikte; yalnız “ezber kası” değil. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0460 | `data/bgm.ts:109` | StringLiteral | Doğru dizi uzunluğu · Digit Span. Dış araç kullanımı gözlem notu (var/yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0461 | `data/bgm.ts:110` | StringLiteral | Sayı Dedektifi: 3–5 birimlik dizi, sözel tekrar. İpucu: görsel destek kademeli kalkar. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0462 | `data/bgm.ts:111` | StringLiteral | Kapıya asılı 3 maddelik “yanına al” listesi (Ö-5 dış bellek). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0463 | `data/bgm.ts:112` | StringLiteral | Sözel yönergeyi yazılı/çizili kopyayla destekleyin; tek kanal yeterli olmayabilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0464 | `data/bgm.ts:113` | StringLiteral | Dış bellek aracı = zayıflık değil, düzenleme. Karşılaştırma dili yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0465 | `data/bgm.ts:115` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0466 | `data/bgm.ts:116` | StringLiteral | sayı/nesne kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0467 | `data/bgm.ts:116` | StringLiteral | küçük tahta | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0468 | `data/bgm.ts:117` | StringLiteral | görsel destek açık → kademeli kalkar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0469 | `data/bgm.ts:119` | StringLiteral | Digit Span / N-Back görev ailesi · transfer iddiası YOK (Cogmed-tipi RED) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0470 | `data/bgm.ts:122` | StringLiteral | Bilişsel Esneklik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0471 | `data/bgm.ts:122` | StringLiteral | Kural değiştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0472 | `data/bgm.ts:123` | StringLiteral | Set değiştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0473 | `data/bgm.ts:124` | StringLiteral | Kurallar değişince eski kuralı bırakıp yenisine geçme alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0474 | `data/bgm.ts:125` | StringLiteral | “Ama demin şöyleydi” takılmasını görünür kılmak; esneklik iddiası yok, gözlem var. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0475 | `data/bgm.ts:126` | StringLiteral | Kural değişiminden sonra ilk doğru tepkiye kadar deneme sayısı (TMT-B / task-switching deseni). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0476 | `data/bgm.ts:127` | StringLiteral | Renk-şekil değiştirme: ilk tur “kırmızıya bas”, ikinci tur “yuvarlağa bas”. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0477 | `data/bgm.ts:128` | StringLiteral | Evde bir oyunun kuralını bilinçli değiştirin (bir tur). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0478 | `data/bgm.ts:129` | StringLiteral | Kural değişimini ses yükseltmeden, kısa cümleyle, göz hizasında bildirin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0479 | `data/bgm.ts:130` | StringLiteral | Hata = kural geçişi verisi; “beceremedin” dili yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0480 | `data/bgm.ts:132` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0481 | `data/bgm.ts:133` | StringLiteral | renk-şekil kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0482 | `data/bgm.ts:134` | StringLiteral | geçişte model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0483 | `data/bgm.ts:136` | StringLiteral | TMT-B / task-switching görev ailesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0484 | `data/bgm.ts:139` | StringLiteral | Dürtü Engelleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0485 | `data/bgm.ts:140` | StringLiteral | İnhibitör kontrol | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0486 | `data/bgm.ts:141` | StringLiteral | Tepki vermeden önce kısa bir durak (Go/No-Go). Ö-1 “Dur–Düşün–Uygula” kartı burada. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0487 | `data/bgm.ts:142` | StringLiteral | Antrenman (Işık Yakala) + bilişsel strateji kartı birlikte; yalnız refleks değil. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0488 | `data/bgm.ts:143` | StringLiteral | Yanlış basış oranı (commission) · strateji kartı kullanıldı mı (E/H, puan değil). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0489 | `data/bgm.ts:144` | StringLiteral | Işık Yakala: yeşilde dokun, kırmızıda bekle. Seans öncesi 3 adımlık kart. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0490 | `data/bgm.ts:145` | StringLiteral | Kapı eşiğinde “üç say, sonra geç” ritüeli. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0491 | `data/bgm.ts:146` | StringLiteral | Yönergeyi bitirmeden çocuktan eylem beklemeyin; omza hafif temaslı dikkat çekme (kavram, kopya değil). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0492 | `data/bgm.ts:147` | StringLiteral | Seans sonu yansıma: “Bugün acele ettiğin bir an oldu mu?” — sistem yorumlamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0493 | `data/bgm.ts:149` | StringLiteral | 6 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0494 | `data/bgm.ts:150` | StringLiteral | yeşil/kırmızı kartlar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0495 | `data/bgm.ts:150` | StringLiteral | 3 adımlık strateji kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0496 | `data/bgm.ts:151` | StringLiteral | kart açık → kart kapalı hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0497 | `data/bgm.ts:153` | StringLiteral | Go/No-Go görev ailesi · davranış terapisi kategorisi (DBRC/token; literatür atfı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0498 | `data/bgm.ts:156` | StringLiteral | Düzenleme Desteği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0499 | `data/bgm.ts:156` | StringLiteral | Nefes / mola | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0500 | `data/bgm.ts:157` | StringLiteral | Duygu ve uyarılma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0501 | `data/bgm.ts:158` | StringLiteral | Yoğunluk artınca kısa, donanımsız durak (A-1 Nefes Ritmi). Biyogeribildirim / PPG YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0502 | `data/bgm.ts:159` | StringLiteral | Engellenme anında görevi bırakmadan 30–60 sn düzenleme alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0503 | `data/bgm.ts:160` | StringLiteral | Mola isteği sayısı · mola sonrası göreve dönüş (E/H). “İyileşti” cümlesi YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0504 | `data/bgm.ts:161` | StringLiteral | Nefes halkası: ekranda yavaşça büyüyen daire; çocuk birlikte nefes alır, sonra devam. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0505 | `data/bgm.ts:162` | StringLiteral | Evde “zamanlı mola”: süre söylenir, bitince sorun birlikte konuşulur. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0506 | `data/bgm.ts:163` | StringLiteral | Nasihat, kıyas, ses yükseltme yok. Uzman/veli model olur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0507 | `data/bgm.ts:164` | StringLiteral | Mightier tipi klinik etki rakamı DEVİR ALINMAZ (K-04). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0508 | `data/bgm.ts:166` | StringLiteral | 2–3 dk (ihtiyaç anında) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0509 | `data/bgm.ts:167` | StringLiteral | nefes halkası kartı / ekran | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0510 | `data/bgm.ts:168` | StringLiteral | birlikte → sözel → çocuk kendi başlatır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0511 | `data/bgm.ts:170` | StringLiteral | A-1 Nefes Ritmi (Gelişim Önerileri v1.2) · donanımsız; biyogeribildirim YOK | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0512 | `data/bgm.ts:173` | StringLiteral | Önceliklendirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0513 | `data/bgm.ts:173` | StringLiteral | Önemli / acil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0514 | `data/bgm.ts:175` | StringLiteral | Sınırlı zamanda hangi işin önce geleceğini seçme alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0515 | `data/bgm.ts:176` | StringLiteral | Hepsinin birden yapılması beklentisini kırmak; sıra uzman ve çocukla kurulur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0516 | `data/bgm.ts:177` | StringLiteral | İlk seçim süresi · seçilen işin bitip bitmediği (gözlem). Verim yüzdesi iddiası yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0517 | `data/bgm.ts:178` | StringLiteral | Üç kart: kolay-kısa, zor-kısa, kolay-uzun. Çocuk birini seçer, gerekçesini söyler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0518 | `data/bgm.ts:179` | StringLiteral | Yarınki üç işi “önce / sonra / olursa” diye yazın (Tablo 9 kavramı, cümle kopyası yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0519 | `data/bgm.ts:180` | StringLiteral | Aynı anda tek açık iş; diğer kartlar kapalı durur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0520 | `data/bgm.ts:181` | StringLiteral | Sonuç önceden konuşulur (Ö-3 kontrat şablonuyla köprü). Sistem puanlamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0521 | `data/bgm.ts:183` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0522 | `data/bgm.ts:184` | StringLiteral | 3 görev kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0523 | `data/bgm.ts:184` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0524 | `data/bgm.ts:185` | StringLiteral | uzman gerekçeyi modeller → sorar → çocuk kendisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0525 | `data/bgm.ts:187` | StringLiteral | PMC 5-küme ① hedef-koçluk · koçluk RCT (yetişkin popülasyon notu) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0526 | `data/bgm.ts:190` | StringLiteral | Sosyal İpucu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0527 | `data/bgm.ts:190` | StringLiteral | Sıra / dinleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0528 | `data/bgm.ts:191` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0529 | `data/bgm.ts:191` | StringLiteral | Sosyal dikkat | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0530 | `data/bgm.ts:192` | StringLiteral | Sıra bekleme, söz bitmeden araya girmeme, yüz/ses ipucunu fark etme alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0531 | `data/bgm.ts:193` | StringLiteral | Açık sosyal beceri eğitimi değil; seans içi sıra ve dinleme gözlemi. Empati terapisi YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0532 | `data/bgm.ts:194` | StringLiteral | Sıra ihlali sayısı · söz bitmeden verilen erken yanıt (gözlem). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0533 | `data/bgm.ts:195` | StringLiteral | İki tur: biri konuşur, diğeri bekler; zil çalınca rol değişir (A-3 köprüsü, grup P2). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0534 | `data/bgm.ts:196` | StringLiteral | Evde yemek sırasında bir kişi konuşurken diğerinin bitmesini bekleme. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0535 | `data/bgm.ts:197` | StringLiteral | Grupta aynı anda tek konuşmacı; görsel “sıra çubuğu” masada durabilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0536 | `data/bgm.ts:198` | StringLiteral | Yapılandırılmış sosyal beceri programı (Ö-7) P2; bu kart onun yerini tutmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0537 | `data/bgm.ts:200` | StringLiteral | 6 dk (2 kişi) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0538 | `data/bgm.ts:201` | StringLiteral | sıra çubuğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0539 | `data/bgm.ts:202` | StringLiteral | çubuk görünür → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0540 | `data/bgm.ts:204` | StringLiteral | DEP M6 sıra alma hedef ailesi (kod referans) · A-3 eşli oyun | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0541 | `data/bgm.ts:207` | StringLiteral | Çift Kanal | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0542 | `data/bgm.ts:207` | StringLiteral | İki iş birden | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0543 | `data/bgm.ts:208` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0544 | `data/bgm.ts:208` | StringLiteral | Bölünmüş dikkat | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0545 | `data/bgm.ts:209` | StringLiteral | Görsel bir izleği sürdürürken basit işitsel hedefi yakalama alıştırması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0546 | `data/bgm.ts:210` | StringLiteral | Gürültülü ortamda tek kanala kapanmayı gözlemek. “Bant genişliği artırma” vaadi YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0547 | `data/bgm.ts:211` | StringLiteral | Tek kanal vs çift kanal isabet farkı (betimleyici). Stroop deseni referans. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0548 | `data/bgm.ts:212` | StringLiteral | Ortadaki şekli izle + kulaklıktan “çift sayı” deyince yan düğmeye bas. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0549 | `data/bgm.ts:213` | StringLiteral | Yok (evde çift kanal önerilmez; yorgunluk riski). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0550 | `data/bgm.ts:214` | StringLiteral | Seans odasında arka plan konuşması kısılır; gerekirse düşük sabit ses. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0551 | `data/bgm.ts:215` | StringLiteral | Yalnız uzman seansında; süre kısa tutulur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0552 | `data/bgm.ts:217` | StringLiteral | 4 dk (kısa) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0553 | `data/bgm.ts:218` | StringLiteral | izlek kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0554 | `data/bgm.ts:218` | StringLiteral | sayı listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0555 | `data/bgm.ts:219` | StringLiteral | tek kanal → çift kanal (yavaş ritim) → normal | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0556 | `data/bgm.ts:221` | StringLiteral | Stroop / dual-task görev ailesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0557 | `data/bgm.ts:224` | StringLiteral | Yüksek Yük | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0558 | `data/bgm.ts:224` | StringLiteral | Baskıda sakin kalma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0559 | `data/bgm.ts:225` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0560 | `data/bgm.ts:225` | StringLiteral | Yük altında sürdürme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0561 | `data/bgm.ts:226` | StringLiteral | Birden fazla kuralın aynı anda geldiği kısa tur; panik dili kullanılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0562 | `data/bgm.ts:227` | StringLiteral | Önceki alıştırmaların bir arada durup durmadığını gözlemek — “kriz tedavisi” değil. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0563 | `data/bgm.ts:228` | StringLiteral | Hata sonrası göreve dönüş (E/H) · tur yarıda bırakıldı mı. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0564 | `data/bgm.ts:229` | StringLiteral | Kısa “karışık tur”: dur-bekle + kural değişimi + süre. Çocuk durdurabilir (S-1). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0565 | `data/bgm.ts:230` | StringLiteral | Yok. Yüksek yük ev ödevi yapılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0566 | `data/bgm.ts:231` | StringLiteral | Çocuk kontrol çubuğu (mola/bitir) açık; ardışık zorlamada mola önerilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0567 | `data/bgm.ts:232` | StringLiteral | Tek oturumluk veriyle genelleme yok (Protokol §5.t). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0568 | `data/bgm.ts:234` | StringLiteral | 4 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0569 | `data/bgm.ts:235` | StringLiteral | önceki turların kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0570 | `data/bgm.ts:235` | StringLiteral | mola/bitir çubuğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0571 | `data/bgm.ts:236` | StringLiteral | uzman yükü kademeli açar; çocuk durdurabilir (S-1) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0572 | `data/bgm.ts:238` | StringLiteral | önceki modüllerin bütünleştirilmesi; ayrı görev ailesi yok | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0573 | `data/bgm.ts:241` | StringLiteral | Kendini Yönetme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0574 | `data/bgm.ts:241` | StringLiteral | Dış iskeleti solma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0575 | `data/bgm.ts:242` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0576 | `data/bgm.ts:242` | StringLiteral | Üstbiliş / otonomi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0577 | `data/bgm.ts:243` | StringLiteral | Hazır görevi çocuğun kendi planlaması; hatırlatıcı kademeli azalır (metakognisyon ONAYLI konum). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0578 | `data/bgm.ts:244` | StringLiteral | Platform iskeletini solmak; “karakter değişimi” vaadi YOK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0579 | `data/bgm.ts:245` | StringLiteral | Hatırlatıcısız başlama (E/H) · planladığı işe dönüş. Öz-başlatma endeksi betimleyicidir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0580 | `data/bgm.ts:246` | StringLiteral | Çocuk bugünkü gerçek işini (ödev/kitap) planlar; uzman yalnız izler, ipucu isterse verir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0581 | `data/bgm.ts:247` | StringLiteral | Kendi yazdığı 3 kutuluk planı odasına asmak (yazılı plan kavramı). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0582 | `data/bgm.ts:248` | StringLiteral | Karşılaştırma dili yok; her geribildirimde en az bir güçlü yön (Z-15). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0583 | `data/bgm.ts:249` | StringLiteral | Navigasyon: Kendini Yönetme (metakognisyon v1.0). Sistem otonomi ilan etmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0584 | `data/bgm.ts:251` | StringLiteral | 8–10 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0585 | `data/bgm.ts:252` | StringLiteral | 3 kutulu plan kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0586 | `data/bgm.ts:252` | StringLiteral | çocuğun kendi işi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0587 | `data/bgm.ts:253` | StringLiteral | istek üzerine → yok | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0588 | `data/bgm.ts:255` | StringLiteral | metakognisyon konumlandırma v1.0 (K-118/119) · ipucu silikleştirme (Activity Schedule deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0589 | `data/bgm.ts:262` | StringLiteral | BGM-12, DEP-2026'nın yerine geçmez. DEP = BEP/RAM saat hizası; BGM = yürütücü işlev menüsü. Uzman ikisinden de seçer. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0590 | `data/bgm.ts:266` | StringLiteral | BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0591 | `data/kisitlar.ts:8` | StringLiteral | Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0592 | `data/kisitlar.ts:10` | StringLiteral | Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0593 | `data/kisitlar.ts:12` | StringLiteral | Rapor taslaktır; uzman onayı olmadan geçerli belge değildir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0594 | `data/kisitlar.ts:16` | StringLiteral | Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0595 | `data/kisitlar.ts:17` | StringLiteral | Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0596 | `data/kisitlar.ts:18` | StringLiteral | TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0597 | `data/kisitlar.ts:19` | StringLiteral | Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0598 | `data/kisitlar.ts:20` | StringLiteral | Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0599 | `data/kisitlar.ts:21` | StringLiteral | SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0600 | `data/kisitlar.ts:26` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0601 | `data/kisitlar.ts:27` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0602 | `data/kisitlar.ts:28` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0603 | `data/kisitlar.ts:29` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0604 | `data/kisitlar.ts:31` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0605 | `data/kisitlar.ts:34` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0606 | `data/kisitlar.ts:38` | StringLiteral | x / + | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0607 | `data/kisitlar.ts:38` | StringLiteral | x: hedeflenen · +: ulaşılan (PKF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0608 | `data/kisitlar.ts:39` | StringLiteral | ölçüt düzeyi (PBF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0609 | `data/kisitlar.ts:40` | StringLiteral | Evet / Hayır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0610 | `data/kisitlar.ts:40` | StringLiteral | gözlendi / gözlenmedi (KDF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0611 | `data/kisitlar.ts:44` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0612 | `data/kisitlar.ts:44` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0613 | `data/kisitlar.ts:55` | StringLiteral | Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0614 | `data/kisitlar.ts:59` | StringLiteral | Devam/yoklama takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0615 | `data/kisitlar.ts:59` | StringLiteral | BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0616 | `data/kisitlar.ts:60` | StringLiteral | Ödeme · fatura · idari-mali işleyiş | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0617 | `data/kisitlar.ts:60` | StringLiteral | K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0618 | `data/kisitlar.ts:61` | StringLiteral | Resmî form üretimi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0619 | `data/kisitlar.ts:61` | StringLiteral | K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0620 | `data/kisitlar.ts:76` | StringLiteral | Ölçüt Bağımlı Test (ÖBT) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0621 | `data/kisitlar.ts:76` | StringLiteral | ilk / ara / son değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0622 | `data/kisitlar.ts:77` | StringLiteral | Tekrar ve deneme sayısı → Ölçüt alanı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0623 | `data/kisitlar.ts:77` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0624 | `data/kisitlar.ts:78` | StringLiteral | Kontrol Listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0625 | `data/kisitlar.ts:78` | StringLiteral | ilk / ara / son değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0626 | `data/kisitlar.ts:79` | StringLiteral | Evet/Hayır girdileri → Açıklamalar sütunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0627 | `data/kisitlar.ts:79` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0628 | `data/kisitlar.ts:80` | StringLiteral | Dereceli Puanlama Anahtarı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0629 | `data/kisitlar.ts:80` | StringLiteral | değerlendirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0630 | `data/kisitlar.ts:81` | StringLiteral | 0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0631 | `data/kisitlar.ts:81` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0632 | `data/kisitlar.ts:82` | StringLiteral | Performans Kayıt Formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0633 | `data/kisitlar.ts:82` | StringLiteral | her modülün başı ve sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0634 | `data/kisitlar.ts:83` | StringLiteral | x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0635 | `data/kisitlar.ts:83` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0636 | `data/kisitlar.ts:84` | StringLiteral | BEP Gelişimi İzleme Özet Formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0637 | `data/kisitlar.ts:84` | StringLiteral | süreç + yıl sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0638 | `data/kisitlar.ts:85` | StringLiteral | Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0639 | `data/kisitlar.ts:85` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0640 | `data/kisitlar.ts:86` | StringLiteral | Portfolyo Kontrol Listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0641 | `data/kisitlar.ts:86` | StringLiteral | modül sonu / yıl sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0642 | `data/kisitlar.ts:87` | StringLiteral | Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0643 | `data/kisitlar.ts:88` | StringLiteral | Portfolyo Dereceli Puanlama Anahtarı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0644 | `data/kisitlar.ts:88` | StringLiteral | portfolyo değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0645 | `data/kisitlar.ts:89` | StringLiteral | kapsam dışı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0646 | `data/kisitlar.ts:94` | StringLiteral | (a) Ücreti Bakanlıkça karşılanan | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0647 | `data/kisitlar.ts:94` | StringLiteral | ZORUNLU (rapor + ÖEDK planı + BKDS onamı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0648 | `data/kisitlar.ts:95` | StringLiteral | ÖEDK eğitim planı ekseninde | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0649 | `data/kisitlar.ts:96` | StringLiteral | (b) Ücretini kendisi/velisi karşılayan | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0650 | `data/kisitlar.ts:96` | StringLiteral | İSTENMİYOR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0651 | `data/kisitlar.ts:97` | StringLiteral | Kayıttaki ölçme sonuçlarıyla BEP birimince (md.24/6 · md.26/3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0652 | `data/kisitlar.ts:103` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0653 | `data/kisitlar.ts:103` | StringLiteral | Tüm dosyalar · rapor onayı · dışa aktarma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0654 | `data/kisitlar.ts:104` | StringLiteral | Uzman / Eğitimci | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0655 | `data/kisitlar.ts:104` | StringLiteral | Kendi dosyaları · oturum · girdi · rapor taslağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0656 | `data/mock.ts:6` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0657 | `data/mock.ts:6` | StringLiteral | Öğrenci A. (2. Sınıf) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0658 | `data/mock.ts:6` | StringLiteral | Atatürk İlkokulu / 2-B | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0659 | `data/mock.ts:7` | StringLiteral | Son ayda 2 gün | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0660 | `data/mock.ts:7` | StringLiteral | RAM eğitsel değerlendirme mevcut (2025) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0661 | `data/mock.ts:8` | StringLiteral | Veli A. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0662 | `data/mock.ts:8` | StringLiteral | 05xx xxx 41 17 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0663 | `data/mock.ts:8` | StringLiteral | İzmir / Bornova | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0664 | `data/mock.ts:9` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0665 | `data/mock.ts:9` | StringLiteral | Öğrenci B. (3. Sınıf) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0666 | `data/mock.ts:9` | StringLiteral | Cumhuriyet İlkokulu / 3-A | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0667 | `data/mock.ts:10` | StringLiteral | BEP dosyası okuldan bekleniyor | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0668 | `data/mock.ts:11` | StringLiteral | Veli B. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0669 | `data/mock.ts:11` | StringLiteral | 05xx xxx 29 03 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0670 | `data/mock.ts:11` | StringLiteral | İzmir / Karşıyaka | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0671 | `data/mock.ts:15` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0672 | `data/mock.ts:15` | StringLiteral | Haftada 1 (40 dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0673 | `data/mock.ts:16` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0674 | `data/mock.ts:17` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0675 | `data/mock.ts:17` | StringLiteral | Haftada 1 (40 dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0676 | `data/mock.ts:18` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0677 | `data/mock.ts:22` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0678 | `data/mock.ts:22` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0679 | `data/mock.ts:23` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0680 | `data/mock.ts:23` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0681 | `data/mock.ts:24` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0682 | `data/mock.ts:24` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0683 | `data/mock.ts:25` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0684 | `data/mock.ts:29` | StringLiteral | Hece ayırma çalışması | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0685 | `data/mock.ts:29` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0686 | `data/mock.ts:30` | StringLiteral | Sözel ipucu → model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0687 | `data/mock.ts:30` | StringLiteral | hece kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0688 | `data/mock.ts:30` | StringLiteral | çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0689 | `data/mock.ts:30` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0690 | `data/mock.ts:31` | StringLiteral | Sesli okuma — tekrarlı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0691 | `data/mock.ts:31` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0692 | `data/mock.ts:32` | StringLiteral | Eşli okuma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0693 | `data/mock.ts:32` | StringLiteral | kısa metin | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0694 | `data/mock.ts:32` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0695 | `data/mock.ts:33` | StringLiteral | Görsel dikkat eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0696 | `data/mock.ts:33` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0697 | `data/mock.ts:34` | StringLiteral | İşaret → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0698 | `data/mock.ts:34` | StringLiteral | eşleme kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0699 | `data/mock.ts:34` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0700 | `data/mock.ts:35` | StringLiteral | İşitsel bellek dizisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0701 | `data/mock.ts:35` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0702 | `data/mock.ts:36` | StringLiteral | Model → gecikmeli model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0703 | `data/mock.ts:36` | StringLiteral | ses kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0704 | `data/mock.ts:36` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0705 | `data/mock.ts:37` | StringLiteral | Sözcük dağarcığı — nesne adlandırma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0706 | `data/mock.ts:37` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0707 | `data/mock.ts:38` | StringLiteral | Fiziksel ipucu → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0708 | `data/mock.ts:38` | StringLiteral | nesne resimleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0709 | `data/mock.ts:38` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0710 | `data/mock.ts:39` | StringLiteral | Nesne niteliği ayırt etme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0711 | `data/mock.ts:39` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0712 | `data/mock.ts:40` | StringLiteral | Model → kısmi ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0713 | `data/mock.ts:40` | StringLiteral | blok seti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0714 | `data/mock.ts:40` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0715 | `data/mock.ts:41` | StringLiteral | Ritmik sayma (100 içinde) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0716 | `data/mock.ts:42` | StringLiteral | Birlikte sayma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0717 | `data/mock.ts:42` | StringLiteral | sayı doğrusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0718 | `data/mock.ts:42` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0719 | `data/mock.ts:43` | StringLiteral | Sıra alma ve bekleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0720 | `data/mock.ts:43` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0721 | `data/mock.ts:44` | StringLiteral | Model → sözel hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0722 | `data/mock.ts:44` | StringLiteral | sıra kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0723 | `data/mock.ts:44` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0724 | `data/mock.ts:44` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0725 | `data/mock.ts:46` | StringLiteral | Sürdürülebilir dikkat — nesne takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0726 | `data/mock.ts:46` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0727 | `data/mock.ts:47` | StringLiteral | Model → sözel ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0728 | `data/mock.ts:47` | StringLiteral | renkli toplar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0729 | `data/mock.ts:47` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0730 | `data/mock.ts:48` | StringLiteral | Yönerge izleme (2 adımlı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0731 | `data/mock.ts:48` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0732 | `data/mock.ts:49` | StringLiteral | Fiziksel rehber → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0733 | `data/mock.ts:49` | StringLiteral | yönerge kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0734 | `data/mock.ts:49` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0735 | `data/mock.ts:50` | StringLiteral | Dinlediğini anlama — kısa öykü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0736 | `data/mock.ts:50` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0737 | `data/mock.ts:51` | StringLiteral | Sözel ipucu → soru-cevap → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0738 | `data/mock.ts:51` | StringLiteral | öykü kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0739 | `data/mock.ts:51` | StringLiteral | soru listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0740 | `data/mock.ts:51` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0741 | `data/mock.ts:52` | StringLiteral | Sözel ifade — cümle kurma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0742 | `data/mock.ts:52` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0743 | `data/mock.ts:53` | StringLiteral | Model cümle → tamamlama → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0744 | `data/mock.ts:53` | StringLiteral | kelime kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0745 | `data/mock.ts:53` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0746 | `data/mock.ts:54` | StringLiteral | Karşılıklı konuşma sürdürme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0747 | `data/mock.ts:54` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0748 | `data/mock.ts:55` | StringLiteral | Sözel başlatma → sıra alma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0749 | `data/mock.ts:55` | StringLiteral | konu kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0750 | `data/mock.ts:55` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0751 | `data/mock.ts:55` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0752 | `data/mock.ts:56` | StringLiteral | Harf-ses eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0753 | `data/mock.ts:56` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0754 | `data/mock.ts:57` | StringLiteral | Model → eşleme → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0755 | `data/mock.ts:57` | StringLiteral | harf kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0756 | `data/mock.ts:57` | StringLiteral | ses kutusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0757 | `data/mock.ts:57` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0758 | `data/mock.ts:58` | StringLiteral | Yazma — harf dikte | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0759 | `data/mock.ts:58` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0760 | `data/mock.ts:59` | StringLiteral | Noktalı iz → kopya → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0761 | `data/mock.ts:59` | StringLiteral | dikte yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0762 | `data/mock.ts:59` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0763 | `data/mock.ts:60` | StringLiteral | Gruplama / sınıflama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0764 | `data/mock.ts:60` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0765 | `data/mock.ts:61` | StringLiteral | Model → sözel ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0766 | `data/mock.ts:61` | StringLiteral | sınıflama kutuları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0767 | `data/mock.ts:61` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0768 | `data/mock.ts:62` | StringLiteral | Birebir eşleştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0769 | `data/mock.ts:62` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0770 | `data/mock.ts:63` | StringLiteral | Fiziksel rehber → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0771 | `data/mock.ts:63` | StringLiteral | eş kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0772 | `data/mock.ts:63` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0773 | `data/mock.ts:64` | StringLiteral | Sıralama (büyük-küçük) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0774 | `data/mock.ts:64` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0775 | `data/mock.ts:65` | StringLiteral | Model → deneme-yanılma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0776 | `data/mock.ts:65` | StringLiteral | sıralama şeridi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0777 | `data/mock.ts:65` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0778 | `data/mock.ts:66` | StringLiteral | Sayı doğrusu ile toplama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0779 | `data/mock.ts:67` | StringLiteral | Model → rehberli → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0780 | `data/mock.ts:67` | StringLiteral | sayı doğrusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0781 | `data/mock.ts:67` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0782 | `data/mock.ts:68` | StringLiteral | Çıkarma (nesne ile) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0783 | `data/mock.ts:69` | StringLiteral | Nesne desteği → zihinden | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0784 | `data/mock.ts:69` | StringLiteral | sayma pulları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0785 | `data/mock.ts:69` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0786 | `data/mock.ts:70` | StringLiteral | Günlük yaşam problemi kurma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0787 | `data/mock.ts:71` | StringLiteral | Sözel senaryo → model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0788 | `data/mock.ts:71` | StringLiteral | problem kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0789 | `data/mock.ts:71` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0790 | `data/mock.ts:72` | StringLiteral | Duygu tanıma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0791 | `data/mock.ts:72` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0792 | `data/mock.ts:73` | StringLiteral | Görsel ipucu → eşleme → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0793 | `data/mock.ts:73` | StringLiteral | duygu kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0794 | `data/mock.ts:73` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0795 | `data/mock.ts:74` | StringLiteral | İş birliği oyunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0796 | `data/mock.ts:74` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0797 | `data/mock.ts:75` | StringLiteral | Eşli oyun → sıra alma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0798 | `data/mock.ts:75` | StringLiteral | kutu oyunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0799 | `data/mock.ts:75` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0800 | `data/mock.ts:76` | StringLiteral | Kurala uyma (oyun) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0801 | `data/mock.ts:76` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0802 | `data/mock.ts:77` | StringLiteral | Model → hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0803 | `data/mock.ts:77` | StringLiteral | kural kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0804 | `data/mock.ts:77` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0805 | `data/mock.ts:80` | StringLiteral | BGM — Odak Kararlılığı (Hedefi Yakala) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0806 | `data/mock.ts:80` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0807 | `data/mock.ts:80` | StringLiteral | tarama kart seti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0808 | `data/mock.ts:80` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0809 | `data/mock.ts:80` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0810 | `data/mock.ts:81` | StringLiteral | BGM — Zaman Algısı (Kum Saati Tahmini) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0811 | `data/mock.ts:81` | StringLiteral | Görsel sayaç açık → yarı kapalı → kapalı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0812 | `data/mock.ts:81` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0813 | `data/mock.ts:81` | StringLiteral | tahmin kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0814 | `data/mock.ts:81` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0815 | `data/mock.ts:82` | StringLiteral | BGM — Parçalama (Üç Kart) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0816 | `data/mock.ts:82` | StringLiteral | Model (uzman böler) → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0817 | `data/mock.ts:82` | StringLiteral | çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0818 | `data/mock.ts:82` | StringLiteral | 3 boş kart | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0819 | `data/mock.ts:82` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0820 | `data/mock.ts:83` | StringLiteral | BGM — Bilgi Mimarisi (Sayı Dedektifi) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0821 | `data/mock.ts:83` | StringLiteral | Görsel destek açık → kademeli kalkar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0822 | `data/mock.ts:83` | StringLiteral | sayı/nesne kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0823 | `data/mock.ts:83` | StringLiteral | küçük tahta | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0824 | `data/mock.ts:83` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0825 | `data/mock.ts:84` | StringLiteral | BGM — Bilişsel Esneklik (Renk mi Şekil mi?) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0826 | `data/mock.ts:84` | StringLiteral | Geçişte model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0827 | `data/mock.ts:84` | StringLiteral | renk-şekil kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0828 | `data/mock.ts:84` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0829 | `data/mock.ts:85` | StringLiteral | BGM — Dürtü Engelleme (Işık Yakala + 3 Adım) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0830 | `data/mock.ts:85` | StringLiteral | Kart açık → kapalı hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0831 | `data/mock.ts:85` | StringLiteral | yeşil/kırmızı kartlar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0832 | `data/mock.ts:85` | StringLiteral | strateji kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0833 | `data/mock.ts:85` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0834 | `data/mock.ts:86` | StringLiteral | BGM — Düzenleme Desteği (Nefes Halkası) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0835 | `data/mock.ts:86` | StringLiteral | Birlikte → sözel → çocuk kendi başlatır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0836 | `data/mock.ts:86` | StringLiteral | nefes halkası kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0837 | `data/mock.ts:86` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0838 | `data/mock.ts:87` | StringLiteral | BGM — Önceliklendirme (Önce Hangisi?) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0839 | `data/mock.ts:87` | StringLiteral | Uzman gerekçeyi modeller → sorar → çocuk kendisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0840 | `data/mock.ts:87` | StringLiteral | 3 görev kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0841 | `data/mock.ts:87` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0842 | `data/mock.ts:87` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0843 | `data/mock.ts:88` | StringLiteral | BGM — Sosyal İpucu (Sıra Çubuğu) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0844 | `data/mock.ts:88` | StringLiteral | Çubuk görünür → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0845 | `data/mock.ts:88` | StringLiteral | sıra çubuğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0846 | `data/mock.ts:88` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0847 | `data/mock.ts:89` | StringLiteral | BGM — Çift Kanal (Çift Görev) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0848 | `data/mock.ts:89` | StringLiteral | Tek kanal → çift kanal → normal | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0849 | `data/mock.ts:89` | StringLiteral | izlek kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0850 | `data/mock.ts:89` | StringLiteral | sayı listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0851 | `data/mock.ts:89` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0852 | `data/mock.ts:90` | StringLiteral | BGM — Yüksek Yük (Karışık Tur) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0853 | `data/mock.ts:90` | StringLiteral | Uzman yükü kademeli açar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0854 | `data/mock.ts:90` | StringLiteral | önceki tur kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0855 | `data/mock.ts:90` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0856 | `data/mock.ts:91` | StringLiteral | BGM — Kendini Yönetme (Kendi Planım) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0857 | `data/mock.ts:91` | StringLiteral | İstek üzerine → yok | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0858 | `data/mock.ts:91` | StringLiteral | 3 kutulu plan kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0859 | `data/mock.ts:91` | StringLiteral | çocuğun kendi işi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0860 | `data/mock.ts:91` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0861 | `data/mock.ts:101` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0862 | `data/mock.ts:101` | StringLiteral | Seans Özeti — 03.09.2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0863 | `data/mock.ts:103` | StringLiteral | Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0864 | `data/mock.ts:104` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0865 | `data/mock.ts:104` | StringLiteral | Aylık Gelişim Özeti — Ağustos 2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0866 | `data/mock.ts:105` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0867 | `data/mock.ts:106` | StringLiteral | Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0868 | `data/mock.ts:107` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0869 | `data/mock.ts:107` | StringLiteral | Dönem Sonu Değerlendirme — 2026 Güz | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0870 | `data/mock.ts:109` | StringLiteral | Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0871 | `data/mock.ts:110` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0872 | `data/mock.ts:110` | StringLiteral | BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0873 | `data/mock.ts:112` | StringLiteral | Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0874 | `data/mock.ts:113` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0875 | `data/mock.ts:113` | StringLiteral | RAM İzleme Paketi Hazırlığı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0876 | `data/mock.ts:115` | StringLiteral | Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0877 | `data/mock.ts:116` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0878 | `data/mock.ts:116` | StringLiteral | Aile Bilgilendirme Çıktısı — Eylül | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0879 | `data/mock.ts:117` | StringLiteral | Uzman / Eğitimci | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0880 | `data/mock.ts:118` | StringLiteral | Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0881 | `data/mock.ts:122` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0882 | `data/mock.ts:122` | StringLiteral | Mutfakta hece avı (5 nesne) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0883 | `data/mock.ts:123` | StringLiteral | Hafta içi 3 gün · 10 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0884 | `data/mock.ts:123` | StringLiteral | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0885 | `data/mock.ts:123` | StringLiteral | Çocuk istekliydi; 4 nesne bağımsız heceledi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0886 | `data/mock.ts:124` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0887 | `data/mock.ts:124` | StringLiteral | Gazete başlığı okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0888 | `data/mock.ts:125` | StringLiteral | Hafta sonu · 1 kez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0889 | `data/mock.ts:126` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0890 | `data/mock.ts:126` | StringLiteral | Sayı kartlarıyla eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0891 | `data/mock.ts:127` | StringLiteral | Hafta içi 2 gün | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0892 | `data/mock.ts:127` | StringLiteral | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0893 | `data/mock.ts:127` | StringLiteral | Aile yoğunluk bildirdi; süre kısaltıldı. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0894 | `data/mock.ts:131` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0895 | `data/mock.ts:132` | StringLiteral | İlk İnceleme tamamlandı (e-Rehberlik) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0896 | `data/mock.ts:133` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0897 | `data/mock.ts:134` | StringLiteral | (b) hattı — RAM raporu istenmiyor (ÖEKY md.20/2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0898 | `data/tipler.ts:11` | StringLiteral | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0899 | `data/tipler.ts:11` | StringLiteral | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0900 | `data/tipler.ts:29` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0901 | `data/tipler.ts:29` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0902 | `data/tipler.ts:42` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-SED-0903 | `data/tipler.ts:42` | StringLiteral | gerçekleşti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |

## Tam16 TS/TSX kaynak dosyası

Bu bölüm UI listesi değil; teknik alan/yorum/kullanılmayan kod ayrımı korunmalıdır. Satır numarası her bloğun ilk satırından başlar.

### `App.tsx`
3244 B ·SHA `15c1553c9e76a268afd492e8d319b17e6a5efc0d925997dbb04eb713704c317f`

~~~~tsx
import { useState } from 'react';
import Kabuk, { type EkranId } from './components/Kabuk';
import { Pano, Dosyalar, Takvim, OturumAtolyesi, Cizelge, RaporAtolyesi, Hizalama, Aile, Ayarlar, RamBep, EvOdevleri, EtkinlikKatalogu, BgmMenu } from './components/Ekranlar';
import { ROLLER, type RolId } from './data/kisitlar';

export default function App() {
  const [ekran, setEkran] = useState<EkranId>('pano');
  const [rol, setRol] = useState<RolId | null>(null);

  // Rol seçimi (spec §4-①). VELİ ROLÜ YOKTUR (K-296/KC7).
  if (!rol) {
    return (
      <div className="min-h-screen grid place-items-center p-6">
        <div className="max-w-lg w-full bg-white rounded-3xl border border-slate-200 p-8 space-y-5">
          <div className="text-center space-y-1">
            <div className="w-12 h-12 rounded-2xl bg-teal-600 text-white grid place-items-center font-black text-xl mx-auto">S</div>
            <h1 className="text-xl font-black">SEDUVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)</h1>
            <p className="text-xs text-slate-500">Özel eğitim merkezi uzman kokpiti · v{__SURUM__}</p>
          </div>
          <p className="text-sm text-slate-600 text-center">Devam etmek için rolünüzü seçin.</p>
          <div className="grid gap-2">
            {ROLLER.map((r) => (
              <button key={r.id} type="button" data-testid={`rol-${r.id}`} onClick={() => setRol(r.id)}
                className="text-left px-4 py-3 rounded-2xl border-2 border-slate-200 hover:border-teal-500 transition-colors">
                <div className="font-bold text-sm">{r.ad}</div>
                <div className="text-xs text-slate-500">{r.yetki}</div>
              </button>
            ))}
          </div>
          <p data-testid="veli-yok" className="text-[11px] text-slate-500 text-center border-t border-slate-100 pt-3">
            Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
          </p>
        </div>
      </div>
    );
  }
  const rolAd = ROLLER.find((r) => r.id === rol)!.ad;
  // üç-sınıf taksonomi (K-251): __PILOT__ kısıtlı, __TAM__ tam ürün, ikisi false ise DEMO
  const modEtiket = (typeof __PILOT__ !== 'undefined' && __PILOT__) ? 'PILOT — kısıtlı (takma ad, sunucusuz)' : (typeof __TAM__ !== 'undefined' && __TAM__) ? 'TAM — MEB dersleri aktif' : 'DEMO — jüri tanıtım';
  return (
    <Kabuk ekran={ekran} setEkran={setEkran} rol={rolAd}>
      <div data-testid="surum-modu" className="mb-3 rounded-xl border px-3 py-2 text-[11px] font-semibold text-center bg-slate-50 border-slate-200 text-slate-700">v{__SURUM__} · {modEtiket}</div>
      {ekran === 'pano' && <Pano />}
      {ekran === 'dosyalar' && <Dosyalar />}
      {ekran === 'takvim' && <Takvim />}
      {ekran === 'oturum' && <OturumAtolyesi />}
      {ekran === 'katalog' && <EtkinlikKatalogu />}
      {ekran === 'cizelge' && <Cizelge />}
      {ekran === 'rapor' && <RaporAtolyesi />}
      {ekran === 'hizalama' && <Hizalama />}
      {ekran === 'bgm' && <BgmMenu />}
      {ekran === 'rambep' && <RamBep />}
      {ekran === 'evodev' && <EvOdevleri />}
      {ekran === 'aile' && <Aile />}
      {ekran === 'ayarlar' && <Ayarlar />}
    </Kabuk>
  );
}

~~~~

### `components/Ekranlar.tsx`
56870 B ·SHA `28a4e25eb95d7c99ad8c5196eb8de5a3b74dec9b08bafa45152a4a8428be47cd`

~~~~tsx
/** SEDUVA Supporta™ MVP ekranları — spec §4 · 13 sekme (v0.8.0: BGM girdi döngüsüne bağlı, K-400). */
import { useMemo, useState } from 'react';
import { Brain, CheckCircle2, AlertTriangle, Printer, Plus, Trash2, Database, ChevronLeft, ChevronRight } from 'lucide-react';
import { useKalici } from '../lib/kullan';
import { temizle, kayitSayisi } from '../lib/depo';
import Sherh from './Sherh';
import { SHERHLER, YASA_1, YASA_2, DEP_MODULLER, DEP_TOPLAM_SAAT, KODLAMA, OTURUM_DURUM, MODUL_TERIM_NOTU, DERS_TAVAN, KAPSAM_DISI, RESMI_FORMLAR, KAYIT_HATTI } from '../data/kisitlar';
import { BGM_MODULLER, BGM_FAZ_ETIKET, BGM_KATMAN_NOTU, BGM_SAYI, BGM_TASLAK_NOTU, bgmEtkinlikId, bgmEtkinlikMi, bgmModulden, type BgmFaz } from '../data/bgm';
import { DOSYALAR, PROGRAMLAR, OTURUMLAR, ETKINLIKLER, GIRDILER, RAPORLAR, EV_ODEVLERI, RAM_KAYITLARI } from '../data/mock';
import AileEgitimMerkezi from './aile/AileEgitimMerkezi';
import type { Girdi, Rapor, EvOdevi, Gorusme, IpucuGozlem } from '../data/tipler';
import type { OturumDurum } from '../data/kisitlar';

const Kart = ({ baslik, children, ek }: { baslik: string; children: React.ReactNode; ek?: React.ReactNode }) => (
  <section className="bg-white rounded-2xl border border-slate-200 p-5 space-y-3">
    <div className="flex items-center justify-between gap-3">
      <h2 className="font-bold text-slate-900">{baslik}</h2>{ek}
    </div>
    {children}
  </section>
);

/* ---------- PANO ---------- */
export function Pano() {
  const bugun = OTURUMLAR.filter((o) => o.durum === 'planlandı');
  const bekleyen = RAPORLAR.filter((r) => r.taslak);
  return (
    <div className="space-y-4">
      <div className="bg-teal-50 border border-teal-200 rounded-2xl p-4 flex items-start gap-3">
        <Database className="w-5 h-5 text-teal-600 shrink-0 mt-0.5" />
        <div>
          <h3 className="font-bold text-teal-900 text-sm">Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif</h3>
          <p className="text-xs text-teal-700 leading-relaxed mt-1">Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.</p>
        </div>
      </div>
      
      <div className="grid sm:grid-cols-2 gap-4">
        <Kart baslik="T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)">
          <ul className="text-sm space-y-2">
            {bugun.map((o) => (
              <li key={o.id} data-testid="pano-oturum" className="flex items-center justify-between p-2 rounded-lg bg-slate-50 border border-slate-100">
                <span>{o.tarih} {o.saat} — {o.dosyaUid} ({o.sureDk} dk)</span>
                <div className="flex gap-1">
                    <span className="text-[10px] font-bold text-slate-500 bg-slate-200 px-1.5 py-0.5 rounded">T1 Merkezi</span>
                    <span className="text-[10px] font-bold text-indigo-500 bg-indigo-50 border border-indigo-200 px-1.5 py-0.5 rounded">T2 Okul Bekleniyor</span>
                </div>
              </li>
            ))}
          </ul>
        </Kart>
        <Kart baslik="Onay Bekleyen Raporlar (Human-Accountable AI)" ek={<span className="text-xs font-bold text-amber-700 bg-amber-50 border border-amber-200 rounded-full px-2 py-0.5">{bekleyen.length}</span>}>
          <ul className="text-sm space-y-1">{bekleyen.map((r) => <li key={r.id}>• {r.baslik}</li>)}</ul>
          <p className="text-[11px] text-slate-500 mt-2 italic">YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).</p>
        </Kart>
      </div>
    </div>
  );
}

/* ---------- DOSYALAR ---------- */
export function Dosyalar() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const d = DOSYALAR.find((x) => x.uid === sec)!;
  const p = PROGRAMLAR.find((x) => x.dosyaUid === sec)!;
  return (
    <>
      <Kart baslik="Dosya listesi">
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((x) => (
            <button key={x.uid} data-testid={`dosya-${x.uid}`} onClick={() => setSec(x.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === x.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {x.uid}
            </button>
          ))}
        </div>
      </Kart>
      <Kart baslik={`Dosya kartı — ${d.uid}`}>
        <dl className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          {[['Ad (maskeli)', d.ad], ['Doğum', d.dogum], ['Okul / Sınıf', d.okulSinif],
            ['Devamsızlık', d.devamsizlikNotu], ['Veli', `${d.veli.ad} · ${d.veli.tel}`],
            ['Rıza kaydı', d.veli.rizaTarihi ?? '—'], ['Geçmiş BEP', d.gecmisBepNotu]].map(([k, v]) => (
            <div key={k as string}><dt className="text-slate-500 text-xs">{k}</dt><dd className="font-medium">{v}</dd></div>
          ))}
        </dl>
      </Kart>
      <Kart baslik="Program kartı">
        <div className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          <div><span className="text-slate-500 text-xs block">Seans sayısı</span>{p.seansSayisi}</div>
          <div><span className="text-slate-500 text-xs block">Sıklık</span>{p.siklik}</div>
          <div><span className="text-slate-500 text-xs block">Aile bileşeni</span>{p.aileBileseni ? 'Var' : 'Yok'}</div>
          <div><span className="text-slate-500 text-xs block">RAM rapor ref.</span>{p.ramRaporRef}</div>
        </div>
        <Sherh metin={SHERHLER.aile} />
      </Kart>
    </>
  );
}

/* ---------- TAKVİM (etkileşimli + kalıcı) ---------- */
export function Takvim() {
  const [oturumlar, setOturumlar] = useKalici('oturumlar', OTURUMLAR);
  const [hafta, setHafta] = useState(0);            // 0 = 03.09 haftası
  const HAFTA_BAS = ['2026-08-27', '2026-09-03', '2026-09-10'];
  const aktifTarih = HAFTA_BAS[hafta + 1] ?? HAFTA_BAS[1];

  const gorunen = useMemo(
    () => oturumlar.filter((o) => Math.abs(new Date(o.tarih).getTime() - new Date(aktifTarih).getTime()) <= 6 * 864e5),
    [oturumlar, aktifTarih]);

  const cakisma = useMemo(() => {
    const m = new Map<string, number>();
    oturumlar.forEach((o) => { const k = `${o.tarih} ${o.saat} ${o.uzmanId}`; m.set(k, (m.get(k) ?? 0) + 1); });
    return [...m.entries()].filter(([, n]) => n > 1).map(([k]) => k);
  }, [oturumlar]);

  const durumDegistir = (id: string, d: OturumDurum) =>
    setOturumlar(oturumlar.map((o) => (o.id === id ? { ...o, durum: d } : o)));

  // K-571/A2: veli görüşme-randevu defteri (hatırlatma GÖNDERİLMEZ — K-334; yalnız yerel — K-05)
  const [gorusmeler, setGorusmeler] = useKalici<Gorusme[]>('gorusmeler', []);
  const [gTarih, setGTarih] = useState('2026-09-17');
  const [gKonu, setGKonu] = useState('');
  const gEkle = () => {
    if (!gKonu.trim()) return;
    setGorusmeler([...gorusmeler, { id: `GR-${gorusmeler.length + 1}`, dosyaUid: 'ÖĞR-4417', tarih: gTarih, konu: gKonu.trim(), durum: 'planlandı', not: '' }]);
    setGKonu('');
  };
  const gDurum = (id: string, d: Gorusme['durum']) => setGorusmeler(gorusmeler.map((g) => (g.id === id ? { ...g, durum: d } : g)));
  const gNot = (id: string, n: string) => setGorusmeler(gorusmeler.map((g) => (g.id === id ? { ...g, not: n } : g)));

  return (
    <>
    <Kart baslik="Oturum takvimi"
      ek={<div className="flex items-center gap-1">
        <button type="button" data-testid="hafta-geri" onClick={() => setHafta((h) => Math.max(-1, h - 1))}
          className="p-1.5 rounded-lg border border-slate-200 hover:bg-slate-50"><ChevronLeft className="w-4 h-4" /></button>
        <span data-testid="hafta-etiket" className="text-xs font-semibold px-2">{aktifTarih} haftası</span>
        <button type="button" data-testid="hafta-ileri" onClick={() => setHafta((h) => Math.min(1, h + 1))}
          className="p-1.5 rounded-lg border border-slate-200 hover:bg-slate-50"><ChevronRight className="w-4 h-4" /></button>
      </div>}>
      {cakisma.length > 0 && (
        <div data-testid="cakisma-uyari" className="flex items-center gap-2 text-xs font-semibold text-rose-700 bg-rose-50 border border-rose-200 rounded-xl px-3 py-2">
          <AlertTriangle className="w-4 h-4" /> Çakışma: {cakisma.join(' · ')} (KC12)
        </div>
      )}
      <table className="w-full text-sm">
        <thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200">
          <th className="py-2">Tarih</th><th>Saat</th><th>Dosya</th><th>Uzman</th><th>Durum</th></tr></thead>
        <tbody>
          {gorunen.map((o) => (
            <tr key={o.id} data-testid="takvim-satir" className="border-b border-slate-100">
              <td className="py-2">{o.tarih}</td><td>{o.saat}</td><td>{o.dosyaUid}</td><td>{o.uzmanId}</td>
              <td>
                <select data-testid={`durum-${o.id}`} value={o.durum}
                  onChange={(e) => durumDegistir(o.id, e.target.value as OturumDurum)}
                  className={`text-[11px] font-bold rounded-full px-2 py-1 border ${
                    o.durum === 'tamamlandı' ? 'bg-emerald-50 text-emerald-700 border-emerald-200' :
                    o.durum === 'planlandı' ? 'bg-sky-50 text-sky-700 border-sky-200' :
                    o.durum === 'gelmedi' ? 'bg-rose-50 text-rose-700 border-rose-200' : 'bg-slate-100 text-slate-600 border-slate-200'}`}>
                  {OTURUM_DURUM.map((d) => <option key={d} value={d}>{d}</option>)}
                </select>
              </td>
            </tr>
          ))}
          {gorunen.length === 0 && <tr><td colSpan={5} className="py-4 text-center text-slate-400 text-sm">Bu haftada oturum yok.</td></tr>}
        </tbody>
      </table>
      <p className="text-[11px] text-slate-500">Durumlar: {OTURUM_DURUM.join(' · ')} · değişiklikler bu cihazda saklanır.</p>
    </Kart>
    <Kart baslik="Veli görüşme-randevu defteri (K-571/A2)" ek={<span className="text-[11px] text-slate-500">hatırlatma gönderilmez — K-334</span>}>
      <div className="rounded-xl bg-amber-50 border border-amber-200 px-3 py-2 text-[11px] font-semibold text-amber-900" data-testid="gorusme-serit">
        Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
      </div>
      <div className="grid sm:grid-cols-3 gap-3 mt-3" data-testid="gorusme-form">
        <label className="text-sm space-y-1"><span className="text-xs text-slate-500 block">Tarih</span>
          <input data-testid="gorusme-tarih" type="date" value={gTarih} onChange={(e) => setGTarih(e.target.value)} className="w-full rounded-xl border border-slate-300 px-3 py-2" /></label>
        <label className="text-sm space-y-1"><span className="text-xs text-slate-500 block">Konu</span>
          <input data-testid="gorusme-konu" value={gKonu} onChange={(e) => setGKonu(e.target.value)} placeholder="örn. B yarı-dönem değerlendirme paylaşımı" className="w-full rounded-xl border border-slate-300 px-3 py-2" /></label>
        <div className="flex items-end"><button type="button" data-testid="gorusme-ekle" onClick={gEkle}
          className="px-4 py-2 rounded-xl bg-teal-600 text-white text-sm font-semibold">Deftere ekle</button></div>
      </div>
      {gorusmeler.length === 0
        ? <p data-testid="gorusme-bos" className="text-sm text-slate-500 mt-3">Defter boş — ilk görüşme kaydını ekleyin.</p>
        : <table className="w-full text-sm mt-3"><thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200"><th className="py-2">Tarih</th><th>Konu</th><th>Durum</th><th>Not</th></tr></thead>
          <tbody>{gorusmeler.map((g) => (
            <tr key={g.id} data-testid="gorusme-satir" className="border-b border-slate-100">
              <td className="py-2">{g.tarih}</td><td>{g.konu}</td>
              <td><select data-testid="gorusme-durum" value={g.durum} onChange={(e) => gDurum(g.id, e.target.value as Gorusme['durum'])} className="rounded-lg border border-slate-300 px-2 py-1 text-xs">
                {['planlandı', 'gerçekleşti', 'ertelendi', 'iptal'].map((d) => <option key={d} value={d}>{d}</option>)}</select></td>
              <td><input data-testid="gorusme-not" value={g.not} onChange={(e) => gNot(g.id, e.target.value)} placeholder="kısa not (yapılandırılmamış)" className="w-full rounded-lg border border-slate-200 px-2 py-1 text-xs" /></td>
            </tr>))}</tbody></table>}
      <p className="text-[11px] text-slate-400 mt-2">Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).</p>
    </Kart>
    </>
  );
}

/* ---------- OTURUM ATÖLYESİ (YASA-1 burada zorlanır) ---------- */
export function OturumAtolyesi() {
  const [etkinlik, setEtkinlik] = useState<string>('');
  const [tip, setTip] = useState<Girdi['kodlamaTipi']>('xArti');
  const [deger, setDeger] = useState('');
  const [ipucu, setIpucu] = useState<IpucuGozlem | ''>(''); // K-571/A4: gözlenen-ipucu-kademesi
  const [kayitlar, setKayitlar] = useKalici<Girdi[]>('girdiler', GIRDILER);
  // K-400: bu dosya için uzmanın seçtiği BGM modülleri (bgm-secim) oturumda ETKİNLİK olarak listelenir (YASA-1 işler).
  const [bgmSecim] = useKalici<Record<string, string[]>>('bgm-secim', { 'ÖĞR-4417': ['FS-1', 'II-6', 'CA-4'], 'ÖĞR-2903': [] });
  const dosyaUid = OTURUMLAR[0].dosyaUid; // OT-101
  const bgmSecili = BGM_MODULLER.filter((m) => (bgmSecim[dosyaUid] ?? []).includes(m.id));
  const secBgm = (id: string) => { setEtkinlik(id); const m = bgmModulden(id); if (m) setTip(m.girdiTipi); };
  const girilebilir = etkinlik !== '' && deger !== '';   // YASA-1
  const aktifBgm = bgmModulden(etkinlik);
  return (
    <>
      <Kart baslik="Oturum kartı — OT-101">
        <p className="text-sm text-slate-600">Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı</p>
        <p className="text-xs text-slate-500" data-testid="oturum-akis">
          Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)
        </p>
        <Sherh metin={SHERHLER.oturum} />
        <div className="rounded-xl border border-slate-300 bg-slate-50 px-3 py-2 text-[11px] font-semibold text-slate-700 flex items-start gap-2">
          <span className="shrink-0">ⓘ</span>
          <span>Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)</span>
        </div>
      </Kart>
      <Kart baslik="Bu oturumda seçili BGM modülleri" ek={<span className="text-[11px] text-slate-500">{dosyaUid} · sıra uzmanın</span>}>
        {bgmSecili.length === 0
          ? <p className="text-sm text-slate-500" data-testid="oturum-bgm-bos">Bu dosya için BGM seçilmedi (Bilişsel Geliştirme ekranından alınır). DEP etkinlikleri yine kullanılabilir.</p>
          : <div className="flex flex-wrap gap-2">
              {bgmSecili.map((m) => (
                <button key={m.id} type="button" data-testid={`oturum-bgm-${m.id}`} onClick={() => secBgm(bgmEtkinlikId(m.id))}
                  className={`text-left rounded-xl border px-3 py-2 text-xs ${etkinlik === bgmEtkinlikId(m.id) ? 'border-sky-500 bg-sky-50' : 'border-slate-200 bg-white'}`}>
                  <div className="font-semibold">{m.id} · {m.ad} <span className="text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5 ml-1">BGM</span></div>
                  <div className="text-slate-500">{m.sureDk} · girdi: {KODLAMA[m.girdiTipi].ad}{m.depKoprusu ? ` · DEP köprüsü ${m.depKoprusu}` : ''}</div>
                </button>
              ))}
            </div>}
        {aktifBgm && (
          <div data-testid="oturum-bgm-detay" className="rounded-xl bg-slate-50 border border-slate-200 px-3 py-2 text-[11px] text-slate-700 space-y-0.5">
            <div><b>Etkinlik:</b> {aktifBgm.etkinlik}</div>
            <div><b>Malzeme:</b> {aktifBgm.malzeme.join(' · ')} · <b>İpucu:</b> {aktifBgm.ipucu}</div>
            <div><b>Ölçüm:</b> {aktifBgm.olcum}</div>
          </div>
        )}
        <p className="text-[11px] text-slate-400">{BGM_TASLAK_NOTU}</p>
      </Kart>
      <Kart baslik="Hızlı girdi paneli" ek={<span className="text-[11px] text-slate-500">YASA-1 etkin</span>}>
        <div className="grid sm:grid-cols-3 gap-3">
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Etkinlik <b className="text-rose-600">*zorunlu</b></span>
            <select data-testid="girdi-etkinlik" value={etkinlik} onChange={(e) => setEtkinlik(e.target.value)}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              <option value="">— etkinlik seçin —</option>
              <optgroup label="DEP-2026 etkinlikleri">
                {ETKINLIKLER.map((e) => <option key={e.id} value={e.id}>{e.ad} ({e.hedefKod})</option>)}
              </optgroup>
              {bgmSecili.length > 0 && (
                <optgroup label="BGM-12 (bu dosya için seçili)">
                  {bgmSecili.map((m) => <option key={m.id} value={bgmEtkinlikId(m.id)}>[BGM] {m.id} · {m.ad}</option>)}
                </optgroup>
              )}
            </select>
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Kodlama</span>
            <select data-testid="girdi-tip" value={tip} onChange={(e) => setTip(e.target.value as Girdi['kodlamaTipi'])}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              {Object.entries(KODLAMA).map(([k, v]) => <option key={k} value={k}>{v.ad}</option>)}
            </select>
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Değer</span>
            <input data-testid="girdi-deger" value={deger} onChange={(e) => setDeger(e.target.value)}
              placeholder={KODLAMA[tip].aciklama} className="w-full rounded-xl border border-slate-300 px-3 py-2" />
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Gözlenen ipucu-kademesi (K-571/A4)</span>
            <select data-testid="girdi-ipucu" value={ipucu} onChange={(e) => setIpucu(e.target.value as IpucuGozlem | '')}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              <option value="">— seçilmeyebilir —</option>
              <option value="model">Model</option>
              <option value="sozel">Sözel</option>
              <option value="bagimsiz">Bağımsız</option>
            </select>
          </label>
        </div>
        {(() => { const e = ETKINLIKLER.find((x) => x.id === etkinlik); return e
          ? <p data-testid="girdi-kademe-plan" className="text-[11px] text-slate-500">Planlı ipucu-kademesi: {e.ipucuKademesi} · gözlem kaydı uzmanın teyididir (K-02: ölçüm-değil-gözlem).</p>
          : null; })()}
        <button type="button" data-testid="girdi-kaydet" disabled={!girilebilir}
          onClick={() => { setKayitlar([...kayitlar, { id: `G-${kayitlar.length + 1}`, oturumId: 'OT-101',
            etkinlikId: etkinlik, kodlamaTipi: tip, deger, tarih: '2026-09-03', girenRol: 'uzman', ipucuGozlem: ipucu || undefined }]); setDeger(''); }}
          className={`inline-flex items-center gap-1.5 px-4 py-2 rounded-xl text-sm font-semibold ${
            girilebilir ? 'bg-teal-600 text-white hover:bg-teal-700' : 'bg-slate-200 text-slate-400 cursor-not-allowed'}`}>
          <Plus className="w-4 h-4" /> Girdi kaydet
        </button>
        {!girilebilir && <p data-testid="yasa1-uyari" className="text-[11px] text-rose-600">{YASA_1}</p>}
        <ul className="text-sm space-y-1 pt-2 border-t border-slate-100">
          {kayitlar.map((g) => {
            const bgm = bgmModulden(g.etkinlikId);
            const e = ETKINLIKLER.find((x) => x.id === g.etkinlikId);
            const ad = bgm ? `${bgm.id} · ${bgm.ad}` : (e?.ad ?? g.etkinlikId);
            return (
              <li key={g.id} data-testid="girdi-satir" data-katman={bgm ? 'bgm' : 'dep'}>
                • {ad} {bgm && <span className="text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5">BGM</span>} → <b>{g.deger}</b>{' '}
                <span className="text-slate-400 text-xs">({KODLAMA[g.kodlamaTipi].ad})</span>
                {g.ipucuGozlem && <span className="text-slate-400 text-xs"> · ipucu(gözlenen): {{ model: 'Model', sozel: 'Sözel', bagimsiz: 'Bağımsız' }[g.ipucuGozlem]}</span>}
              </li>
            );
          })}
        </ul>
      </Kart>
    </>
  );
}

/* ---------- ÇİZELGE (YASA-2) ---------- */
export function Cizelge() {
  const [tum] = useKalici<Girdi[]>('girdiler', GIRDILER);
  // K-400: DEP ve BGM girdileri AYRI filtrelenir — iki katman karıştırılmaz (K-398 kuyruğu).
  const [katman, setKatman] = useState<'hepsi' | 'dep' | 'bgm'>('hepsi');
  const girdiler = tum.filter((g) => katman === 'hepsi' ? true : katman === 'bgm' ? bgmEtkinlikMi(g.etkinlikId) : !bgmEtkinlikMi(g.etkinlikId));
  const sayim = girdiler.length;
  const basari = girdiler.filter((g) => g.deger === '+' || g.deger === 'Evet' || g.deger === '3').length;
  const bgmSayi = tum.filter((g) => bgmEtkinlikMi(g.etkinlikId)).length;
  return (
    <>
      <div className="rounded-xl border border-amber-300 bg-amber-50 px-3 py-2 text-[11px] font-semibold text-amber-900 flex flex-col gap-1" data-testid="k4-serit">
        <span>Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz</span>
        <span>Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil</span>
      </div>
    <Kart baslik="DEP saat-izleri — girdilerden türetilmiş (K-571/A1)" ek={<span className="text-[11px] text-slate-500">YASA-2 deseni: elle çizilmez</span>}>
      <div data-testid="dep-saat-izleri">
        <table className="w-full text-sm"><thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200"><th className="py-2">Dosya</th><th>Tamamlanan oturum</th><th>Toplam süre</th><th>DEP girdisi</th></tr></thead>
        <tbody>{DOSYALAR.map((d) => {
          const ot = OTURUMLAR.filter((o) => o.dosyaUid === d.uid && o.durum === 'tamamlandı');
          const dk = ot.reduce((t, o) => t + o.sureDk, 0);
          const gdSayi = GIRDILER.filter((g) => { const o = OTURUMLAR.find((x) => x.id === g.oturumId); return o?.dosyaUid === d.uid && !bgmEtkinlikMi(g.etkinlikId); }).length;
          return <tr key={d.uid} data-testid="dep-saat-satir" className="border-b border-slate-100">
            <td className="py-2">{d.uid}</td><td>{ot.length}</td><td><b>{dk} dk</b></td><td>{gdSayi}</td></tr>;
        })}</tbody></table>
        <p className="text-[11px] text-slate-400 mt-2">Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).</p>
      </div>
    </Kart>
    <Kart baslik="İzleme çizelgesi" ek={<span className="text-[11px] text-slate-500">girdilerden türetildi</span>}>
      <div className="flex gap-1.5">
        {(['hepsi', 'dep', 'bgm'] as const).map((k) => (
          <button key={k} type="button" data-testid={`cizelge-filtre-${k}`} onClick={() => setKatman(k)}
            className={`px-2.5 py-1 rounded-lg text-[11px] border ${katman === k ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
            {k === 'hepsi' ? 'Tümü' : k === 'dep' ? 'DEP-2026' : `BGM-12 (${bgmSayi})`}
          </button>
        ))}
      </div>
      <div className="flex items-end gap-2 h-28" data-testid="cizelge-grafik">
        {girdiler.map((g, i) => (
          <div key={g.id} className="flex-1 flex flex-col items-center justify-end gap-1 h-full" data-katman={bgmEtkinlikMi(g.etkinlikId) ? 'bgm' : 'dep'}>
            {/* v0.8.0: yükseklik px — yüzde yükseklik esnek satırda 0'a çöküyordu (v0.7.0 görsel hatası) */}
            <div data-testid="cizelge-cubuk" className={`w-full rounded-t-lg ${bgmEtkinlikMi(g.etkinlikId) ? 'bg-sky-500' : 'bg-teal-500'}`}
              style={{ height: `${Math.min(96, 28 + i * 16)}px` }} />
            <span className="text-[10px] text-slate-500">{g.deger}</span>
          </div>
        ))}
      </div>
      <p className="text-sm">Toplam girdi: <b data-testid="cizelge-toplam">{sayim}</b> · Hedefe ulaşılan: <b>{basari}</b></p>
      <p className="text-[11px] text-slate-500" data-testid="cizelge-katman-notu">Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.</p>
      <Sherh metin={SHERHLER.cizelge} />
      <p className="text-[11px] text-slate-400">{YASA_2}</p>
    </Kart>
    </>
  );
}

/* ---------- RAPOR ATÖLYESİ (YASA-3) ---------- */
const TUR_ETIKET: Record<string, string> = {
  seans: 'Seans özeti', aylik: 'Aylık özet', donem: 'Dönem sonu',
  'bep-ilerleme': 'BEP ilerleme taslağı', 'ram-paketi': 'RAM izleme paketi',
  'aile-bilgilendirme': 'Aile bilgilendirme',
};

export function RaporAtolyesi() {
  const [liste, setListe] = useKalici<Rapor[]>('raporlar', RAPORLAR);
  const onayla = (id: string) => setListe(liste.map((r) => r.id === id ? { ...r, taslak: false, onayKim: 'Yönetici', onayTarih: '2026-09-03' } : r));

  // Human-Accountable AI: Eğitimsel Destek Önerisi (Uncertainty Layer eklendi)
  const sistemOnerisi = (r: Rapor) => {
    const ot = OTURUMLAR.filter((o) => o.dosyaUid === r.dosyaUid && o.durum === 'tamamlandı');
    const dk = ot.reduce((t, o) => t + o.sureDk, 0);
    const ozet = `

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: ${ot.length} T1 seansı, ${dk} dk aktif izlem)
Çocuğun dikkat sürekliliğinde %20'lik varyans tespit edildi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.`;
    setListe(liste.map((x) => (x.id === r.id ? { ...x, icerik: x.icerik + ozet } : x)));
  };

  const reddetVeGerekcelendir = (r: Rapor) => {
    const ozet = `

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.`;
    setListe(liste.map((x) => (x.id === r.id ? { ...x, icerik: x.icerik + ozet } : x)));
  };

  const disaAktar = (r: Rapor) => {
    if (r.taslak) return;
    const html = `<!doctype html><title>${r.baslik}</title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:16px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1>${TUR_ETIKET[r.tur] ?? r.tur} — ${r.baslik}</h1><div class=muhur>ONAYLI — ${r.onayKim ?? ''} ${r.onayTarih ?? ''}</div><pre>${r.icerik}</pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;|&nbsp; Kopya 2/2 — Kurum arşivi · ${new Date().toISOString().slice(0,10)} · Supporta v${typeof __SURUM__!=='undefined'?__SURUM__:'0.8.1'}</div><script>window.print()<\/script>`;
    const w = window.open('', '_blank'); if (w) { w.document.write(html); w.document.close(); }
    const csv = `tur,baslik,durum,icerik
${r.tur},"${r.baslik.replace(/"/g,'""')}",ONAYLI,"${r.icerik.replace(/"/g,'""')}"`;
    const blob = new Blob([csv], { type: 'text/csv;charset=utf-8;' });
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a'); a.href = url; a.download = `${r.id}-${r.tur}.csv`; a.click(); URL.revokeObjectURL(url);
  };
  
  return (
    <div className="space-y-4">
      {liste.map((r) => (
        <Kart key={r.id} baslik={`${TUR_ETIKET[r.tur] ?? r.tur} — ${r.baslik}`} ek={r.taslak ? <span data-testid="muhur-taslak" className="text-[11px] font-black tracking-wider text-amber-700 bg-amber-50 border border-amber-300 rounded-lg px-2 py-1">UZMAN ONAYI BEKLİYOR</span> : <span data-testid="muhur-onayli" className="inline-flex items-center gap-1 text-[11px] font-bold text-emerald-700 bg-emerald-50 border border-emerald-200 rounded-lg px-2 py-1"><CheckCircle2 className="w-3.5 h-3.5" /> UZMAN ONAYLI</span>}>
          <textarea 
            value={r.icerik} 
            onChange={(e) => setListe(liste.map(x => x.id === r.id ? {...x, icerik: e.target.value} : x))}
            disabled={!r.taslak}
            className="w-full h-40 p-3 text-sm text-slate-700 bg-slate-50 border border-slate-200 rounded-xl font-mono focus:ring-2 focus:ring-teal-500 outline-none"
          />
          
          <div className="flex flex-col gap-3 mt-3">
            {r.taslak && (
              <div className="bg-indigo-50 border border-indigo-100 p-3 rounded-xl space-y-3">
                <div className="flex items-center gap-2">
                  <Brain className="w-4 h-4 text-indigo-600" />
                  <span className="text-xs font-bold text-indigo-900">Human-Accountable AI (YZ Destek Asistanı)</span>
                </div>
                <div className="flex flex-wrap gap-2">
                  <button type="button" onClick={() => sistemOnerisi(r)} className="px-3 py-1.5 rounded-lg bg-white border border-indigo-200 text-indigo-700 hover:bg-indigo-100 text-xs font-semibold shadow-sm transition-colors">
                    Kanıtı İncele ve YZ Önerisi Al
                  </button>
                  <button type="button" onClick={() => reddetVeGerekcelendir(r)} className="px-3 py-1.5 rounded-lg bg-white border border-rose-200 text-rose-700 hover:bg-rose-50 text-xs font-semibold shadow-sm transition-colors">
                    Öneriyi Reddet ve Gerekçelendir
                  </button>
                </div>
                <p className="text-[10px] text-indigo-600 italic">YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.</p>
              </div>
            )}
            
            <div className="flex items-center gap-2 flex-wrap pt-2 border-t border-slate-100">
              {r.taslak && <button type="button" data-testid={`onayla-${r.id}`} onClick={() => onayla(r.id)} className="px-4 py-2 rounded-xl bg-teal-600 hover:bg-teal-700 text-white text-xs font-bold shadow-sm transition-colors">✓ Değişiklikleri Onayla ve İmzala</button>}
              <button type="button" data-testid={`disa-${r.id}`} disabled={r.taslak} onClick={()=>disaAktar(r)} className={`inline-flex items-center gap-1 px-4 py-2 rounded-xl text-xs font-bold shadow-sm transition-colors ${r.taslak ? 'bg-slate-100 text-slate-400 cursor-not-allowed border border-slate-200' : 'bg-slate-900 text-white hover:bg-black'}`}><Printer className="w-4 h-4" /> Dışa aktar (2 kopya)</button>
              {r.taslak && <span className="text-[11px] text-rose-600 font-semibold" data-testid="kc10">Onaysız rapor dışa aktarılamaz.</span>}
            </div>
          </div>
        </Kart>
      ))}
    </div>
  );
}

/* ---------- PROGRAM HİZALAMA (Y2-A / KC13) ---------- */
export function Hizalama() {
  const [modul, setModul] = useState<string>('M3');
  const m = DEP_MODULLER.find((x) => x.id === modul)!;
  const toplam = DEP_TOPLAM_SAAT;
  return (
    <Kart baslik="MEB destek eğitim programı modülleriyle hizalı çıktı">
      <div className="flex gap-2 flex-wrap">
        {DEP_MODULLER.map((x) => (
          <button key={x.id} data-testid={`dep-${x.id}`} onClick={() => setModul(x.id)}
            className={`px-3 py-1.5 rounded-xl text-xs border ${modul === x.id ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
            {x.id} · {x.ad} <b>({x.saat} sa)</b>
          </button>
        ))}
      </div>
      <p className="text-sm">Seçili: <b>{m.ad}</b> — {m.bolum} bölüm · önerilen <b>{m.saat} ders saati</b></p>
      <p data-testid="dep-toplam" className="text-[11px] text-slate-500">Toplam program: <b>{toplam} ders saati</b> · 6 modül · giriş yalnız ELLE yapılır.</p>
      <div data-testid="modul-serbest" className="rounded-xl bg-teal-50 border border-teal-200 px-3 py-2 text-[11px] text-teal-900">
        <b>Modül seçimi serbesttir.</b> {MODUL_TERIM_NOTU}
      </div>
      <p data-testid="ders-tavan" className="text-[11px] text-slate-500">
        Resmî tavan (ÖEK Yön. md.24/4): aylık <b>{DERS_TAVAN.aylikBireysel}</b> bireysel · <b>{DERS_TAVAN.aylikGrup}</b> grup ·
        haftalık <b>{DERS_TAVAN.haftalikBireysel}</b>/<b>{DERS_TAVAN.haftalikGrup}</b> · günlük toplam <b>{DERS_TAVAN.gunlukToplam}</b> saat.
      </p>
      <Sherh metin={SHERHLER.hizali} ton="uyari" />
    </Kart>
  );
}

/* ---------- AİLE & ÖĞRETMEN + AİLE EĞİTİM MERKEZİ (v0.8.4 A/B) ---------- */
export function Aile() {
  const [secAile, setSecAile] = useState(DOSYALAR[0].uid);
  return (
    <>
      <Kart baslik="Aile & Öğretmen İşbirliği">
        <p className="text-sm text-slate-700">Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.</p>
        <Sherh metin={SHERHLER.aile} ton="uyari" />
      </Kart>
      <Kart baslik="Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)" ek={<span className="text-[11px] text-slate-500">K-407 · 5+1 · TASLAK</span>}>
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} type="button" data-testid={`aile-dosya-${d.uid}`} onClick={() => setSecAile(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${secAile === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>{d.uid}</button>
          ))}
        </div>
        <AileEgitimMerkezi dosyaUid={secAile} />
      </Kart>
      <Kart baslik="Bilgilendirme çıktısı">
        <p className="text-sm text-slate-600">Yalnız <b>onaylı</b> raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).</p>
        <div className="rounded-xl bg-slate-50 border border-slate-200 p-3 text-xs font-mono" data-testid="sms-taslak">
          Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
        </div>
      </Kart>
    </>
  );
}

/* ---------- AYARLAR ---------- */
export function Ayarlar() {
  return (
    <Kart baslik="Şerh kütüphanesi ve roller">
      <ul className="text-sm space-y-2">
        {Object.entries(SHERHLER).map(([k, v]) => (
          <li key={k}><span className="text-xs font-bold text-slate-500 uppercase">{k}</span><Sherh metin={v} /></li>
        ))}
      </ul>
      <p className="text-[11px] text-slate-500">Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).</p>
      <div className="pt-3 border-t border-slate-100 space-y-2">
        <h3 className="font-bold text-sm">Kapsam dışı (bilinçli sınırlar)</h3>
        <ul data-testid="kapsam-disi" className="text-xs space-y-1.5">
          {KAPSAM_DISI.map((k) => (
            <li key={k.ad} className="rounded-xl bg-slate-50 border border-slate-200 px-3 py-2">
              <b>{k.ad}</b> — <span className="text-slate-600">{k.gerekce}</span>
            </li>
          ))}
        </ul>
      </div>
      <div className="pt-3 border-t border-slate-100 space-y-2">
        <h3 className="font-bold text-sm flex items-center gap-1.5"><Database className="w-4 h-4 text-slate-500" /> Yerel veri</h3>
        <p className="text-xs text-slate-600">
          Girdiler, oturum durumları ve rapor onayları <b>yalnız bu cihazda</b> saklanır (KVKK yerel-önce).
          Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: <b data-testid="kayit-sayisi">{kayitSayisi()}</b>
        </p>
        <button type="button" data-testid="veri-sil"
          onClick={() => { temizle(); location.reload(); }}
          className="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-xl bg-rose-50 text-rose-700 border border-rose-200 text-xs font-semibold hover:bg-rose-100">
          <Trash2 className="w-3.5 h-3.5" /> Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
        </button>
      </div>
    </Kart>
  );
}


/* ---------- RAM & BEP TAKİBİ (K-395) ---------- */
export function RamBep() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const r = RAM_KAYITLARI.find((x) => x.dosyaUid === sec)!;
  const pr = PROGRAMLAR.find((x) => x.dosyaUid === sec)!;
  const hat = KAYIT_HATTI.find((h) => h.id === pr.kayitHatti)!;
  return (
    <>
      <Kart baslik="RAM raporu ve kayıt hattı">
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} data-testid={`ram-dosya-${d.uid}`} onClick={() => setSec(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>{d.uid}</button>
          ))}
        </div>
        <div data-testid="kayit-hatti" className="rounded-xl bg-sky-50 border border-sky-200 px-3 py-2 text-xs text-sky-900">
          <b>Kayıt hattı: {hat.ad}</b><br />RAM raporu: <b>{hat.ram}</b> · Planlama: {hat.planlama}
        </div>
        <dl className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          {[['Rapor no', r.raporNo], ['Rapor tarihi', r.tarih], ['Geçerlilik', r.gecerlilik],
            ['EDİF durumu', r.edifDurumu], ['Sonraki izleme', r.sonrakiIzleme],
            ['Portfolyo', r.portfolyoHazir ? 'Hazır' : 'Hazır değil']].map(([k, v]) => (
            <div key={k as string}><dt className="text-slate-500 text-xs">{k}</dt><dd className="font-medium">{v}</dd></div>
          ))}
        </dl>
        <Sherh metin={SHERHLER.hizali} ton="uyari" />
      </Kart>
      <Kart baslik="Resmî form ailesi — hangi girdi neyi besler"
        ek={<span className="text-[11px] text-slate-500">DEP-2026 EK-1…EK-7</span>}>
        <table className="w-full text-sm" data-testid="resmi-formlar">
          <thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200">
            <th className="py-2 w-16">Ek</th><th>Form</th><th className="hidden sm:table-cell">Doldurma anı</th><th>Supporta katkısı</th></tr></thead>
          <tbody>
            {RESMI_FORMLAR.map((f) => (
              <tr key={f.ek} className="border-b border-slate-100 align-top">
                <td className="py-2 font-bold">{f.ek}</td>
                <td className="pr-2">{f.ad}</td>
                <td className="pr-2 text-slate-500 text-xs hidden sm:table-cell">{f.an}</td>
                <td className="text-xs text-slate-600">{f.besleyen}</td>
              </tr>
            ))}
          </tbody>
        </table>
        <div data-testid="form-sinir" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900">
          <b>Sınır:</b> Supporta bu formları <b>DOLDURMAZ</b>. x/+ işaretini, performans düzeyini ve
          “ulaşılamama nedenini” <b>uzman</b> belirler; portfolyo <b>RAM onayına</b> gider.
          Model: <b>Supporta kanıt üretir · uzman karar verir · RAM onaylar.</b>
        </div>
        <div className="rounded-xl border border-slate-300 bg-slate-50 px-3 py-2 text-[11px] font-semibold text-slate-700" data-testid="k1-serit">
          Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
        </div>
      </Kart>
    </>
  );
}

/* ---------- EV ÖDEVLERİ / SEANS DIŞI (K-395) ---------- */
export function EvOdevleri() {
  const [liste, setListe] = useKalici<EvOdevi[]>('evodev', EV_ODEVLERI);
  const durumDegis = (id: string, d: EvOdevi['durum']) =>
    setListe(liste.map((o) => (o.id === id ? { ...o, durum: d } : o)));
  return (
    <>
      <Kart baslik="Ev çalışmaları ve seans dışı görevler"
        ek={<span className="text-[11px] text-slate-500">kim · ne · ne zaman</span>}>
        <ul className="space-y-2">
          {liste.map((o) => (
            <li key={o.id} data-testid="evodev-satir" className="rounded-xl border border-slate-200 px-3 py-2">
              <div className="flex items-start justify-between gap-3">
                <div>
                  <div className="font-semibold text-sm">{o.baslik}</div>
                  <div className="text-xs text-slate-500">{o.dosyaUid} · {o.kim} · {o.neZaman}</div>
                  {o.not && <div className="text-xs text-slate-600 mt-1">Not: {o.not}</div>}
                </div>
                <select data-testid={`evodev-durum-${o.id}`} value={o.durum}
                  onChange={(e) => durumDegis(o.id, e.target.value as EvOdevi['durum'])}
                  className={`text-[11px] font-bold rounded-full px-2 py-1 border shrink-0 ${
                    o.durum === 'yapıldı' ? 'bg-emerald-50 text-emerald-700 border-emerald-200' :
                    o.durum === 'yapılmadı' ? 'bg-rose-50 text-rose-700 border-rose-200' :
                    'bg-sky-50 text-sky-700 border-sky-200'}`}>
                  <option value="verildi">verildi</option><option value="yapıldı">yapıldı</option><option value="yapılmadı">yapılmadı</option>
                </select>
              </div>
            </li>
          ))}
        </ul>
        <Sherh metin="Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz." />
      </Kart>
      <Kart baslik="Seans başı izleme ritüeli">
        <ol className="text-sm space-y-1 list-decimal list-inside text-slate-700">
          <li>Ev çalışması gözden geçirilir (yapıldı/yapılmadı — <b>yargı değil gözlem</b>).</li>
          <li>Bir önceki oturumun hedef davranışı hatırlatılır.</li>
          <li>Bugünün etkinliği ve ipucu kademesi belirlenir.</li>
          <li>Oturum sonunda veli için tek satırlık jargonsuz not yazılır.</li>
        </ol>
        <Sherh metin={SHERHLER.aile} />
      </Kart>
    </>
  );
}


/* ---------- M4: ETKİNLİK & HEDEF KATALOĞU (K-396) — düzenlenebilir (v0.8.1) + BGM ayrı filtre (v0.8.3 K-403 kuyruğu E2) ---------- */
export function EtkinlikKatalogu() {
  const [katman, setKatman] = useState<'hepsi' | 'DEP' | 'BGM'>('hepsi');
  const [modul, setModul] = useState<string>('hepsi');
  const [katalog, setKatalog] = useKalici<import('../data/tipler').Etkinlik[]>('etkinlikler', ETKINLIKLER);
  const [duzenId, setDuzenId] = useState<string | null>(null);
  const [form, setForm] = useState<{ ad: string; hedefKod: string; modulAdi: string; ipucuKademesi: string; malzeme: string; katman: 'DEP' | 'BGM' }>({ ad: '', hedefKod: '', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi: '', malzeme: '', katman: 'DEP' });
  const katmanFiltreli = katman === 'hepsi' ? katalog : katalog.filter((e) => (e.katman ?? 'DEP') === katman);
  const liste = modul === 'hepsi' ? katmanFiltreli : katmanFiltreli.filter((e) => e.modulAdi === modul);
  const moduller = katman === 'BGM' ? ['hepsi', 'BGM-12'] : ['hepsi', ...DEP_MODULLER.map((m) => m.ad)];
  const kaydet = () => {
    if (!form.ad.trim() || !form.hedefKod.trim()) return;
    const yeni: import('../data/tipler').Etkinlik = { id: duzenId ?? `ET-${Date.now()}`, ad: form.ad.trim(), hedefKod: form.hedefKod.trim(), modulAdi: form.katman==='BGM' ? 'BGM-12' : form.modulAdi, ipucuKademesi: form.ipucuKademesi.trim() || 'Model → bağımsız', malzeme: form.malzeme.split(',').map((s)=>s.trim()).filter(Boolean), katman: form.katman };
    if (duzenId) setKatalog(katalog.map((e)=> e.id===duzenId ? yeni : e));
    else setKatalog([...katalog, yeni]);
    setDuzenId(null); setForm({ ad: '', hedefKod: '', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi: '', malzeme: '', katman: 'DEP' });
  };
  const duzenle = (id: string) => { const e = katalog.find((x)=>x.id===id)!; setDuzenId(id); setForm({ ad: e.ad, hedefKod: e.hedefKod, modulAdi: e.modulAdi, ipucuKademesi: e.ipucuKademesi, malzeme: e.malzeme.join(', '), katman: (e.katman ?? 'DEP') as 'DEP'|'BGM' }); };
  const sil = (id: string) => setKatalog(katalog.filter((e)=>e.id!==id));
  return (
    <>
      <Kart baslik="Etkinlik ve hedef davranış kataloğu" ek={<span className="text-[11px] text-slate-500">{liste.length} / {katalog.length} etkinlik · DEP {katalog.filter(e=>(e.katman??'DEP')==='DEP').length} · BGM {katalog.filter(e=>e.katman==='BGM').length}</span>}>
        <div className="flex gap-1.5 flex-wrap">
          {(['hepsi','DEP','BGM'] as const).map((k)=> (
            <button key={k} data-testid={`katman-${k}`} onClick={()=>{setKatman(k); setModul('hepsi');}}
              className={`px-3 py-1 rounded-full text-[11px] font-bold border ${katman===k?'bg-slate-900 text-white border-slate-900':'bg-white border-slate-200'}`}>
              {k==='hepsi'?`Tümü (${katalog.length})`:k==='DEP'?`DEP-2026 (${katalog.filter(e=>(e.katman??'DEP')==='DEP').length})`:`BGM-12 (${katalog.filter(e=>e.katman==='BGM').length})`}
            </button>
          ))}
        </div>
        <div className="flex gap-1.5 flex-wrap">
          {moduller.map((m) => (
            <button key={m} data-testid={`kat-filtre-${m === 'hepsi' ? 'hepsi' : m.split(' ')[0]}`}
              onClick={() => setModul(m)}
              className={`px-2.5 py-1 rounded-lg text-[11px] border ${modul === m ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {m === 'hepsi' ? 'Tümü' : m}
            </button>
          ))}
        </div>
        <div className="rounded-2xl border border-slate-200 bg-slate-50 p-3 space-y-2">
          <div className="text-xs font-bold text-slate-700">{duzenId ? 'Etkinliği düzenle' : 'Yeni etkinlik ekle'} <span className="font-normal text-slate-500">· kayıt bu cihazda saklanır</span></div>
          <div className="grid sm:grid-cols-2 gap-2">
            <select data-testid="etk-katman" value={form.katman} onChange={(e)=>setForm({...form, katman:e.target.value as 'DEP'|'BGM', modulAdi: e.target.value==='BGM' ? 'BGM-12' : DEP_MODULLER[0].ad})} className="rounded-xl border border-slate-300 px-3 py-2 text-sm">
              <option value="DEP">DEP-2026</option><option value="BGM">BGM-12</option>
            </select>
            <input data-testid="etk-ad" value={form.ad} onChange={(e)=>setForm({...form, ad:e.target.value})} placeholder="Etkinlik adı *" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            <input data-testid="etk-kod" value={form.hedefKod} onChange={(e)=>setForm({...form, hedefKod:e.target.value})} placeholder="Hedef kod (örn 3.1.2 / BGM-FS-1) *" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            {form.katman==='DEP' && <select data-testid="etk-modul" value={form.modulAdi} onChange={(e)=>setForm({...form, modulAdi:e.target.value})} className="rounded-xl border border-slate-300 px-3 py-2 text-sm">{DEP_MODULLER.map((m)=><option key={m.id} value={m.ad}>{m.id} · {m.ad}</option>)}</select>}
            <input data-testid="etk-ipucu" value={form.ipucuKademesi} onChange={(e)=>setForm({...form, ipucuKademesi:e.target.value})} placeholder="İpucu kademesi (örn Model→bağımsız)" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            <input data-testid="etk-malzeme" value={form.malzeme} onChange={(e)=>setForm({...form, malzeme:e.target.value})} placeholder="Malzeme (virgülle ayır)" className="sm:col-span-2 rounded-xl border border-slate-300 px-3 py-2 text-sm" />
          </div>
          <div className="flex gap-2">
            <button type="button" data-testid="etk-kaydet" onClick={kaydet} disabled={!form.ad.trim()||!form.hedefKod.trim()} className={`px-3 py-1.5 rounded-xl text-xs font-semibold ${!form.ad.trim()||!form.hedefKod.trim() ? 'bg-slate-200 text-slate-400 cursor-not-allowed' : 'bg-teal-600 text-white hover:bg-teal-700'}`}>{duzenId ? 'Güncelle' : 'Ekle'}</button>
            {duzenId && <button type="button" data-testid="etk-iptal" onClick={()=>{setDuzenId(null); setForm({ ad:'', hedefKod:'', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi:'', malzeme:'', katman:'DEP'});}} className="px-3 py-1.5 rounded-xl text-xs border border-slate-300 bg-white">İptal</button>}
            <button type="button" data-testid="etk-sifirla" onClick={()=>{ setKatalog(ETKINLIKLER); setDuzenId(null); }} className="ml-auto text-[11px] text-slate-500 underline">Varsayılana sıfırla</button>
          </div>
        </div>
        <div className="grid sm:grid-cols-2 gap-3">
          {liste.map((e) => (
            <div key={e.id} data-testid="etkinlik-karti" className="rounded-xl border border-slate-200 p-3 space-y-1.5 bg-white">
              <div className="flex items-start justify-between gap-2">
                <span className="font-semibold text-sm">{e.ad} {(e.katman==='BGM') && <span className="ml-1 text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5">BGM</span>}</span>
                <span className={`text-[10px] font-bold border rounded-full px-2 py-0.5 shrink-0 ${e.katman==='BGM'?'bg-sky-50 text-sky-700 border-sky-200':'bg-teal-50 text-teal-700 border-teal-200'}`}>{e.hedefKod}</span>
              </div>
              <div className="text-[11px] text-slate-500">{e.modulAdi} · <span className={`text-[10px] font-bold px-1.5 py-0.5 rounded-full border ${e.katman==='BGM'?'bg-sky-50 text-sky-700 border-sky-200':'bg-emerald-50 text-emerald-700 border-emerald-200'}`}>{e.katman ?? 'DEP'}</span></div>
              <div className="text-xs"><b>İpucu kademesi:</b> {e.ipucuKademesi}</div>
              <div className="text-xs text-slate-600"><b>Malzeme:</b> {e.malzeme.join(' · ')}</div>
              <div className="flex gap-1.5 pt-1">
                <button type="button" data-testid={`etk-duzenle-${e.id}`} onClick={()=>duzenle(e.id)} className="text-[11px] px-2 py-1 rounded-lg border border-slate-200 bg-white">Düzenle</button>
                <button type="button" data-testid={`etk-sil-${e.id}`} onClick={()=>sil(e.id)} className="text-[11px] px-2 py-1 rounded-lg border border-rose-200 bg-rose-50 text-rose-700">Sil</button>
              </div>
            </div>
          ))}
        </div>
        <div data-testid="katalog-sinir" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900"><b>Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR</b> — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.</div>
      </Kart>
    </>
  );
}

/* ---------- BGM-12 MENÜ (K-398) — sıra uzmanında, atlanabilir ---------- */
export function BgmMenu() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const [secim, setSecim] = useKalici<Record<string, string[]>>('bgm-secim', {
    'ÖĞR-4417': ['FS-1', 'II-6', 'CA-4'],
    'ÖĞR-2903': [],
  });
  const [acik, setAcik] = useState<string | null>('FS-1');
  const siradaki = secim[sec] ?? [];
  const al = (id: string) => {
    if (siradaki.includes(id)) return;
    setSecim({ ...secim, [sec]: [...siradaki, id] });
  };
  const cikar = (id: string) => setSecim({ ...secim, [sec]: siradaki.filter((x) => x !== id) });
  const fazlar: BgmFaz[] = ['I', 'II', 'III'];
  return (
    <>
      <Kart baslik="Bilişsel Geliştirme Modülleri (BGM-12)"
        ek={<span className="text-[11px] text-slate-500">{BGM_SAYI} modül · menü</span>}>
        <div data-testid="bgm-katman" className="rounded-xl bg-sky-50 border border-sky-200 px-3 py-2 text-[11px] text-sky-900">
          <b>İki katman.</b> {BGM_KATMAN_NOTU}
        </div>
        <div data-testid="bgm-serbest" className="rounded-xl bg-teal-50 border border-teal-200 px-3 py-2 text-[11px] text-teal-900">
          <b>Modül seçimi serbesttir.</b> {MODUL_TERIM_NOTU} Persona sarmalı dayatılmaz.
        </div>
        <div data-testid="bgm-taslak" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900">
          <b>TASLAK.</b> {BGM_TASLAK_NOTU} Tam kartlar: <code>SEDUVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md</code>.
        </div>
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} type="button" data-testid={`bgm-dosya-${d.uid}`} onClick={() => setSec(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {d.uid}
            </button>
          ))}
        </div>
        <p className="text-xs text-slate-600">
          Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil):{' '}
          <b data-testid="bgm-secili-liste">{siradaki.length ? siradaki.join(' → ') : 'henüz seçilmedi — 1-2-3 atlanabilir'}</b>
        </p>
      </Kart>
      {fazlar.map((f) => (
        <Kart key={f} baslik={BGM_FAZ_ETIKET[f]}>
          <div className="grid sm:grid-cols-2 gap-3">
            {BGM_MODULLER.filter((m) => m.faz === f).map((m) => {
              const secili = siradaki.includes(m.id);
              const ac = acik === m.id;
              return (
                <div key={m.id} data-testid={`bgm-kart-${m.id}`}
                  className={`rounded-xl border p-3 space-y-2 ${secili ? 'border-teal-400 bg-teal-50/40' : 'border-slate-200'}`}>
                  <div className="flex items-start justify-between gap-2">
                    <button type="button" className="text-left" onClick={() => setAcik(ac ? null : m.id)}>
                      <div className="font-semibold text-sm">{m.id} · {m.ad}</div>
                      <div className="text-[11px] text-slate-500">{m.kisa} · {m.dehbAlan}</div>
                    </button>
                    {m.oncelikli && <span className="text-[10px] font-bold bg-amber-50 text-amber-800 border border-amber-200 rounded-full px-2 py-0.5 shrink-0">çekirdek</span>}
                  </div>
                  <div className="flex gap-1.5">
                    {secili
                      ? <button type="button" data-testid={`bgm-cikar-${m.id}`} onClick={() => cikar(m.id)}
                          className="text-[11px] font-semibold px-2 py-1 rounded-lg bg-white border border-slate-300">Programdan çıkar</button>
                      : <button type="button" data-testid={`bgm-al-${m.id}`} onClick={() => al(m.id)}
                          className="text-[11px] font-semibold px-2 py-1 rounded-lg bg-teal-600 text-white">Programa al</button>}
                    <button type="button" data-testid={`bgm-ac-${m.id}`} onClick={() => setAcik(ac ? null : m.id)}
                      className="text-[11px] px-2 py-1 rounded-lg border border-slate-200">Kart</button>
                  </div>
                  {ac && (
                    <dl data-testid={`bgm-yuva-${m.id}`} className="text-[11px] space-y-1 text-slate-700 border-t border-slate-200 pt-2">
                      <div><b>Tanım:</b> {m.tanim}</div>
                      <div><b>Amaç:</b> {m.amac}</div>
                      <div><b>Ölçüm:</b> {m.olcum}</div>
                      <div><b>Etkinlik:</b> {m.etkinlik} <span className="text-slate-500">({m.sureDk})</span></div>
                      <div><b>Malzeme:</b> {m.malzeme.join(' · ')} · <b>İpucu:</b> {m.ipucu} · <b>Girdi:</b> {KODLAMA[m.girdiTipi].ad}</div>
                      <div><b>Ödev:</b> {m.odev}</div>
                      <div><b>Önlem:</b> {m.onlem}</div>
                      <div><b>Öneri:</b> {m.oneri}</div>
                      <div><b>DEP köprüsü:</b> {m.depKoprusu ? `${m.depKoprusu} — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)` : 'yok (bütünleştirme turu)'}</div>
                      <div className="text-slate-500"><b>Dayanak:</b> {m.dayanak}</div>
                    </dl>
                  )}
                </div>
              );
            })}
          </div>
        </Kart>
      ))}
      <Sherh metin={SHERHLER.k02} ton="uyari" />
    </>
  );
}


~~~~

### `components/Kabuk.tsx`
3094 B ·SHA `57018b5336d0c73538a0a4461ed84c026596cccc24e399da8c9cfb40213389b1`

~~~~tsx
/** Uygulama kabuğu: sol menü + üst bant. Veli rolü YOKTUR (K-296/KC7). */
import type { ReactNode } from 'react';
import { FolderOpen, CalendarDays, ClipboardList, BarChart3, FileText, Users, Settings, LayoutDashboard, BookOpen, FileCheck2, Home, Library, Brain } from 'lucide-react';
import { SHERHLER } from '../data/kisitlar';

export const EKRANLAR = [
  { id: 'pano', ad: 'Eğitmen Kürsüsü', ikon: LayoutDashboard },
  { id: 'dosyalar', ad: 'Dosyalar', ikon: FolderOpen },
  { id: 'takvim', ad: 'Takvim', ikon: CalendarDays },
  { id: 'oturum', ad: 'Oturum Atölyesi', ikon: ClipboardList },
  { id: 'katalog', ad: 'Etkinlik Kataloğu', ikon: Library },
  { id: 'cizelge', ad: 'İzleme Çizelgesi', ikon: BarChart3 },
  { id: 'rapor', ad: 'Rapor Atölyesi', ikon: FileText },
  { id: 'hizalama', ad: 'Program Hizalama', ikon: BookOpen },
  { id: 'bgm', ad: 'Bilişsel Geliştirme', ikon: Brain },
  { id: 'rambep', ad: 'RAM & BEP Takibi', ikon: FileCheck2 },
  { id: 'evodev', ad: 'Ev Çalışmaları', ikon: Home },
  { id: 'aile', ad: 'Aile & Öğretmen', ikon: Users },
  { id: 'ayarlar', ad: 'Ayarlar', ikon: Settings },
] as const;
export type EkranId = (typeof EKRANLAR)[number]['id'];

export default function Kabuk({ ekran, setEkran, rol, children }:
  { ekran: EkranId; setEkran: (e: EkranId) => void; rol: string; children: ReactNode }) {
  return (
    <div className="min-h-screen flex">
      <aside className="w-60 bg-white border-r border-slate-200 flex flex-col shrink-0">
        <div className="px-4 py-4 border-b border-slate-100">
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 rounded-xl bg-teal-600 text-white grid place-items-center font-black">S</div>
            <div>
              <div className="font-bold text-sm">SEDUVA Supporta™</div>
              <div className="text-[10px] text-slate-500">Uzman Kokpiti · v{__SURUM__}</div>
            </div>
          </div>
        </div>
        <nav className="flex-1 p-2 space-y-0.5">
          {EKRANLAR.map((e) => {
            const I = e.ikon; const akt = ekran === e.id;
            return (
              <button key={e.id} type="button" data-testid={`nav-${e.id}`} onClick={() => setEkran(e.id)}
                className={`w-full flex items-center gap-2 px-3 py-2 rounded-xl text-sm transition-colors ${
                  akt ? 'bg-teal-600 text-white font-semibold' : 'text-slate-700 hover:bg-slate-100'}`}>
                <I className="w-4 h-4" /> {e.ad}
              </button>
            );
          })}
        </nav>
        <div className="p-3 border-t border-slate-100 text-[10px] text-slate-500">
          Rol: <b>{rol}</b> · Sentetik demo verisi
        </div>
      </aside>
      <main className="flex-1 min-w-0">
        <div className="bg-white border-b border-slate-200 px-6 py-2">
          <Sherhli />
        </div>
        <div className="p-6 space-y-5 max-w-6xl">{children}</div>
      </main>
    </div>
  );
}
function Sherhli() {
  return <p className="text-[11px] text-slate-600"><b>SEDUVA Supporta:</b> {SHERHLER.k02}</p>;
}

~~~~

### `components/Sherh.tsx`
628 B ·SHA `0270e18645a0065ba9acb123afda1e9936ab96b44e7bc1cf5cd262c0f93f391a`

~~~~tsx
/** Silinemez şerh bloğu (spec §7 · KC3: kullanıcı kapatamaz). */
import { ShieldAlert } from 'lucide-react';
export default function Sherh({ metin, ton = 'nötr' }: { metin: string; ton?: 'nötr' | 'uyari' }) {
  const s = ton === 'uyari'
    ? 'bg-amber-50 border-amber-300 text-amber-900'
    : 'bg-slate-50 border-slate-200 text-slate-600';
  return (
    <div data-testid="sherh" data-silinemez="true"
         className={`flex items-start gap-2 rounded-xl border px-3 py-2 text-[11px] leading-relaxed ${s}`}>
      <ShieldAlert className="w-3.5 h-3.5 shrink-0 mt-0.5" />
      <span>{metin}</span>
    </div>
  );
}

~~~~

### `components/aile/AileEgitimMerkezi.tsx`
6806 B ·SHA `bf6e90d5ee035a78f9a2a6a0c858c26e115ca301f29f02b4ea7074ca799a0699`

~~~~tsx
import { useState } from 'react';
import { AILE_GENEL_5 } from '../../data/aile/genel';
import { AILE_KISISEL_SABLON, AILE_KISISEL_HAVUZ } from '../../data/aile/kisisel';
import { SHERHLER } from '../../data/kisitlar';

export default function AileEgitimMerkezi({ dosyaUid }: { dosyaUid: string }) {
  const [sekme, setSekme] = useState<'A' | 'B'>('A');
  const [secili, setSecili] = useState<string>('AG-1');
  const [kopya, setKopya] = useState<string>('');

  const aktif = AILE_GENEL_5.find((x) => x.id === secili) ?? AILE_GENEL_5[0];

  const yazdir = (baslik: string, icerik: string) => {
    const html = `<!doctype html><title>${baslik}</title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px;border:1px solid #e2e8f0;padding:12px;border-radius:10px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:12px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1>${baslik} — ${dosyaUid}</h1><div class=muhur>ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER</div><pre>${icerik}</pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;|&nbsp; Kopya 2/2 — Kurum arşivi · ${new Date().toISOString().slice(0,10)} · Supporta v${typeof __SURUM__ !== 'undefined' ? __SURUM__ : '0.8.4'} · ${SHERHLER.aile}</div><script>window.print()<\/script>`;
    const w = window.open('', '_blank');
    if (w) { w.document.write(html); w.document.close(); }
  };

  return (
    <div className="space-y-4">
      <div className="flex gap-2">
        <button
          type="button"
          data-testid="aile-sekme-A"
          onClick={() => setSekme('A')}
          className={`px-3 py-1.5 rounded-xl text-sm ${sekme === 'A' ? 'bg-teal-600 text-white' : 'bg-slate-100'}`}
        >
          A — Genel (5 mini-modül)
        </button>
        <button
          type="button"
          data-testid="aile-sekme-B"
          onClick={() => setSekme('B')}
          className={`px-3 py-1.5 rounded-xl text-sm ${sekme === 'B' ? 'bg-teal-600 text-white' : 'bg-slate-100'}`}
        >
          B — Analize Göre (uzman seçer)
        </button>
      </div>

      {sekme === 'A' ? (
        <div className="grid md:grid-cols-3 gap-4">
          <div className="space-y-2">
            {AILE_GENEL_5.map((k) => (
              <button
                key={k.id}
                type="button"
                data-testid={`aile-genel-${k.id}`}
                onClick={() => setSecili(k.id)}
                className={`w-full text-left p-3 rounded-xl border text-sm ${secili === k.id ? 'border-teal-600 bg-teal-50' : 'border-slate-200 bg-white'}`}
              >
                <div className="font-semibold">{k.baslik}</div>
                <div className="text-xs text-slate-500">{k.sureDk} dk · {k.amac.slice(0, 60)}…</div>
              </button>
            ))}
          </div>
          <div className="md:col-span-2 bg-white border border-slate-200 rounded-xl p-4 space-y-3">
            <div className="font-bold">{aktif.baslik}</div>
            <div className="text-sm text-slate-600">{aktif.amac}</div>
            <ul className="list-disc pl-5 text-sm space-y-1">
              {aktif.icerik.map((m, i) => (
                <li key={i}>{m}</li>
              ))}
            </ul>
            {aktif.malzeme.length > 0 && <div className="text-xs text-slate-500">Malzeme: {aktif.malzeme.join(', ')}</div>}
            {aktif.uyari && <div className="text-xs text-amber-700 bg-amber-50 border border-amber-200 rounded-lg p-2">{aktif.uyari}</div>}
            <div className="flex gap-2">
              <button
                type="button"
                data-testid="aile-yazdir-A"
                onClick={() => yazdir(aktif.baslik, `${aktif.amac}\n\n${aktif.icerik.join('\n- ')}\n\nMalzeme: ${aktif.malzeme.join(', ') || '—'}\n${aktif.uyari ?? ''}`)}
                className="px-3 py-1.5 rounded-xl bg-teal-600 text-white text-sm"
              >
                Yazdır / PDF
              </button>
              <button
                type="button"
                data-testid="aile-kopyala-A"
                onClick={() => {
                  const t = `${aktif.baslik}\n${aktif.amac}\n${aktif.icerik.join('\n')}`;
                  navigator.clipboard?.writeText(t);
                  setKopya('Kopyalandı');
                  setTimeout(() => setKopya(''), 1500);
                }}
                className="px-3 py-1.5 rounded-xl bg-slate-100 text-sm"
              >
                Kopyala
              </button>
              {kopya && <span className="text-xs text-teal-700 py-1.5">{kopya}</span>}
            </div>
            <p className="text-[11px] text-slate-500">{SHERHLER.aile} · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.</p>
          </div>
        </div>
      ) : (
        <div className="bg-white border border-slate-200 rounded-xl p-4 space-y-3">
          <div className="font-bold">{AILE_KISISEL_SABLON.baslik}</div>
          <div className="text-sm text-slate-600">{AILE_KISISEL_SABLON.baglam}</div>
          <div className="text-xs text-slate-500">Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02).</div>
          <div className="grid md:grid-cols-3 gap-2">
            {AILE_KISISEL_HAVUZ.map((h) => (
              <div key={h.id} className="p-3 rounded-xl border border-slate-200 bg-slate-50">
                <div className="font-semibold text-sm">{h.baslik}</div>
                <div className="text-xs text-slate-500">Tetik: {h.tetik}</div>
              </div>
            ))}
          </div>
          <pre className="text-xs bg-slate-50 border border-slate-200 rounded-xl p-3 whitespace-pre-wrap">{AILE_KISISEL_SABLON.uzmanNotuSablonu}</pre>
          <div className="text-sm">
            <span className="font-semibold">Aileye görev örneği:</span> {AILE_KISISEL_SABLON.aileyeGorev}
          </div>
          <div className="text-xs text-slate-500">Ölçüm: {AILE_KISISEL_SABLON.olcum}</div>
          <div className="flex gap-2">
            <button
              type="button"
              data-testid="aile-yazdir-B"
              onClick={() => yazdir(AILE_KISISEL_SABLON.baslik, `${AILE_KISISEL_SABLON.uzmanNotuSablonu}\n\nGörev: ${AILE_KISISEL_SABLON.aileyeGorev}\nÖlçüm: ${AILE_KISISEL_SABLON.olcum}`)}
              className="px-3 py-1.5 rounded-xl bg-teal-600 text-white text-sm"
            >
              Şablonu Yazdır
            </button>
          </div>
          <p className="text-[11px] text-slate-500">{SHERHLER.aile} · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir.</p>
        </div>
      )}
    </div>
  );
}

~~~~

### `components/egitmen/EgitmenDestekPaneli.tsx`
5441 B ·SHA `d3c595bdae6baab3ab8fe291d91ec1fcb11985876591c5567067d11cfa5b7b06`

~~~~tsx
// K-651: SUPPORTA (Merkez) - Eğitmen Destek Paneli
// Dalga 2 Eğitsel Zeka: Support Fading (Desteği Geri Çekme) ve Recovery (Mola Sonrası Toparlanma)

import { useState } from 'react';

interface OgrenciProfil {
  id: string;
  ad: string;
  aktifDestek: string;
  basariSerisi: number; // Support Fading tetikleyicisi
  enIyiToparlanma: string; // Recovery profil verisi
}

const MOCK_OGRENCILER: OgrenciProfil[] = [
  { id: '1', ad: 'Can B.', aktifDestek: 'Görsel İpucu', basariSerisi: 4, enIyiToparlanma: 'Düşük Uyaranlı Görev' },
  { id: '2', ad: 'Ali Y.', aktifDestek: 'Görev Parçalama', basariSerisi: 1, enIyiToparlanma: 'Sözel Yönerge' },
  { id: '3', ad: 'Elif S.', aktifDestek: 'Zamanlayıcı', basariSerisi: 5, enIyiToparlanma: 'Hareketli Mola' },
];

export default function EgitmenDestekPaneli() {
  const [secili, setSecili] = useState<OgrenciProfil>(MOCK_OGRENCILER[0]);

  // Kural: 3 ve üzeri başarılı görevde destek azaltma önerilir
  const isFadingReady = secili.basariSerisi >= 3;

  return (
    <div className="p-6 bg-slate-50 min-h-screen">
      <h1 className="text-2xl font-bold text-slate-800 border-b border-slate-300 pb-3 mb-6">
        Eğitmen Destek Paneli (Supporta)
      </h1>

      <div className="flex gap-6">
        {/* Sol Menü: Öğrenci Seçimi */}
        <div className="w-1/3 bg-white p-4 rounded-xl shadow-sm border border-slate-200">
          <h2 className="text-sm font-semibold text-slate-500 mb-4 uppercase tracking-wider">Öğrenci Listesi</h2>
          <div className="flex flex-col gap-2">
            {MOCK_OGRENCILER.map((ogr) => (
              <button
                key={ogr.id}
                onClick={() => setSecili(ogr)}
                className={`p-3 text-left rounded-lg transition-all ${
                  secili.id === ogr.id 
                    ? 'bg-blue-600 text-white shadow-md' 
                    : 'bg-slate-100 text-slate-700 hover:bg-slate-200'
                }`}
              >
                {ogr.ad}
                {ogr.basariSerisi >= 3 && <span className="ml-2 text-yellow-300">💡</span>}
              </button>
            ))}
          </div>
        </div>

        {/* Sağ Panel: Profil ve İçgörüler */}
        <div className="w-2/3 flex flex-col gap-4">
          
          {/* Support Fading Modülü */}
          <div className="bg-white p-5 rounded-xl shadow-sm border border-slate-200">
            <h3 className="text-lg font-bold text-slate-800 mb-1">Destek Profili</h3>
            <p className="text-sm text-slate-500 mb-4">Şu an uygulanan destek stratejisi ve performansı.</p>
            
            <div className="p-4 bg-blue-50 border border-blue-100 rounded-lg">
              <div className="flex justify-between items-center">
                <div>
                  <p className="text-sm text-blue-600 font-medium">Aktif Destek (Müdahale)</p>
                  <p className="text-xl font-bold text-blue-900">{secili.aktifDestek}</p>
                </div>
                <div className="text-right">
                  <p className="text-sm text-blue-600 font-medium">İstikrarlı Başarı Serisi</p>
                  <p className="text-xl font-bold text-blue-900">{secili.basariSerisi} Görev</p>
                </div>
              </div>
            </div>

            {isFadingReady && (
              <div className="mt-4 p-4 bg-emerald-50 border border-emerald-200 rounded-lg flex items-start gap-3">
                <div className="text-2xl">💡</div>
                <div>
                  <h4 className="font-bold text-emerald-900">Desteği Geri Çekme Önerisi (Support Fading)</h4>
                  <p className="text-sm text-emerald-800 mt-1">
                    Bu öğrenci <b>{secili.aktifDestek}</b> stratejisinde uzmanlaştı. Bağımsızlığı artırmak adına, 
                    sonraki seansta desteği bir alt seviyeye indirmeyi (Fading) deneyebilirsiniz.
                  </p>
                  <button className="mt-3 px-4 py-2 bg-emerald-600 hover:bg-emerald-700 text-white text-sm font-semibold rounded-md transition-colors">
                    Desteği Azalt / Kaldır
                  </button>
                </div>
              </div>
            )}
          </div>

          {/* Recovery Profile Modülü */}
          <div className="bg-white p-5 rounded-xl shadow-sm border border-slate-200">
            <h3 className="text-lg font-bold text-slate-800 mb-1">Toparlanma (Recovery) Zekası</h3>
            <p className="text-sm text-slate-500 mb-4">Öğrencinin moladan veya kriz anından sonra en hızlı toparlandığı koşullar.</p>
            
            <div className="p-4 bg-purple-50 border border-purple-100 rounded-lg flex items-center justify-between">
              <div>
                <p className="text-sm text-purple-600 font-medium">En Verimli Dönüş (Transition) Aracı:</p>
                <p className="text-lg font-bold text-purple-900">{secili.enIyiToparlanma}</p>
              </div>
              <div className="text-purple-300 text-4xl">⏱️</div>
            </div>
            <p className="text-xs text-purple-700 mt-2">
              Öneri: Mola dönüşlerinde yüksek uyaranlı veya zor görevlerden kaçının. Başlangıçta <b>{secili.enIyiToparlanma}</b> vererek bilişsel geçişi (transition) kolaylaştırın.
            </p>
          </div>

        </div>
      </div>
    </div>
  );
}

~~~~

### `data/aile/genel.ts`
3424 B ·SHA `31b5111e95e85c281a63796c15e5edd66a31a6fa41e745064153b0263f87bc3d`

~~~~tsx
/** A — Genel Davranış-Tutum Bilgilendirme (5 mini-modül, her aileye aynı — önleyici)
 *  Kaynak kavramı: MEB DEHB Aile Rehberi Tablo 11/12 + §7 + Z-7 — cümle kopyalanmadan, kavram düzeyinde özet.
 *  K-08 pedagog onayı 04.09 kullanıcı, K-02 dili, K-14 gözlemlenebilir dil, K-15 dijital puan YOK.
 *  TASLAK — şirket sonrası Turnitin + hukuk tek pakette.
 */
export interface AileGenelKart {
  id: string;
  baslik: string;
  amac: string;
  icerik: string[]; // 3-4 madde, kavram özetleri
  sureDk: number;
  malzeme: string[];
  uyari?: string;
}

export const AILE_GENEL_5: AileGenelKart[] = [
  {
    id: 'AG-1',
    baslik: 'Nasihat ve Kıyas Yok — Gözlem Dili',
    amac: 'Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.',
    icerik: [
      '“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.',
      '“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).',
      'Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).',
    ],
    sureDk: 15,
    malzeme: ['A4 gözlem kartı', 'kalem'],
    uyari: 'Yorum/değer yargısı yok — yalnızca gözlem.',
  },
  {
    id: 'AG-2',
    baslik: 'Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne',
    amac: 'Yazılı planla öngörülebilirlik sağlamak (Z-1).',
    icerik: [
      'Akşam rutinini 5 soruyla duvara asın: ne yapılacak · ne zaman · nerede · ne kadar · sonra ne var (Tablo 9/10 kavramı).',
      'Resimli/renkli kartta her adım tek satır, tik kutusu ekleyin.',
      'Planı çocukla birlikte hazırlayın, her gün aynı yerde tutun.',
    ],
    sureDk: 20,
    malzeme: ['rutin şablonu (A4)', 'renkli kalem'],
  },
  {
    id: 'AG-3',
    baslik: 'Görsel Ortam — Uyaran Yalıtımı',
    amac: 'Çalışma yüzeyinde dikkat çeldiriciyi azaltmak (Tablo 12 + Z-7 görsel).',
    icerik: [
      'Masada yalnızca o derste gerekli materyal kalsın, fazlası kutuya.',
      'Dersten önce yüzey toplama ritüeli: 1 dk birlikte toplayın.',
      'Duvarlarda hareketli/ışıklı uyaranı çalışma anında kaldırın.',
    ],
    sureDk: 10,
    malzeme: ['toplama kutusu'],
  },
  {
    id: 'AG-4',
    baslik: 'İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge',
    amac: 'İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + Z-7 işitsel).',
    icerik: [
      'Çalışma anında TV/arka plan sesini kapatın, kapıyı kapalı tutun.',
      'Yönergeyi göz hizasında, tek cümle, 2 adımı geçmeden söyleyin.',
      'Gerekirse söze değil, hafif dokunarak (omuz) dikkat toplayın.',
    ],
    sureDk: 10,
    malzeme: [],
  },
  {
    id: 'AG-5',
    baslik: 'Pekiştireç ve Kayıt — Hedef Davranış + İpucu',
    amac: 'Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 uyumlu çerçeve, Z-2).',
    icerik: [
      'Tek hedef seçin: “ödevin ilk 10 dk’sında masada kalma”.',
      'İpucu kademesi: model → sözel hatırlatma → bağımsız; ipucunu kademeli çekin.',
      'Her gün “yaptı / yapmadı” tik kartına işleyin, haftalık uzmana getirin (dijital puan yok).',
    ],
    sureDk: 15,
    malzeme: ['hedef kartı', 'tik tablosu'],
    uyari: 'Pekiştireç maddi değil, etkinlik/övgü temelli olabilir — uzman belirler.',
  },
];

~~~~

### `data/aile/kisisel.ts`
2063 B ·SHA `5042b956dea4e9d4869d08eaff71f19c471ba1cf1f1bcb8b6ad70d087d78e758`

~~~~tsx
/** B — Çocuğun Analiz Sonuçlarına Göre Aile Eğitimi (kişiselleştirilmiş, uzmanın seçtiği 1 kart)
 *  K-02: sistem otomatik öneri ÜRETMEZ — uzman B-4/C-3 rapordan seçer, veliye iletir.
 *  K-14: gözlemlenebilir + sayılabilir + bağlamlı dil. K-15: dijital puan YOK, basılabilir.
 *  K-08: TASLAK — şirket sonrası Turnitin/hukuk.
 */

export interface AileKisiselSablon {
  id: string;
  baglam: string; // hangi analiz tetikler (ör: izleme çizelgesinde “odak kopma >X”)
  baslik: string;
  uzmanNotuSablonu: string; // boş alan, uzman doldurur — sistem doldurmaz
  aileyeGorev: string; // 1 görev, 1 ipucu formatında
  olcum: string; // nasıl kayıt tutulacak (tik, süre)
}

export const AILE_KISISEL_SABLON: AileKisiselSablon = {
  id: 'AB-1',
  baglam: 'İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu',
  baslik: 'Analize Göre Aile Görevi (Uzman Seçer)',
  uzmanNotuSablonu: `[UZMAN DOLDURUR — K-02]\nGözlem/Rapor bulgusu (tarihli, sayılabilir): ...\nAileye önerilen tek görev (1 cümle, bağlamlı): ...\nİpucu kademesi (model/sözel/bağımsız): ...\nKayıt biçimi (tik/süre): ...\nSonraki izleme tarihi: ...\n`,
  aileyeGorev: 'Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.',
  olcum: 'Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.',
};

// Havuzdan seçim için 3 örnek başlık (uzman havuzdan 1’ini seçer, sistem seçmez)
export const AILE_KISISEL_HAVUZ = [
  { id: 'BK-1', baslik: 'Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme)', tetik: 'Çizelgede kopma > eşik' },
  { id: 'BK-2', baslik: 'Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev', tetik: 'Ev Çalışmaları “yapılmadı” >2' },
  { id: 'BK-3', baslik: 'Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme', tetik: 'Girdi “0/3” yoğun' },
] as const;

~~~~

### `data/bgm.ts`
16260 B ·SHA `93c62cc2772cea15044e48e021cef13ffb699fdc8adb406145982f46a91fb014`

~~~~tsx
/**
 * Bilişsel Geliştirme Modülleri (BGM-12) — Supporta menü katmanı.
 * Kaynak: CURRICULUM v1.3 §5 · TANIM KARTLARI v1.6 KART 2 · K-267 · K-393 · K-398 · K-400.
 * Tam taslak: SEDUVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md (pedagog + K-08 benzerlik taraması ÖNCESİ).
 *
 * Bu katman DEP-2026'dan AYRI durur:
 *   DEP  = BEP/RAM resmî saat-modül hizası (Program Hizalama)
 *   BGM  = DEHB yürütücü işlev içerik menüsü (bu dosya)
 * Uzman her ikisinden de seçer; sabit 12'li sıra YOKTUR (MODUL_SECIM_SERBEST).
 *
 * Dil: K-02 — tanı/tedavi/terapi iddiası yok; etki vaadi yok.
 * CURRICULUM kalıntıları (Bio-Sync, limbik, ms-beyin, "körlük") DEVRALINMAZ.
 */

export type BgmFaz = 'I' | 'II' | 'III';

export type BgmModul = {
  id: string;
  ad: string;
  kisa: string;
  faz: BgmFaz;
  dehbAlan: string;
  tanim: string;
  amac: string;
  olcum: string;
  etkinlik: string;
  odev: string;
  onlem: string;
  oneri: string;
  /** KART 2 "öncelikli çekirdek" */
  oncelikli: boolean;
  /** v0.8.0 (K-400) — etkinlik alan seti (DEP M4 ile aynı desen) */
  /** Bu BGM'nin KANIT üretebileceği DEP-2026 modülü; öneri — BEP birimi kararı değil (K-263). */
  depKoprusu: string | null;
  /** YASA-1: BGM etkinliği girdi üretir; varsayılan kodlama tipi. */
  girdiTipi: 'xArti' | 'sifirUc' | 'evetHayir';
  sureDk: string;
  malzeme: string[];
  ipucu: string;
  /** Ödev var mı (DS-10 / CM-11: yok). */
  odevVar: boolean;
  /** Dayanak = görev ailesi / kategori ATFI. Etki iddiası değil (K-04). */
  dayanak: string;
};

export const BGM_FAZ_ETIKET: Record<BgmFaz, string> = {
  I: 'Grup I — bilişsel kararlılık (sıra değil)',
  II: 'Grup II — esneklik ve düzenleme (sıra değil)',
  III: 'Grup III — uygulama ve otonomi (sıra değil)',
};

export const BGM_MODULLER: readonly BgmModul[] = [
  {
    id: 'FS-1', ad: 'Odak Kararlılığı', kisa: 'Görevi sürdürme',
    faz: 'I', dehbAlan: 'Sürdürülebilir dikkat',
    tanim: 'Kısa süreli bir görevi, çeldirici varken bile bırakmadan sürdürme alıştırması.',
    amac: 'Seans içinde kesintisiz çalışma süresini gözlemek; uzman hedefi BEP satırına taşır.',
    olcum: 'Kesintisiz odak süresi (dk) · isabet / yanlış basış (CPT deseni). Yüzdelik ve tanı YOK.',
    etkinlik: 'Kısa görsel tarama turu: hedef şekil belirdiğinde dokun, diğerlerinde bekle.',
    odev: 'Evde 5 dk tek görev (kitap/çalışma yaprağı). Puanlanmaz.',
    onlem: 'Masada yalnız o anki materyal; ekran ve televizyon görüş alanında olmasın.',
    oneri: 'Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.',
    oncelikli: true,
    depKoprusu: 'M1', girdiTipi: 'sifirUc', sureDk: '5–7 dk',
    malzeme: ['tarama kart seti', 'kum saati'],
    ipucu: 'model → sözel ("hedefi bekle") → bağımsız',
    odevVar: true,
    dayanak: 'CPT görev ailesi · PMC 5-küme ⑤ çevre kontrolü (literatür atfı; SEDUVA sonucu değil)',
  },
  {
    id: 'TPM-2', ad: 'Zaman Algısı', kisa: 'Süre tahmini',
    faz: 'I', dehbAlan: 'Zamanı ayarlama',
    tanim: 'Bir işin ne kadar süreceğini tahmin etme ve gerçek süreyle karşılaştırma.',
    amac: '“Az kaldı / çok kaldı” hissini sayılabilir süreyle eşlemek (takvim “hafta” değil, seans içi süre).',
    olcum: 'Tahmin − gerçek süre farkı (sn). Persona “İç Saat” ile aynı aile.',
    etkinlik: 'Kum saati tahmini: uzman 30/60/90 sn tutar, çocuk işaretler.',
    odev: 'Akşam rutininin bir adımına süre koyun (ör. çanta hazırlığı). Puan yok.',
    onlem: 'Görünür analog saat veya kum saati; sözel “acele et” yerine süre göstergesi.',
    oneri: 'Geçiş uyarısı (Z-13) seans bitimine 5 ve 1 dk kala — utançsız dil.',
    oncelikli: true,
    depKoprusu: 'M4', girdiTipi: 'sifirUc', sureDk: '5 dk',
    malzeme: ['kum saati / analog kronometre', 'tahmin kartı'],
    ipucu: 'görsel sayaç açık → yarı kapalı → kapalı',
    odevVar: true,
    dayanak: 'TMT-A / süre tahmini görev ailesi · PMC 5-küme ③ rutin-zamanlama',
  },
  {
    id: 'CC-3', ad: 'Parçalama (Chunking)', kisa: 'İşi bölme',
    faz: 'I', dehbAlan: 'Göreve başlama',
    tanim: 'Büyük işi tek adımlık parçalara bölme; ilk adımı görünür kılma (Z-15).',
    amac: 'Başlayamamayı “tembellik” diye değil, ilk-adım eksikliği olarak ele almak.',
    olcum: 'İlk eyleme kadar geçen süre · tamamlanan parça sayısı. Ölçüm yorumunu uzman yazar.',
    etkinlik: 'Görevi 3 karta böl: 1) bak 2) ilk satır 3) bırak. Kart 1 bitmeden 2 açılmaz.',
    odev: 'Yarınki ödevi velinin yanında 3 kutuya yazın. Sistem puanlamaz.',
    onlem: 'Yönerge en fazla 2 adım (Z-8); üçüncü adım ayrı cümle.',
    oneri: 'İpucu kademesi: model → sözel → bağımsız; silikleştirme notu uzmanda.',
    oncelikli: false,
    depKoprusu: 'M3', girdiTipi: 'xArti', sureDk: '6–8 dk',
    malzeme: ['çalışma yaprağı', '3 boş kart', 'kalem'],
    ipucu: 'model (uzman böler) → sözel → bağımsız (çocuk böler)',
    odevVar: true,
    dayanak: 'PMC 5-küme ① hedef-koçluk + ④ basit geri bildirim · MEB DEHB Bülteni "küçük parçalara bölme" (kavram atfı)',
  },
  {
    id: 'CA-4', ad: 'Bilgi Mimarisi', kisa: 'Çalışma belleği',
    faz: 'I', dehbAlan: 'Çalışma belleği',
    tanim: 'Kısa süreli tutulan bilgiyi sırayla geri çağırma alıştırması (Digit Span / N-Back deseni).',
    amac: 'Antrenman + dış araç (liste, görsel plan) birlikte; yalnız “ezber kası” değil.',
    olcum: 'Doğru dizi uzunluğu · Digit Span. Dış araç kullanımı gözlem notu (var/yok).',
    etkinlik: 'Sayı Dedektifi: 3–5 birimlik dizi, sözel tekrar. İpucu: görsel destek kademeli kalkar.',
    odev: 'Kapıya asılı 3 maddelik “yanına al” listesi (Ö-5 dış bellek). Puan yok.',
    onlem: 'Sözel yönergeyi yazılı/çizili kopyayla destekleyin; tek kanal yeterli olmayabilir.',
    oneri: 'Dış bellek aracı = zayıflık değil, düzenleme. Karşılaştırma dili yok.',
    oncelikli: true,
    depKoprusu: 'M1', girdiTipi: 'sifirUc', sureDk: '5 dk',
    malzeme: ['sayı/nesne kartları', 'küçük tahta'],
    ipucu: 'görsel destek açık → kademeli kalkar',
    odevVar: true,
    dayanak: 'Digit Span / N-Back görev ailesi · transfer iddiası YOK (Cogmed-tipi RED)',
  },
  {
    id: 'CS-5', ad: 'Bilişsel Esneklik', kisa: 'Kural değiştirme',
    faz: 'II', dehbAlan: 'Set değiştirme',
    tanim: 'Kurallar değişince eski kuralı bırakıp yenisine geçme alıştırması.',
    amac: '“Ama demin şöyleydi” takılmasını görünür kılmak; esneklik iddiası yok, gözlem var.',
    olcum: 'Kural değişiminden sonra ilk doğru tepkiye kadar deneme sayısı (TMT-B / task-switching deseni).',
    etkinlik: 'Renk-şekil değiştirme: ilk tur “kırmızıya bas”, ikinci tur “yuvarlağa bas”.',
    odev: 'Evde bir oyunun kuralını bilinçli değiştirin (bir tur). Puan yok.',
    onlem: 'Kural değişimini ses yükseltmeden, kısa cümleyle, göz hizasında bildirin.',
    oneri: 'Hata = kural geçişi verisi; “beceremedin” dili yok.',
    oncelikli: false,
    depKoprusu: 'M4', girdiTipi: 'sifirUc', sureDk: '5 dk',
    malzeme: ['renk-şekil kartları'],
    ipucu: 'geçişte model → sözel → bağımsız',
    odevVar: true,
    dayanak: 'TMT-B / task-switching görev ailesi',
  },
  {
    id: 'II-6', ad: 'Dürtü Engelleme', kisa: 'Dur–bekle–yap',
    faz: 'II', dehbAlan: 'İnhibitör kontrol',
    tanim: 'Tepki vermeden önce kısa bir durak (Go/No-Go). Ö-1 “Dur–Düşün–Uygula” kartı burada.',
    amac: 'Antrenman (Işık Yakala) + bilişsel strateji kartı birlikte; yalnız refleks değil.',
    olcum: 'Yanlış basış oranı (commission) · strateji kartı kullanıldı mı (E/H, puan değil).',
    etkinlik: 'Işık Yakala: yeşilde dokun, kırmızıda bekle. Seans öncesi 3 adımlık kart.',
    odev: 'Kapı eşiğinde “üç say, sonra geç” ritüeli. Puan yok.',
    onlem: 'Yönergeyi bitirmeden çocuktan eylem beklemeyin; omza hafif temaslı dikkat çekme (kavram, kopya değil).',
    oneri: 'Seans sonu yansıma: “Bugün acele ettiğin bir an oldu mu?” — sistem yorumlamaz.',
    oncelikli: true,
    depKoprusu: 'M6', girdiTipi: 'evetHayir', sureDk: '6 dk',
    malzeme: ['yeşil/kırmızı kartlar', '3 adımlık strateji kartı'],
    ipucu: 'kart açık → kart kapalı hatırlatma → bağımsız',
    odevVar: true,
    dayanak: 'Go/No-Go görev ailesi · davranış terapisi kategorisi (DBRC/token; literatür atfı)',
  },
  {
    id: 'SR-7', ad: 'Düzenleme Desteği', kisa: 'Nefes / mola',
    faz: 'II', dehbAlan: 'Duygu ve uyarılma',
    tanim: 'Yoğunluk artınca kısa, donanımsız durak (A-1 Nefes Ritmi). Biyogeribildirim / PPG YOK.',
    amac: 'Engellenme anında görevi bırakmadan 30–60 sn düzenleme alıştırması.',
    olcum: 'Mola isteği sayısı · mola sonrası göreve dönüş (E/H). “İyileşti” cümlesi YOK.',
    etkinlik: 'Nefes halkası: ekranda yavaşça büyüyen daire; çocuk birlikte nefes alır, sonra devam.',
    odev: 'Evde “zamanlı mola”: süre söylenir, bitince sorun birlikte konuşulur. Puan yok.',
    onlem: 'Nasihat, kıyas, ses yükseltme yok. Uzman/veli model olur.',
    oneri: 'Mightier tipi klinik etki rakamı DEVİR ALINMAZ (K-04).',
    oncelikli: true,
    depKoprusu: 'M6', girdiTipi: 'evetHayir', sureDk: '2–3 dk (ihtiyaç anında)',
    malzeme: ['nefes halkası kartı / ekran'],
    ipucu: 'birlikte → sözel → çocuk kendi başlatır',
    odevVar: true,
    dayanak: 'A-1 Nefes Ritmi (Gelişim Önerileri v1.2) · donanımsız; biyogeribildirim YOK',
  },
  {
    id: 'SP-8', ad: 'Önceliklendirme', kisa: 'Önemli / acil',
    faz: 'II', dehbAlan: 'Planlama',
    tanim: 'Sınırlı zamanda hangi işin önce geleceğini seçme alıştırması.',
    amac: 'Hepsinin birden yapılması beklentisini kırmak; sıra uzman ve çocukla kurulur.',
    olcum: 'İlk seçim süresi · seçilen işin bitip bitmediği (gözlem). Verim yüzdesi iddiası yok.',
    etkinlik: 'Üç kart: kolay-kısa, zor-kısa, kolay-uzun. Çocuk birini seçer, gerekçesini söyler.',
    odev: 'Yarınki üç işi “önce / sonra / olursa” diye yazın (Tablo 9 kavramı, cümle kopyası yok).',
    onlem: 'Aynı anda tek açık iş; diğer kartlar kapalı durur.',
    oneri: 'Sonuç önceden konuşulur (Ö-3 kontrat şablonuyla köprü). Sistem puanlamaz.',
    oncelikli: false,
    depKoprusu: 'M5', girdiTipi: 'evetHayir', sureDk: '5 dk',
    malzeme: ['3 görev kartı', 'kum saati'],
    ipucu: 'uzman gerekçeyi modeller → sorar → çocuk kendisi',
    odevVar: true,
    dayanak: 'PMC 5-küme ① hedef-koçluk · koçluk RCT (yetişkin popülasyon notu)',
  },
  {
    id: 'SR-9', ad: 'Sosyal İpucu', kisa: 'Sıra / dinleme',
    faz: 'III', dehbAlan: 'Sosyal dikkat',
    tanim: 'Sıra bekleme, söz bitmeden araya girmeme, yüz/ses ipucunu fark etme alıştırması.',
    amac: 'Açık sosyal beceri eğitimi değil; seans içi sıra ve dinleme gözlemi. Empati terapisi YOK.',
    olcum: 'Sıra ihlali sayısı · söz bitmeden verilen erken yanıt (gözlem).',
    etkinlik: 'İki tur: biri konuşur, diğeri bekler; zil çalınca rol değişir (A-3 köprüsü, grup P2).',
    odev: 'Evde yemek sırasında bir kişi konuşurken diğerinin bitmesini bekleme. Puan yok.',
    onlem: 'Grupta aynı anda tek konuşmacı; görsel “sıra çubuğu” masada durabilir.',
    oneri: 'Yapılandırılmış sosyal beceri programı (Ö-7) P2; bu kart onun yerini tutmaz.',
    oncelikli: false,
    depKoprusu: 'M6', girdiTipi: 'xArti', sureDk: '6 dk (2 kişi)',
    malzeme: ['sıra çubuğu', 'zil'],
    ipucu: 'çubuk görünür → sözel → bağımsız',
    odevVar: true,
    dayanak: 'DEP M6 sıra alma hedef ailesi (kod referans) · A-3 eşli oyun',
  },
  {
    id: 'DS-10', ad: 'Çift Kanal', kisa: 'İki iş birden',
    faz: 'III', dehbAlan: 'Bölünmüş dikkat',
    tanim: 'Görsel bir izleği sürdürürken basit işitsel hedefi yakalama alıştırması.',
    amac: 'Gürültülü ortamda tek kanala kapanmayı gözlemek. “Bant genişliği artırma” vaadi YOK.',
    olcum: 'Tek kanal vs çift kanal isabet farkı (betimleyici). Stroop deseni referans.',
    etkinlik: 'Ortadaki şekli izle + kulaklıktan “çift sayı” deyince yan düğmeye bas.',
    odev: 'Yok (evde çift kanal önerilmez; yorgunluk riski).',
    onlem: 'Seans odasında arka plan konuşması kısılır; gerekirse düşük sabit ses.',
    oneri: 'Yalnız uzman seansında; süre kısa tutulur.',
    oncelikli: false,
    depKoprusu: 'M1', girdiTipi: 'sifirUc', sureDk: '4 dk (kısa)',
    malzeme: ['izlek kartı', 'sayı listesi'],
    ipucu: 'tek kanal → çift kanal (yavaş ritim) → normal',
    odevVar: false,
    dayanak: 'Stroop / dual-task görev ailesi',
  },
  {
    id: 'CM-11', ad: 'Yüksek Yük', kisa: 'Baskıda sakin kalma',
    faz: 'III', dehbAlan: 'Yük altında sürdürme',
    tanim: 'Birden fazla kuralın aynı anda geldiği kısa tur; panik dili kullanılmaz.',
    amac: 'Önceki alıştırmaların bir arada durup durmadığını gözlemek — “kriz tedavisi” değil.',
    olcum: 'Hata sonrası göreve dönüş (E/H) · tur yarıda bırakıldı mı.',
    etkinlik: 'Kısa “karışık tur”: dur-bekle + kural değişimi + süre. Çocuk durdurabilir (S-1).',
    odev: 'Yok. Yüksek yük ev ödevi yapılmaz.',
    onlem: 'Çocuk kontrol çubuğu (mola/bitir) açık; ardışık zorlamada mola önerilir.',
    oneri: 'Tek oturumluk veriyle genelleme yok (Protokol §5.t).',
    oncelikli: false,
    depKoprusu: null, girdiTipi: 'evetHayir', sureDk: '4 dk',
    malzeme: ['önceki turların kartları', 'mola/bitir çubuğu'],
    ipucu: 'uzman yükü kademeli açar; çocuk durdurabilir (S-1)',
    odevVar: false,
    dayanak: 'önceki modüllerin bütünleştirilmesi; ayrı görev ailesi yok',
  },
  {
    id: 'TM-12', ad: 'Kendini Yönetme', kisa: 'Dış iskeleti solma',
    faz: 'III', dehbAlan: 'Üstbiliş / otonomi',
    tanim: 'Hazır görevi çocuğun kendi planlaması; hatırlatıcı kademeli azalır (metakognisyon ONAYLI konum).',
    amac: 'Platform iskeletini solmak; “karakter değişimi” vaadi YOK.',
    olcum: 'Hatırlatıcısız başlama (E/H) · planladığı işe dönüş. Öz-başlatma endeksi betimleyicidir.',
    etkinlik: 'Çocuk bugünkü gerçek işini (ödev/kitap) planlar; uzman yalnız izler, ipucu isterse verir.',
    odev: 'Kendi yazdığı 3 kutuluk planı odasına asmak (yazılı plan kavramı). Puan yok.',
    onlem: 'Karşılaştırma dili yok; her geribildirimde en az bir güçlü yön (Z-15).',
    oneri: 'Navigasyon: Kendini Yönetme (metakognisyon v1.0). Sistem otonomi ilan etmez.',
    oncelikli: false,
    depKoprusu: 'M3', girdiTipi: 'xArti', sureDk: '8–10 dk',
    malzeme: ['3 kutulu plan kartı', 'çocuğun kendi işi'],
    ipucu: 'istek üzerine → yok',
    odevVar: true,
    dayanak: 'metakognisyon konumlandırma v1.0 (K-118/119) · ipucu silikleştirme (Activity Schedule deseni)',
  },
] as const;

export const BGM_SAYI = BGM_MODULLER.length; // 12
export const BGM_ONCELIKLI = BGM_MODULLER.filter((m) => m.oncelikli).map((m) => m.id);
export const BGM_KATMAN_NOTU =
  'BGM-12, DEP-2026\'nın yerine geçmez. DEP = BEP/RAM saat hizası; BGM = yürütücü işlev menüsü. Uzman ikisinden de seçer.';

/** Pedagog + K-08 benzerlik taraması geçilmedi; ürün metinleri TASLAKTIR (K-398/K-400 dürüstlük). */
export const BGM_TASLAK_NOTU =
  'BGM kart metinleri PEDAGOG ONAYLI (04.09.2026); otomatik benzerlik ön taraması %0.000 temiz. Harici tarama + hukuki görüş (şirket sonrası) bekliyor. Etki iddiası içermez.';

/** BGM etkinliği kimliği — Oturum Atölyesi'nde DEP etkinlikleriyle aynı listede, ayrı etiketle (YASA-1). */
export const bgmEtkinlikId = (modulId: string) => `BGM-${modulId}`;
export const bgmEtkinlikMi = (etkinlikId: string) => etkinlikId.startsWith('BGM-');
export const bgmModulden = (etkinlikId: string) =>
  BGM_MODULLER.find((m) => bgmEtkinlikId(m.id) === etkinlikId) ?? null;

~~~~

### `data/kisitlar.ts`
6406 B ·SHA `868bfdb585d9f0a488f113c2e09756e7a2ffad1d6f1d47db50936e613ea3edcd`

~~~~tsx
/**
 * SEDUVA Supporta™ — KALICI KISITLAR (spec §1)
 * Bu dosya ürünün "anayasası"dır: şerhler silinemez, YASA'lar arayüzde zorlanır.
 * Kaynak: supporta-mvp-spec_v0.2.md · K-263 · K-281 · K-296 · K-331 · K-334 · K-88
 */

/** YASA-1: her performans girdisi BİR etkinliğe bağlıdır; etkinliksiz girdi sisteme girmez. */
export const YASA_1 = 'Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.';
/** YASA-2: çizelge motoru etkinlik motorundan doğar (bağımsız çizelge yok). */
export const YASA_2 = 'Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.';
/** YASA-3: her rapor taslaktır; uzman onayı olmadan geçerli belge değildir. */
export const YASA_3 = 'Rapor taslaktır; uzman onayı olmadan geçerli belge değildir.';

/** Ekranlarda SİLİNEMEZ sabit şerhler (spec §7). */
export const SHERHLER = {
  oturum: 'Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.',
  cizelge: 'Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.',
  rapor: 'TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).',
  aile: 'Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).',
  hizali: 'Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.',
  k02: 'SEDUVA Supporta bir destek eğitim aracıdır. Tanı, tedavi veya terapi uygulamaz; uzman kullanır.',
} as const;

/** DEP-2026 modül yapısı — giriş YALNIZ elle; hiçbir MEB sisteminden çekilmez (Y3 kırmızı çizgi). */
export const DEP_MODULLER = [
  { id: 'M1', ad: 'Öğrenmeye Destek', saat: 150, bolum: 5 },
  { id: 'M2', ad: 'Dil ve İletişim', saat: 150, bolum: 4 },
  { id: 'M3', ad: 'Okuma ve Yazma', saat: 300, bolum: 6 },
  { id: 'M4', ad: 'Erken Matematik', saat: 200, bolum: 8 },
  { id: 'M5', ad: 'Matematik', saat: 200, bolum: 4 },
  { id: 'M6', ad: 'Sosyal Etkileşim', saat: 100, bolum: 3 },
] as const;
export const DEP_TOPLAM_SAAT = DEP_MODULLER.reduce((t, m) => t + m.saat, 0); // 1100
export const DEP_SEMA_SURUM = 'DEP-2026 (ORGM 2026_01)';

/** Girdi kodlama tipleri (spec M5). */
export const KODLAMA = {
  xArti: { ad: 'x / +', aciklama: 'x: hedeflenen · +: ulaşılan (PKF deseni)' },
  sifirUc: { ad: '0-3', aciklama: 'ölçüt düzeyi (PBF deseni)' },
  evetHayir: { ad: 'Evet / Hayır', aciklama: 'gözlendi / gözlenmedi (KDF deseni)' },
} as const;

/** Oturum durumları (spec M2). */
export const OTURUM_DURUM = ['planlandı', 'tamamlandı', 'iptal', 'gelmedi'] as const;
export type OturumDurum = (typeof OTURUM_DURUM)[number];

/**
 * K-267 TERİM KURALI: birim adı **MODÜL**'dür ("hafta" değil).
 * Kapsayıcı ad: "Bilişsel Geliştirme Modülleri" (CURRICULUM §5 başlığı köklü).
 * K-393: Supporta'da modüller **sıralı değildir**.
 * K-398: kural BGM-12 menüsüne de uygulanır (KART 2). DEP-2026 ayrı katmandır.
 */
export const MODUL_SECIM_SERBEST = true;
export const MODUL_TERIM_NOTU =
  'Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.';

/** ÖEK Yönetmeliği (RG 11/7/2025-32953) kaynaklı KAPSAM DIŞI çizgileri (K-330). */
export const KAPSAM_DISI = [
  { ad: 'Devam/yoklama takibi', gerekce: 'BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.' },
  { ad: 'Ödeme · fatura · idari-mali işleyiş', gerekce: 'K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.' },
  { ad: 'Resmî form üretimi', gerekce: 'K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.' },
] as const;

/** Ders saati tavanları — ÖEK Yön. md.24/4 (güncel resmî sınır; ürün bunları AŞAN plan önermez). */
export const DERS_TAVAN = {
  aylikBireysel: 12, aylikGrup: 4, haftalikBireysel: 4, haftalikGrup: 2,
  gunlukToplam: 3, telafiPenceresiAy: 24,
} as const;

/**
 * DEP-2026 resmî FORM AİLESİ (EK-1…EK-7) — kaynak: LEXIVA-BEP-FORM-ESLEMESI_v1.0 (K-370).
 * K-395: LEXIVA'da çıkarılan bu eşleme ÖZEL EĞİTİM GENELİDİR; Supporta'ya da aittir.
 * Supporta KANIT üretir · uzman KARAR verir · RAM ONAYLAR. Form doldurulmaz (K-263).
 */
export const RESMI_FORMLAR = [
  { ek: 'EK-1', ad: 'Ölçüt Bağımlı Test (ÖBT)', an: 'ilk / ara / son değ.',
    besleyen: 'Tekrar ve deneme sayısı → Ölçüt alanı', tur: 'kanıt' },
  { ek: 'EK-2', ad: 'Kontrol Listesi', an: 'ilk / ara / son değ.',
    besleyen: 'Evet/Hayır girdileri → Açıklamalar sütunu', tur: 'kanıt' },
  { ek: 'EK-3', ad: 'Dereceli Puanlama Anahtarı', an: 'değerlendirme',
    besleyen: '0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)', tur: 'kanıt' },
  { ek: 'EK-4', ad: 'Performans Kayıt Formu', an: 'her modülün başı ve sonu',
    besleyen: 'x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)', tur: 'kanıt' },
  { ek: 'EK-5', ad: 'BEP Gelişimi İzleme Özet Formu', an: 'süreç + yıl sonu',
    besleyen: 'Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler', tur: 'kanıt' },
  { ek: 'EK-6', ad: 'Portfolyo Kontrol Listesi', an: 'modül sonu / yıl sonu',
    besleyen: 'Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)', tur: 'dosya' },
  { ek: 'EK-7', ad: 'Portfolyo Dereceli Puanlama Anahtarı', an: 'portfolyo değ.',
    besleyen: '—', tur: 'kapsam dışı' },
] as const;

/** Kayıt hattı ayrımı — ÖEKY md.20/2 (RG 11/7/2025-32953). İki farklı süreç. */
export const KAYIT_HATTI = [
  { id: 'a', ad: '(a) Ücreti Bakanlıkça karşılanan', ram: 'ZORUNLU (rapor + ÖEDK planı + BKDS onamı)',
    planlama: 'ÖEDK eğitim planı ekseninde' },
  { id: 'b', ad: '(b) Ücretini kendisi/velisi karşılayan', ram: 'İSTENMİYOR',
    planlama: 'Kayıttaki ölçme sonuçlarıyla BEP birimince (md.24/6 · md.26/3)' },
] as const;
export type KayitHatti = (typeof KAYIT_HATTI)[number]['id'];

/** Roller ve yetkiler (spec §3). VELİ ROLÜ YOKTUR (K-296/KC7). */
export const ROLLER = [
  { id: 'yonetici', ad: 'Yönetici', yetki: 'Tüm dosyalar · rapor onayı · dışa aktarma' },
  { id: 'uzman', ad: 'Uzman / Eğitimci', yetki: 'Kendi dosyaları · oturum · girdi · rapor taslağı' },
] as const;
export type RolId = (typeof ROLLER)[number]['id'];

~~~~

### `data/mock.ts`
13796 B ·SHA `1bf7767b955b43f4808a4118596e1444ff0fa7e9832b1bfbdefc18bcae5e9e57`

~~~~tsx
/** Sentetik demo verisi — K-05: prototipte GERÇEK ÇOCUK VERİSİ YOKTUR.
 *  Maskeli UID + kurgusal ad; yaş bandı 8-10 (K-270). */
import type { Dosya, Program, Oturum, Etkinlik, Girdi, Rapor, EvOdevi, RamKaydi } from './tipler';

export const DOSYALAR: Dosya[] = [
  { uid: 'ÖĞR-4417', ad: 'Öğrenci A. (2. Sınıf)', dogum: '2018-04-12', okulSinif: 'Atatürk İlkokulu / 2-B',
    devamsizlikNotu: 'Son ayda 2 gün', gecmisBepNotu: 'RAM eğitsel değerlendirme mevcut (2025)',
    veli: { ad: 'Veli A.', tel: '05xx xxx 41 17', adres: 'İzmir / Bornova', rizaTarihi: '2026-08-20' } },
  { uid: 'ÖĞR-2903', ad: 'Öğrenci B. (3. Sınıf)', dogum: '2017-11-03', okulSinif: 'Cumhuriyet İlkokulu / 3-A',
    devamsizlikNotu: '—', gecmisBepNotu: 'BEP dosyası okuldan bekleniyor',
    veli: { ad: 'Veli B.', tel: '05xx xxx 29 03', adres: 'İzmir / Karşıyaka', rizaTarihi: '2026-09-01' } },
];

export const PROGRAMLAR: Program[] = [
  { dosyaUid: 'ÖĞR-4417', seansSayisi: 24, siklik: 'Haftada 1 (40 dk)', aileBileseni: true,
    ramRaporRef: 'RAM-2025/1184', depModul: 'M3', depSaat: 300, depSemaSurum: 'DEP-2026 (ORGM 2026_01)', kayitHatti: 'a' },
  { dosyaUid: 'ÖĞR-2903', seansSayisi: 16, siklik: 'Haftada 1 (40 dk)', aileBileseni: false,
    ramRaporRef: '—', depModul: null, depSaat: null, depSemaSurum: 'DEP-2026 (ORGM 2026_01)', kayitHatti: 'b' },
];

export const OTURUMLAR: Oturum[] = [
  { id: 'OT-101', dosyaUid: 'ÖĞR-4417', tarih: '2026-09-03', saat: '10:00', durum: 'tamamlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-102', dosyaUid: 'ÖĞR-4417', tarih: '2026-09-10', saat: '10:00', durum: 'planlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-103', dosyaUid: 'ÖĞR-2903', tarih: '2026-09-03', saat: '10:00', durum: 'planlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-104', dosyaUid: 'ÖĞR-2903', tarih: '2026-08-27', saat: '11:00', durum: 'gelmedi', sureDk: 40, uzmanId: 'UZM-2' },
];

export const ETKINLIKLER: Etkinlik[] = [
  { id: 'ET-1', ad: 'Hece ayırma çalışması', hedefKod: '3.1.2', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Sözel ipucu → model → bağımsız', malzeme: ['hece kartları', 'çalışma yaprağı'], katman: 'DEP' },
  { id: 'ET-2', ad: 'Sesli okuma — tekrarlı', hedefKod: '3.3.1', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Eşli okuma → bağımsız', malzeme: ['kısa metin', 'kronometre'], katman: 'DEP' },
  { id: 'ET-3', ad: 'Görsel dikkat eşleme', hedefKod: '1.1.3', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'İşaret → sözel → bağımsız', malzeme: ['eşleme kartları'], katman: 'DEP' },
  { id: 'ET-4', ad: 'İşitsel bellek dizisi', hedefKod: '1.2.1', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Model → gecikmeli model → bağımsız', malzeme: ['ses kartları'], katman: 'DEP' },
  { id: 'ET-5', ad: 'Sözcük dağarcığı — nesne adlandırma', hedefKod: '2.2.1', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Fiziksel ipucu → sözel → bağımsız', malzeme: ['nesne resimleri'], katman: 'DEP' },
  { id: 'ET-6', ad: 'Nesne niteliği ayırt etme', hedefKod: '4.1.2', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → kısmi ipucu → bağımsız', malzeme: ['blok seti'], katman: 'DEP' },
  { id: 'ET-7', ad: 'Ritmik sayma (100 içinde)', hedefKod: '5.1.4', modulAdi: 'Matematik',
    ipucuKademesi: 'Birlikte sayma → bağımsız', malzeme: ['sayı doğrusu'], katman: 'DEP' },
  { id: 'ET-8', ad: 'Sıra alma ve bekleme', hedefKod: '6.2.3', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Model → sözel hatırlatma → bağımsız', malzeme: ['sıra kartı', 'kum saati'], katman: 'DEP' },
  // — v0.8.1 genişletme: her modüle +2/3 ek (toplam 24, 4×6) —
  { id: 'ET-9', ad: 'Sürdürülebilir dikkat — nesne takibi', hedefKod: '1.3.2', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Model → sözel ipucu → bağımsız', malzeme: ['renkli toplar', 'tepsi'], katman: 'DEP' },
  { id: 'ET-10', ad: 'Yönerge izleme (2 adımlı)', hedefKod: '1.4.1', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Fiziksel rehber → sözel → bağımsız', malzeme: ['yönerge kartları'], katman: 'DEP' },
  { id: 'ET-11', ad: 'Dinlediğini anlama — kısa öykü', hedefKod: '2.1.3', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Sözel ipucu → soru-cevap → bağımsız', malzeme: ['öykü kartı', 'soru listesi'], katman: 'DEP' },
  { id: 'ET-12', ad: 'Sözel ifade — cümle kurma', hedefKod: '2.3.2', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Model cümle → tamamlama → bağımsız', malzeme: ['kelime kartları'], katman: 'DEP' },
  { id: 'ET-13', ad: 'Karşılıklı konuşma sürdürme', hedefKod: '2.4.1', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Sözel başlatma → sıra alma → bağımsız', malzeme: ['konu kartları', 'kum saati'], katman: 'DEP' },
  { id: 'ET-14', ad: 'Harf-ses eşleme', hedefKod: '3.2.1', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Model → eşleme → bağımsız', malzeme: ['harf kartları', 'ses kutusu'], katman: 'DEP' },
  { id: 'ET-15', ad: 'Yazma — harf dikte', hedefKod: '3.4.2', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Noktalı iz → kopya → bağımsız', malzeme: ['dikte yaprağı', 'kalem'], katman: 'DEP' },
  { id: 'ET-16', ad: 'Gruplama / sınıflama', hedefKod: '4.2.3', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → sözel ipucu → bağımsız', malzeme: ['sınıflama kutuları', 'nesneler'], katman: 'DEP' },
  { id: 'ET-17', ad: 'Birebir eşleştirme', hedefKod: '4.3.1', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Fiziksel rehber → bağımsız', malzeme: ['eş kartları'], katman: 'DEP' },
  { id: 'ET-18', ad: 'Sıralama (büyük-küçük)', hedefKod: '4.4.2', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → deneme-yanılma → bağımsız', malzeme: ['sıralama şeridi'], katman: 'DEP' },
  { id: 'ET-19', ad: 'Sayı doğrusu ile toplama', hedefKod: '5.2.2', modulAdi: 'Matematik',
    ipucuKademesi: 'Model → rehberli → bağımsız', malzeme: ['sayı doğrusu', 'pul'], katman: 'DEP' },
  { id: 'ET-20', ad: 'Çıkarma (nesne ile)', hedefKod: '5.2.4', modulAdi: 'Matematik',
    ipucuKademesi: 'Nesne desteği → zihinden', malzeme: ['sayma pulları'], katman: 'DEP' },
  { id: 'ET-21', ad: 'Günlük yaşam problemi kurma', hedefKod: '5.3.1', modulAdi: 'Matematik',
    ipucuKademesi: 'Sözel senaryo → model → bağımsız', malzeme: ['problem kartları'], katman: 'DEP' },
  { id: 'ET-22', ad: 'Duygu tanıma', hedefKod: '6.1.2', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Görsel ipucu → eşleme → bağımsız', malzeme: ['duygu kartları'], katman: 'DEP' },
  { id: 'ET-23', ad: 'İş birliği oyunu', hedefKod: '6.3.1', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Eşli oyun → sıra alma → bağımsız', malzeme: ['kutu oyunu'], katman: 'DEP' },
  { id: 'ET-24', ad: 'Kurala uyma (oyun)', hedefKod: '6.3.3', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Model → hatırlatma → bağımsız', malzeme: ['kural kartı'], katman: 'DEP' },

  // — v0.8.3 BGM-12 etkinlikleri — katalogda ayrı filtre (DEP ile karıştırma yok; K-398 kuyruğu) —
  { id: 'ET-BGM-FS-1', ad: 'BGM — Odak Kararlılığı (Hedefi Yakala)', hedefKod: 'BGM-FS-1', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['tarama kart seti', 'kum saati'], katman: 'BGM' },
  { id: 'ET-BGM-TPM-2', ad: 'BGM — Zaman Algısı (Kum Saati Tahmini)', hedefKod: 'BGM-TPM-2', modulAdi: 'BGM-12', ipucuKademesi: 'Görsel sayaç açık → yarı kapalı → kapalı', malzeme: ['kum saati', 'tahmin kartı'], katman: 'BGM' },
  { id: 'ET-BGM-CC-3', ad: 'BGM — Parçalama (Üç Kart)', hedefKod: 'BGM-CC-3', modulAdi: 'BGM-12', ipucuKademesi: 'Model (uzman böler) → sözel → bağımsız', malzeme: ['çalışma yaprağı', '3 boş kart', 'kalem'], katman: 'BGM' },
  { id: 'ET-BGM-CA-4', ad: 'BGM — Bilgi Mimarisi (Sayı Dedektifi)', hedefKod: 'BGM-CA-4', modulAdi: 'BGM-12', ipucuKademesi: 'Görsel destek açık → kademeli kalkar', malzeme: ['sayı/nesne kartları', 'küçük tahta'], katman: 'BGM' },
  { id: 'ET-BGM-CS-5', ad: 'BGM — Bilişsel Esneklik (Renk mi Şekil mi?)', hedefKod: 'BGM-CS-5', modulAdi: 'BGM-12', ipucuKademesi: 'Geçişte model → sözel → bağımsız', malzeme: ['renk-şekil kartları'], katman: 'BGM' },
  { id: 'ET-BGM-II-6', ad: 'BGM — Dürtü Engelleme (Işık Yakala + 3 Adım)', hedefKod: 'BGM-II-6', modulAdi: 'BGM-12', ipucuKademesi: 'Kart açık → kapalı hatırlatma → bağımsız', malzeme: ['yeşil/kırmızı kartlar', 'strateji kartı'], katman: 'BGM' },
  { id: 'ET-BGM-SR-7', ad: 'BGM — Düzenleme Desteği (Nefes Halkası)', hedefKod: 'BGM-SR-7', modulAdi: 'BGM-12', ipucuKademesi: 'Birlikte → sözel → çocuk kendi başlatır', malzeme: ['nefes halkası kartı'], katman: 'BGM' },
  { id: 'ET-BGM-SP-8', ad: 'BGM — Önceliklendirme (Önce Hangisi?)', hedefKod: 'BGM-SP-8', modulAdi: 'BGM-12', ipucuKademesi: 'Uzman gerekçeyi modeller → sorar → çocuk kendisi', malzeme: ['3 görev kartı', 'kum saati'], katman: 'BGM' },
  { id: 'ET-BGM-SR-9', ad: 'BGM — Sosyal İpucu (Sıra Çubuğu)', hedefKod: 'BGM-SR-9', modulAdi: 'BGM-12', ipucuKademesi: 'Çubuk görünür → sözel → bağımsız', malzeme: ['sıra çubuğu', 'zil'], katman: 'BGM' },
  { id: 'ET-BGM-DS-10', ad: 'BGM — Çift Kanal (Çift Görev)', hedefKod: 'BGM-DS-10', modulAdi: 'BGM-12', ipucuKademesi: 'Tek kanal → çift kanal → normal', malzeme: ['izlek kartı', 'sayı listesi'], katman: 'BGM' },
  { id: 'ET-BGM-CM-11', ad: 'BGM — Yüksek Yük (Karışık Tur)', hedefKod: 'BGM-CM-11', modulAdi: 'BGM-12', ipucuKademesi: 'Uzman yükü kademeli açar', malzeme: ['önceki tur kartları'], katman: 'BGM' },
  { id: 'ET-BGM-TM-12', ad: 'BGM — Kendini Yönetme (Kendi Planım)', hedefKod: 'BGM-TM-12', modulAdi: 'BGM-12', ipucuKademesi: 'İstek üzerine → yok', malzeme: ['3 kutulu plan kartı', 'çocuğun kendi işi'], katman: 'BGM' },
];

export const GIRDILER: Girdi[] = [
  { id: 'G-1', oturumId: 'OT-101', etkinlikId: 'ET-1', kodlamaTipi: 'xArti', deger: '+', tarih: '2026-09-03', girenRol: 'uzman' },
  { id: 'G-2', oturumId: 'OT-101', etkinlikId: 'ET-2', kodlamaTipi: 'sifirUc', deger: '2', tarih: '2026-09-03', girenRol: 'uzman' },
  { id: 'G-3', oturumId: 'OT-101', etkinlikId: 'ET-3', kodlamaTipi: 'evetHayir', deger: 'Evet', tarih: '2026-09-03', girenRol: 'uzman' },
];

export const RAPORLAR: Rapor[] = [
  { id: 'R-1', dosyaUid: 'ÖĞR-4417', tur: 'seans', baslik: 'Seans Özeti — 03.09.2026',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.' },
  { id: 'R-2', dosyaUid: 'ÖĞR-4417', tur: 'aylik', baslik: 'Aylık Gelişim Özeti — Ağustos 2026',
    taslak: false, onayKim: 'Yönetici', onayTarih: '2026-09-01', kopyaSayisi: 2,
    icerik: 'Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.' },
  { id: 'R-3', dosyaUid: 'ÖĞR-4417', tur: 'donem', baslik: 'Dönem Sonu Değerlendirme — 2026 Güz',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.' },
  { id: 'R-4', dosyaUid: 'ÖĞR-4417', tur: 'bep-ilerleme', baslik: 'BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.' },
  { id: 'R-5', dosyaUid: 'ÖĞR-4417', tur: 'ram-paketi', baslik: 'RAM İzleme Paketi Hazırlığı',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM\'a iletilir; iki kopya üretilir.' },
  { id: 'R-6', dosyaUid: 'ÖĞR-4417', tur: 'aile-bilgilendirme', baslik: 'Aile Bilgilendirme Çıktısı — Eylül',
    taslak: false, onayKim: 'Uzman / Eğitimci', onayTarih: '2026-09-02', kopyaSayisi: 1,
    icerik: 'Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.' },
];

export const EV_ODEVLERI: EvOdevi[] = [
  { id: 'EV-1', dosyaUid: 'ÖĞR-4417', baslik: 'Mutfakta hece avı (5 nesne)', kim: 'Veli',
    neZaman: 'Hafta içi 3 gün · 10 dk', durum: 'yapıldı', not: 'Çocuk istekliydi; 4 nesne bağımsız heceledi.' },
  { id: 'EV-2', dosyaUid: 'ÖĞR-4417', baslik: 'Gazete başlığı okuma', kim: 'Veli',
    neZaman: 'Hafta sonu · 1 kez', durum: 'verildi', not: '' },
  { id: 'EV-3', dosyaUid: 'ÖĞR-2903', baslik: 'Sayı kartlarıyla eşleme', kim: 'Veli',
    neZaman: 'Hafta içi 2 gün', durum: 'yapılmadı', not: 'Aile yoğunluk bildirdi; süre kısaltıldı.' },
];

export const RAM_KAYITLARI: RamKaydi[] = [
  { dosyaUid: 'ÖĞR-4417', raporNo: 'RAM-2025/1184', tarih: '2025-10-14', gecerlilik: '2026-10-14',
    edifDurumu: 'İlk İnceleme tamamlandı (e-Rehberlik)', portfolyoHazir: true, sonrakiIzleme: '2026-09-30' },
  { dosyaUid: 'ÖĞR-2903', raporNo: '—', tarih: '—', gecerlilik: '—',
    edifDurumu: '(b) hattı — RAM raporu istenmiyor (ÖEKY md.20/2)', portfolyoHazir: false, sonrakiIzleme: '—' },
];

~~~~

### `data/tipler.ts`
2349 B ·SHA `0de7b17924221ab7e5af0b2f5f1d8b0ef31ee6108e8e87d8b0dde498e4cecb78`

~~~~tsx
/** SEDUVA Supporta™ — veri modeli (spec §5). */
import type { OturumDurum } from './kisitlar';

export interface Veli { ad: string; tel: string; adres: string; rizaTarihi: string | null; }
export interface Dosya {
  uid: string; ad: string; dogum: string; okulSinif: string;
  devamsizlikNotu: string; veli: Veli; gecmisBepNotu: string;
}
export interface EvOdevi {
  id: string; dosyaUid: string; baslik: string; kim: string;
  neZaman: string; durum: 'verildi' | 'yapıldı' | 'yapılmadı'; not: string;
}
export interface RamKaydi {
  dosyaUid: string; raporNo: string; tarih: string; gecerlilik: string;
  edifDurumu: string; portfolyoHazir: boolean; sonrakiIzleme: string;
}
export interface Program {
  dosyaUid: string; seansSayisi: number; siklik: string;
  aileBileseni: boolean; ramRaporRef: string;
  depModul: string | null; depSaat: number | null; depSemaSurum: string;
  kayitHatti: 'a' | 'b';   // ÖEKY md.20/2
}
export interface Oturum {
  id: string; dosyaUid: string; tarih: string; saat: string;
  durum: OturumDurum; sureDk: number; uzmanId: string;
}
export interface Etkinlik {
  id: string; ad: string; hedefKod: string; modulAdi: string;
  ipucuKademesi: string; malzeme: string[]; katman?: 'DEP' | 'BGM';
}
export interface Girdi {
  id: string; oturumId: string; etkinlikId: string;   // YASA-1: etkinlik ZORUNLU
  kodlamaTipi: 'xArti' | 'sifirUc' | 'evetHayir';
  deger: string; tarih: string; girenRol: string;
  ipucuGozlem?: IpucuGozlem;   // K-571/A4 (opsiyonel; eski-veri güvenli)
}
/** K-571/A4: uzmanın GÖZLEDİĞİ ipucu-kademesi (etkinlik-ipucuKademesi planlıdır; bu alan oturum-ayakta teyididir — K-02: gözlem-kaydı, ölçüm-değil). */
export type IpucuGozlem = 'model' | 'sozel' | 'bagimsiz';
/** K-571/A2: veli görüşme-randevu defteri kaydı — hatırlatma GÖNDERİLMEZ (K-334); defter yalnız yerel (K-05). */
export interface Gorusme {
  id: string; dosyaUid: string; tarih: string; konu: string;
  durum: 'planlandı' | 'gerçekleşti' | 'ertelendi' | 'iptal';
  not: string;
}
export type RaporTur = 'seans' | 'aylik' | 'donem' | 'bep-ilerleme' | 'ram-paketi' | 'aile-bilgilendirme';
export interface Rapor {
  id: string; dosyaUid: string; tur: RaporTur; baslik: string;
  taslak: boolean; onayKim: string | null; onayTarih: string | null;
  kopyaSayisi: number; icerik: string;
}

~~~~

### `lib/depo.ts`
980 B ·SHA `5a092cceee50bc329f3c55f886640b0ab96e7335a10c555bff71c4e274fc8b87`

~~~~tsx
/**
 * Yerel kalıcılık (localStorage) — KVKK yerel-önce ilkesi (K-07/K-09).
 * Buluta hiçbir şey gitmez. Sürüm anahtarı ile şema değişiminde eski veri düşer.
 */
const ONEK = 'seduva-supporta';
const SEMA = 'v1';
const K = (ad: string) => `${ONEK}:${SEMA}:${ad}`;

export function yukle<T>(ad: string, varsayilan: T): T {
  try {
    const ham = localStorage.getItem(K(ad));
    return ham ? (JSON.parse(ham) as T) : varsayilan;
  } catch { return varsayilan; }
}
export function kaydet<T>(ad: string, deger: T): void {
  try { localStorage.setItem(K(ad), JSON.stringify(deger)); } catch { /* kota/kapalı: sessiz geç */ }
}
export function temizle(): void {
  try {
    Object.keys(localStorage).filter((k) => k.startsWith(`${ONEK}:`)).forEach((k) => localStorage.removeItem(k));
  } catch { /* yoksay */ }
}
export function kayitSayisi(): number {
  try { return Object.keys(localStorage).filter((k) => k.startsWith(`${ONEK}:`)).length; } catch { return 0; }
}

~~~~

### `lib/kullan.ts`
355 B ·SHA `46810d4fa8d9838b16029e9c367bf64d1a145ef73f08edacbc99066280d5b842`

~~~~tsx
/** localStorage'a bağlı state kancası. */
import { useEffect, useState } from 'react';
import { yukle, kaydet } from './depo';

export function useKalici<T>(ad: string, varsayilan: T) {
  const [deger, setDeger] = useState<T>(() => yukle(ad, varsayilan));
  useEffect(() => { kaydet(ad, deger); }, [ad, deger]);
  return [deger, setDeger] as const;
}

~~~~

### `main.tsx`
220 B ·SHA `0841d035eaea39546619092e503383a2682334339d1384137f6f4d04c73eeafa`

~~~~tsx
import React from 'react';
import { createRoot } from 'react-dom/client';
import App from './App';
import './index.css';
createRoot(document.getElementById('root')!).render(<React.StrictMode><App /></React.StrictMode>);

~~~~

### `surum.d.ts`
181 B ·SHA `070eb2cfcd976ffdf9a06eea3da5d7186538912f8b14d446be3580645647c54c`

~~~~tsx
/** Sürüm sabiti (K-368). Tek doğruluk kaynağı: package.json → version. */
declare const __SURUM__: string;
declare const __TAM__: boolean;
declare const __PILOT__: boolean;

~~~~

# Ek C-LEX — SUPPORTA-LEX bağımsız kanıt havuzu

## DOM35 durum / seçilmiş akışlar

### SUP-LEX-DOM-uzman-rol-secimi

~~~~text
S
LEXIVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)

Özel eğitim merkezi uzman kokpiti · v2.10.0

Devam etmek için rolünüzü seçin.

Yönetici
Tüm dosyalar · rapor onayı · dışa aktarma
Uzman / Eğitimci
Kendi dosyaları · oturum · girdi · rapor taslağı

Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
~~~~

### SUP-LEX-DOM-uzman-nav-pano

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif

Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.

T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)
2026-09-10 10:00 — ÖĞR-4417 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
2026-09-03 10:00 — ÖĞR-2903 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
Onay Bekleyen Raporlar (Human-Accountable AI)
4
• Seans Özeti — 03.09.2026
• Dönem Sonu Değerlendirme — 2026 Güz
• BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
• RAM İzleme Paketi Hazırlığı

YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).
~~~~

### SUP-LEX-DOM-uzman-nav-dosyalar

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Dosya listesi
ÖĞR-4417
ÖĞR-2903
Dosya kartı — ÖĞR-4417
Ad (maskeli)
Öğrenci A. (2. Sınıf)
Doğum
2018-04-12
Okul / Sınıf
Atatürk İlkokulu / 2-B
Devamsızlık
Son ayda 2 gün
Veli
Veli A. · 05xx xxx 41 17
Rıza kaydı
2026-08-20
Geçmiş BEP
RAM eğitsel değerlendirme mevcut (2025)
Program kartı
Seans sayısı
24
Sıklık
Haftada 1 (40 dk)
Aile bileşeni
Var
RAM rapor ref.
RAM-2025/1184
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-LEX-DOM-uzman-nav-takvim

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Oturum takvimi
2026-09-03 haftası
Çakışma: 2026-09-03 10:00 UZM-1 (KC12)
Tarih	Saat	Dosya	Uzman	Durum
2026-09-03	10:00	ÖĞR-4417	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

2026-09-03	10:00	ÖĞR-2903	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

Durumlar: planlandı · tamamlandı · iptal · gelmedi · değişiklikler bu cihazda saklanır.

Veli görüşme-randevu defteri (K-571/A2)
hatırlatma gönderilmez — K-334
Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
Tarih
Konu
Deftere ekle

Defter boş — ilk görüşme kaydını ekleyin.

Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).
~~~~

### SUP-LEX-DOM-uzman-nav-oturum

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Oturum kartı — OT-101

Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı

Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)

Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
ⓘ
Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)
Bu oturumda seçili BGM modülleri
ÖĞR-4417 · sıra uzmanın
EQ-01 · Ses Merdiveni BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M3
EQ-02 · Ses Birimi Ayırt Etme BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M3
EQ-05 · Söyleneni Yaz BGM
6 dk · girdi: x / + · DEP köprüsü M3

Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez.

Hızlı girdi paneli
YASA-1 etkin
Etkinlik *zorunlu
— etkinlik seçin —
Hece ayırma çalışması (3.1.2)
Sesli okuma — tekrarlı (3.3.1)
Görsel dikkat eşleme (1.1.3)
İşitsel bellek dizisi (1.2.1)
Sözcük dağarcığı — nesne adlandırma (2.2.1)
Nesne niteliği ayırt etme (4.1.2)
Ritmik sayma (100 içinde) (5.1.4)
Sıra alma ve bekleme (6.2.3)
Sürdürülebilir dikkat — nesne takibi (1.3.2)
Yönerge izleme (2 adımlı) (1.4.1)
Dinlediğini anlama — kısa öykü (2.1.3)
Sözel ifade — cümle kurma (2.3.2)
Karşılıklı konuşma sürdürme (2.4.1)
Harf-ses eşleme (3.2.1)
Yazma — harf dikte (3.4.2)
Gruplama / sınıflama (4.2.3)
Birebir eşleştirme (4.3.1)
Sıralama (büyük-küçük) (4.4.2)
Sayı doğrusu ile toplama (5.2.2)
Çıkarma (nesne ile) (5.2.4)
Günlük yaşam problemi kurma (5.3.1)
Duygu tanıma (6.1.2)
İş birliği oyunu (6.3.1)
Kurala uyma (oyun) (6.3.3)
BGM — Ses Merdiveni (Fonolojik Eşleme) (BGM-EQ-01)
BGM — Ses Birimi Ayırt Etme (SBA Turu) (BGM-EQ-02)
BGM — Hece ve Parçalar (El Çırparak Heceleme) (BGM-EQ-03)
BGM — Harf Tanıma ve Çizim (b/d-l İzleme) (BGM-EQ-04)
BGM — Söyleneni Yaz (Hata Sınıfı ile) (BGM-EQ-05)
BGM — Akıcı Okuma (Tekrarlı + M-4) (BGM-EQ-06)
BGM — Sözcük Çantası (Günün 5 Sözcüğü) (BGM-EQ-07)
BGM — Anlama Kartı (Okudunu Söyle) (BGM-EQ-08)
BGM — Sayı Blokları (Çokluk + Karıştırma Çifti) (BGM-EQ-09)
BGM — Süre Algısı (Kum Saati Tahmini) (BGM-EQ-10)
BGM — Transfer ve Serbest Okuma (BGM-EQ-11)
BGM — Okuma Özerkliği (Kendi Planım) (BGM-EQ-12)
[BGM] EQ-01 · Ses Merdiveni
[BGM] EQ-02 · Ses Birimi Ayırt Etme
[BGM] EQ-05 · Söyleneni Yaz
Kodlama
x / +
0-3
Evet / Hayır
Değer
Gözlenen ipucu-kademesi (K-571/A4)
— seçilmeyebilir —
Model
Sözel
Bağımsız
Girdi kaydet

Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.

• Hece ayırma çalışması → + (x / +)
• Sesli okuma — tekrarlı → 2 (0-3)
• Görsel dikkat eşleme → Evet (Evet / Hayır)
~~~~

### SUP-LEX-DOM-uzman-nav-katalog

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Etkinlik ve hedef davranış kataloğu
36 / 36 etkinlik · DEP 24 · BGM 12
Tümü (36)
DEP-2026 (24)
BGM-12 (12)
Tümü
Öğrenmeye Destek
Dil ve İletişim
Okuma ve Yazma
Erken Matematik
Matematik
Sosyal Etkileşim
Yeni etkinlik ekle · kayıt bu cihazda saklanır
DEP-2026
BGM-12
M1 · Öğrenmeye Destek
M2 · Dil ve İletişim
M3 · Okuma ve Yazma
M4 · Erken Matematik
M5 · Matematik
M6 · Sosyal Etkileşim
Ekle
Varsayılana sıfırla
Hece ayırma çalışması
3.1.2
Okuma ve Yazma · DEP
İpucu kademesi: Sözel ipucu → model → bağımsız
Malzeme: hece kartları · çalışma yaprağı
Düzenle
Sil
Sesli okuma — tekrarlı
3.3.1
Okuma ve Yazma · DEP
İpucu kademesi: Eşli okuma → bağımsız
Malzeme: kısa metin · kronometre
Düzenle
Sil
Görsel dikkat eşleme
1.1.3
Öğrenmeye Destek · DEP
İpucu kademesi: İşaret → sözel → bağımsız
Malzeme: eşleme kartları
Düzenle
Sil
İşitsel bellek dizisi
1.2.1
Öğrenmeye Destek · DEP
İpucu kademesi: Model → gecikmeli model → bağımsız
Malzeme: ses kartları
Düzenle
Sil
Sözcük dağarcığı — nesne adlandırma
2.2.1
Dil ve İletişim · DEP
İpucu kademesi: Fiziksel ipucu → sözel → bağımsız
Malzeme: nesne resimleri
Düzenle
Sil
Nesne niteliği ayırt etme
4.1.2
Erken Matematik · DEP
İpucu kademesi: Model → kısmi ipucu → bağımsız
Malzeme: blok seti
Düzenle
Sil
Ritmik sayma (100 içinde)
5.1.4
Matematik · DEP
İpucu kademesi: Birlikte sayma → bağımsız
Malzeme: sayı doğrusu
Düzenle
Sil
Sıra alma ve bekleme
6.2.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → sözel hatırlatma → bağımsız
Malzeme: sıra kartı · kum saati
Düzenle
Sil
Sürdürülebilir dikkat — nesne takibi
1.3.2
Öğrenmeye Destek · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: renkli toplar · tepsi
Düzenle
Sil
Yönerge izleme (2 adımlı)
1.4.1
Öğrenmeye Destek · DEP
İpucu kademesi: Fiziksel rehber → sözel → bağımsız
Malzeme: yönerge kartları
Düzenle
Sil
Dinlediğini anlama — kısa öykü
2.1.3
Dil ve İletişim · DEP
İpucu kademesi: Sözel ipucu → soru-cevap → bağımsız
Malzeme: öykü kartı · soru listesi
Düzenle
Sil
Sözel ifade — cümle kurma
2.3.2
Dil ve İletişim · DEP
İpucu kademesi: Model cümle → tamamlama → bağımsız
Malzeme: kelime kartları
Düzenle
Sil
Karşılıklı konuşma sürdürme
2.4.1
Dil ve İletişim · DEP
İpucu kademesi: Sözel başlatma → sıra alma → bağımsız
Malzeme: konu kartları · kum saati
Düzenle
Sil
Harf-ses eşleme
3.2.1
Okuma ve Yazma · DEP
İpucu kademesi: Model → eşleme → bağımsız
Malzeme: harf kartları · ses kutusu
Düzenle
Sil
Yazma — harf dikte
3.4.2
Okuma ve Yazma · DEP
İpucu kademesi: Noktalı iz → kopya → bağımsız
Malzeme: dikte yaprağı · kalem
Düzenle
Sil
Gruplama / sınıflama
4.2.3
Erken Matematik · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: sınıflama kutuları · nesneler
Düzenle
Sil
Birebir eşleştirme
4.3.1
Erken Matematik · DEP
İpucu kademesi: Fiziksel rehber → bağımsız
Malzeme: eş kartları
Düzenle
Sil
Sıralama (büyük-küçük)
4.4.2
Erken Matematik · DEP
İpucu kademesi: Model → deneme-yanılma → bağımsız
Malzeme: sıralama şeridi
Düzenle
Sil
Sayı doğrusu ile toplama
5.2.2
Matematik · DEP
İpucu kademesi: Model → rehberli → bağımsız
Malzeme: sayı doğrusu · pul
Düzenle
Sil
Çıkarma (nesne ile)
5.2.4
Matematik · DEP
İpucu kademesi: Nesne desteği → zihinden
Malzeme: sayma pulları
Düzenle
Sil
Günlük yaşam problemi kurma
5.3.1
Matematik · DEP
İpucu kademesi: Sözel senaryo → model → bağımsız
Malzeme: problem kartları
Düzenle
Sil
Duygu tanıma
6.1.2
Sosyal Etkileşim · DEP
İpucu kademesi: Görsel ipucu → eşleme → bağımsız
Malzeme: duygu kartları
Düzenle
Sil
İş birliği oyunu
6.3.1
Sosyal Etkileşim · DEP
İpucu kademesi: Eşli oyun → sıra alma → bağımsız
Malzeme: kutu oyunu
Düzenle
Sil
Kurala uyma (oyun)
6.3.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → hatırlatma → bağımsız
Malzeme: kural kartı
Düzenle
Sil
BGM — Ses Merdiveni (Fonolojik Eşleme) BGM
BGM-EQ-01
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: merdiven şeması · ses kartları · kum saati
Düzenle
Sil
BGM — Ses Birimi Ayırt Etme (SBA Turu) BGM
BGM-EQ-02
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: ekran (SBA) · ses kartları
Düzenle
Sil
BGM — Hece ve Parçalar (El Çırparak Heceleme) BGM
BGM-EQ-03
BGM-12 · BGM
İpucu kademesi: Model (uzman bölür) → sözel → bağımsız
Malzeme: hece kartları · parçalama şeridi
Düzenle
Sil
BGM — Harf Tanıma ve Çizim (b/d-l İzleme) BGM
BGM-EQ-04
BGM-12 · BGM
İpucu kademesi: Fiziksel izleme → model → sözel
Malzeme: büyük puntolu sayfa · harf kartları
Düzenle
Sil
BGM — Söyleneni Yaz (Hata Sınıfı ile) BGM
BGM-EQ-05
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: yazım yaprağı · hata sınıfı kartları
Düzenle
Sil
BGM — Akıcı Okuma (Tekrarlı + M-4) BGM
BGM-EQ-06
BGM-12 · BGM
İpucu kademesi: Eşli okuma → tek başına
Malzeme: hedef metin · süre sayacı · M-4 formu
Düzenle
Sil
BGM — Sözcük Çantası (Günün 5 Sözcüğü) BGM
BGM-EQ-07
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: sözcük kartları (5) · çanta görseli
Düzenle
Sil
BGM — Anlama Kartı (Okudunu Söyle) BGM
BGM-EQ-08
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: kısa metin kartı · anlama kartları (3)
Düzenle
Sil
BGM — Sayı Blokları (Çokluk + Karıştırma Çifti) BGM
BGM-EQ-09
BGM-12 · BGM
İpucu kademesi: Model → isaret → bağımsız
Malzeme: sayı blokları · sayı kartları
Düzenle
Sil
BGM — Süre Algısı (Kum Saati Tahmini) BGM
BGM-EQ-10
BGM-12 · BGM
İpucu kademesi: Görsel sayaç açık → yarı kapalı → kapalı
Malzeme: kum saati · tahmin kartı
Düzenle
Sil
BGM — Transfer ve Serbest Okuma BGM
BGM-EQ-11
BGM-12 · BGM
İpucu kademesi: Uzman yanımda → aynı odada → ayrı
Malzeme: serbest okuma metinleri · transfer kartı
Düzenle
Sil
BGM — Okuma Özerkliği (Kendi Planım) BGM
BGM-EQ-12
BGM-12 · BGM
İpucu kademesi: İstek üzerine → yok
Malzeme: 3 kutulu plan kartı · çocuğun kendi kitabı
Düzenle
Sil
Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.
~~~~

### SUP-LEX-DOM-uzman-nav-cizelge

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz
Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil
DEP saat-izleri — girdilerden türetilmiş (K-571/A1)
YASA-2 deseni: elle çizilmez
Dosya	Tamamlanan oturum	Toplam süre	DEP girdisi
ÖĞR-4417	1	40 dk	3
ÖĞR-2903	0	0 dk	0

Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).

İzleme çizelgesi
girdilerden türetildi
Tümü
DEP-2026
BGM-12 (0)
+
2
Evet

Toplam girdi: 3 · Hedefe ulaşılan: 2

Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.

Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.

Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.
~~~~

### SUP-LEX-DOM-uzman-nav-rapor

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-LEX-DOM-uzman-nav-hizalama

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
MEB destek eğitim programı modülleriyle hizalı çıktı
M1 · Öğrenmeye Destek (150 sa)
M2 · Dil ve İletişim (150 sa)
M3 · Okuma ve Yazma (300 sa)
M4 · Erken Matematik (200 sa)
M5 · Matematik (200 sa)
M6 · Sosyal Etkileşim (100 sa)

Seçili: Okuma ve Yazma — 6 bölüm · önerilen 300 ders saati

Toplam program: 1100 ders saati · 6 modül · giriş yalnız ELLE yapılır.

Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.

Resmî tavan (ÖEK Yön. md.24/4): aylık 12 bireysel · 4 grup · haftalık 4/2 · günlük toplam 3 saat.

Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
~~~~

### SUP-LEX-DOM-uzman-nav-bgm

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Bilişsel Geliştirme Modülleri (BGM-12)
12 modül · menü
İki katman. Okuma menüsü (12), DEP-2021'in yerine geçmez. DEP = BEP/RAM saat hizası; menü = okuma/fonolojik içerik. Uzman ikisinden de seçer.
Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. Persona sarmalı dayatılmaz.
TASLAK. Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez. Tam kartlar: LEXIVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md.
ÖĞR-4417
ÖĞR-2903

Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): EQ-01 → EQ-02 → EQ-05

Grup I — fonolojik temel (sıra değil)
EQ-01 · Ses Merdiveni
Fonolojik eşleme · Fonolojik farkındalık
çekirdek
Programdan çıkar
Kart
Tanım: Merdiven ardıl sırasıyla (sözcük→uyak→hece→sesbirimi) basamak basamak ilerleme pratiği (DEP 3.2.1: önce eşleme).
Amaç: Başlangıç-sesi farkındalığını merdiven üstünde izlenebilir kılmak; uzman hedefi BEP satırına taşır.
Ölçüm: Basamak isabeti (0–3) · eşleme/ayırt etme tutarlılığı. Bant/eşik ve tanı YOK (K-02).
Etkinlik: Merdiven şeması üzerinde 2 örnek eşleme (model), sonra 6 sözcük bağımsız tur. (5–7 dk)
Malzeme: merdiven şeması · ses kartları (6) · kum saati · İpucu: model → sözel ("ilk sesi yakala") → bağımsız · Girdi: 0-3
Ödev: Evde 5 sözcüğün başlangıç sesini eşleştirin (kavram; resmî form metni değil). Puanlanmaz.
Önlem: Masada yalnız merdiven şeması ve ses kartları; ekran görüş alanında olmasın.
Öneri: Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.
DEP köprüsü: M3 — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)
Dayanak: 2021 DEP 3.1/3.2.1 ardıl sıra · MEB Ses Farkındalık Öğretmen Kılavuzu (yapı atfı; K-08)
EQ-02 · Ses Birimi Ayırt Etme
Harf seçiciliği · Fonolojik farkındalık
çekirdek
Programdan çıkar
Kart
EQ-03 · Hece ve Parçalar
Sözcüğü bölme · Fonolojik parçalama
Programa al
Kart
EQ-04 · Harf Tanıma ve Çizim
b/d-l izleme · Görsel-tanım / yazım
Programa al
Kart
Grup II — okuma/yazma/matematik (sıra değil)
EQ-05 · Söyleneni Yaz
İşitsel yazım · Yazma
çekirdek
Programdan çıkar
Kart
EQ-06 · Akıcı Okuma
Tekrarlı okuma · Akıcılık (D-L2)
çekirdek
Programa al
Kart
EQ-07 · Sözcük Çantası
Kelime dağarcığı · Sözcük dağarcığı (DEP M2.2)
Programa al
Kart
EQ-08 · Anlama Kartı
Okudunu söyle · Anlama
Programa al
Kart
EQ-09 · Sayı Blokları
Çokluk ve karıştırma · Matematik (D-L4)
Programa al
Kart
EQ-10 · Süre Algısı
Süre tahmini · Süre tahmini (seans içi)
Programa al
Kart
Grup III — aktarım ve özerklik (sıra değil)
EQ-11 · Transfer ve Serbest Okuma
Yeni metine taşıma · Aktarım (D-L7)
Programa al
Kart
EQ-12 · Okuma Özerkliği
Dış iskeleti solma · Üstbiliş / otonomi
Programa al
Kart
LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.
~~~~

### SUP-LEX-DOM-uzman-nav-rambep

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
RAM raporu ve kayıt hattı
ÖĞR-4417
ÖĞR-2903
Kayıt hattı: (a) Ücreti Bakanlıkça karşılanan
RAM raporu: ZORUNLU (rapor + ÖEDK planı + BKDS onamı) · Planlama: ÖEDK eğitim planı ekseninde
Rapor no
RAM-2025/1184
Rapor tarihi
2025-10-14
Geçerlilik
2026-10-14
EDİF durumu
İlk İnceleme tamamlandı (e-Rehberlik)
Sonraki izleme
2026-09-30
Portfolyo
Hazır
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
Resmî form ailesi — hangi girdi neyi besler
DEP-2026 EK-1…EK-7
Ek	Form	Doldurma anı	Supporta katkısı
EK-1	Ölçüt Bağımlı Test (ÖBT)	ilk / ara / son değ.	Tekrar ve deneme sayısı → Ölçüt alanı
EK-2	Kontrol Listesi	ilk / ara / son değ.	Evet/Hayır girdileri → Açıklamalar sütunu
EK-3	Dereceli Puanlama Anahtarı	değerlendirme	0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)
EK-4	Performans Kayıt Formu	her modülün başı ve sonu	x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)
EK-5	BEP Gelişimi İzleme Özet Formu	süreç + yıl sonu	Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler
EK-6	Portfolyo Kontrol Listesi	modül sonu / yıl sonu	Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)
EK-7	Portfolyo Dereceli Puanlama Anahtarı	portfolyo değ.	—
Sınır: Supporta bu formları DOLDURMAZ. x/+ işaretini, performans düzeyini ve “ulaşılamama nedenini” uzman belirler; portfolyo RAM onayına gider. Model: Supporta kanıt üretir · uzman karar verir · RAM onaylar.
Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
~~~~

### SUP-LEX-DOM-uzman-nav-evodev

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Ev çalışmaları ve seans dışı görevler
kim · ne · ne zaman
Mutfakta hece avı (5 nesne)
ÖĞR-4417 · Veli · Hafta içi 3 gün · 10 dk
Not: Çocuk istekliydi; 4 nesne bağımsız heceledi.
verildi
yapıldı
yapılmadı
Gazete başlığı okuma
ÖĞR-4417 · Veli · Hafta sonu · 1 kez
verildi
yapıldı
yapılmadı
Sayı kartlarıyla eşleme
ÖĞR-2903 · Veli · Hafta içi 2 gün
Not: Aile yoğunluk bildirdi; süre kısaltıldı.
verildi
yapıldı
yapılmadı
Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz.
Seans başı izleme ritüeli
Ev çalışması gözden geçirilir (yapıldı/yapılmadı — yargı değil gözlem).
Bir önceki oturumun hedef davranışı hatırlatılır.
Bugünün etkinliği ve ipucu kademesi belirlenir.
Oturum sonunda veli için tek satırlık jargonsuz not yazılır.
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-LEX-DOM-uzman-nav-aile

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görse…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-LEX-DOM-uzman-nav-ayarlar

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Şerh kütüphanesi ve roller
OTURUM
Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
CİZELGE
Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.
RAPOR
TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).
AİLE
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
HİZALİ
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
K02
LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).

Kapsam dışı (bilinçli sınırlar)
Devam/yoklama takibi — BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.
Ödeme · fatura · idari-mali işleyiş — K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.
Resmî form üretimi — K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.
Yerel veri

Girdiler, oturum durumları ve rapor onayları yalnız bu cihazda saklanır (KVKK yerel-önce). Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: 7

Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
~~~~

### SUP-LEX-DOM-uzman-rapor-yz-oneri

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi. — YZ EĞİTİMSEL DESTEK ÖNERİSİ — (Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı) Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir. ⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

YZ ÖNERİSİ KATMANI — uzman onayı gerektirir
✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-LEX-DOM-uzman-rapor-reddet

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi. — YZ EĞİTİMSEL DESTEK ÖNERİSİ — (Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı) Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir. ⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır. — YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ — Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

YZ ÖNERİSİ KATMANI — uzman onayı gerektirir
✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-LEX-DOM-uzman-rapor-onayli

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYLI
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi. — YZ EĞİTİMSEL DESTEK ÖNERİSİ — (Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı) Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir. ⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır. — YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ — Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
Dışa aktar (2 kopya)
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=True, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-LEX-DOM-uzman-aile-A

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görse…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-LEX-DOM-uzman-aile-sekme-A

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görse…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-LEX-DOM-uzman-aile-sekme-B

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Uzman / Eğitimci · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Analize Göre Aile Görevi (Uzman Seçer)
İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu
Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02).
Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme)
Tetik: Çizelgede kopma > eşik
Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev
Tetik: Ev Çalışmaları “yapılmadı” >2
Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme
Tetik: Girdi “0/3” yoğun
[UZMAN DOLDURUR — K-02]
Gözlem/Rapor bulgusu (tarihli, sayılabilir): ...
Aileye önerilen tek görev (1 cümle, bağlamlı): ...
İpucu kademesi (model/sözel/bağımsız): ...
Kayıt biçimi (tik/süre): ...
Sonraki izleme tarihi: ...

Aileye görev örneği: Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.
Ölçüm: Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.
Şablonu Yazdır

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-LEX-DOM-yonetici-rol-secimi

~~~~text
S
LEXIVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)

Özel eğitim merkezi uzman kokpiti · v2.10.0

Devam etmek için rolünüzü seçin.

Yönetici
Tüm dosyalar · rapor onayı · dışa aktarma
Uzman / Eğitimci
Kendi dosyaları · oturum · girdi · rapor taslağı

Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
~~~~

### SUP-LEX-DOM-yonetici-nav-pano

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif

Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.

T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)
2026-09-10 10:00 — ÖĞR-4417 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
2026-09-03 10:00 — ÖĞR-2903 (40 dk)
T1 Merkezi
T2 Okul Bekleniyor
Onay Bekleyen Raporlar (Human-Accountable AI)
4
• Seans Özeti — 03.09.2026
• Dönem Sonu Değerlendirme — 2026 Güz
• BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
• RAM İzleme Paketi Hazırlığı

YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).
~~~~

### SUP-LEX-DOM-yonetici-nav-dosyalar

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Dosya listesi
ÖĞR-4417
ÖĞR-2903
Dosya kartı — ÖĞR-4417
Ad (maskeli)
Öğrenci A. (2. Sınıf)
Doğum
2018-04-12
Okul / Sınıf
Atatürk İlkokulu / 2-B
Devamsızlık
Son ayda 2 gün
Veli
Veli A. · 05xx xxx 41 17
Rıza kaydı
2026-08-20
Geçmiş BEP
RAM eğitsel değerlendirme mevcut (2025)
Program kartı
Seans sayısı
24
Sıklık
Haftada 1 (40 dk)
Aile bileşeni
Var
RAM rapor ref.
RAM-2025/1184
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-LEX-DOM-yonetici-nav-takvim

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Oturum takvimi
2026-09-03 haftası
Çakışma: 2026-09-03 10:00 UZM-1 (KC12)
Tarih	Saat	Dosya	Uzman	Durum
2026-09-03	10:00	ÖĞR-4417	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

2026-09-03	10:00	ÖĞR-2903	UZM-1	
planlandı
tamamlandı
iptal
gelmedi

Durumlar: planlandı · tamamlandı · iptal · gelmedi · değişiklikler bu cihazda saklanır.

Veli görüşme-randevu defteri (K-571/A2)
hatırlatma gönderilmez — K-334
Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
Tarih
Konu
Deftere ekle

Defter boş — ilk görüşme kaydını ekleyin.

Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).
~~~~

### SUP-LEX-DOM-yonetici-nav-oturum

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Oturum kartı — OT-101

Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı

Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)

Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
ⓘ
Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)
Bu oturumda seçili BGM modülleri
ÖĞR-4417 · sıra uzmanın
EQ-01 · Ses Merdiveni BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M3
EQ-02 · Ses Birimi Ayırt Etme BGM
5–7 dk · girdi: 0-3 · DEP köprüsü M3
EQ-05 · Söyleneni Yaz BGM
6 dk · girdi: x / + · DEP köprüsü M3

Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez.

Hızlı girdi paneli
YASA-1 etkin
Etkinlik *zorunlu
— etkinlik seçin —
Hece ayırma çalışması (3.1.2)
Sesli okuma — tekrarlı (3.3.1)
Görsel dikkat eşleme (1.1.3)
İşitsel bellek dizisi (1.2.1)
Sözcük dağarcığı — nesne adlandırma (2.2.1)
Nesne niteliği ayırt etme (4.1.2)
Ritmik sayma (100 içinde) (5.1.4)
Sıra alma ve bekleme (6.2.3)
Sürdürülebilir dikkat — nesne takibi (1.3.2)
Yönerge izleme (2 adımlı) (1.4.1)
Dinlediğini anlama — kısa öykü (2.1.3)
Sözel ifade — cümle kurma (2.3.2)
Karşılıklı konuşma sürdürme (2.4.1)
Harf-ses eşleme (3.2.1)
Yazma — harf dikte (3.4.2)
Gruplama / sınıflama (4.2.3)
Birebir eşleştirme (4.3.1)
Sıralama (büyük-küçük) (4.4.2)
Sayı doğrusu ile toplama (5.2.2)
Çıkarma (nesne ile) (5.2.4)
Günlük yaşam problemi kurma (5.3.1)
Duygu tanıma (6.1.2)
İş birliği oyunu (6.3.1)
Kurala uyma (oyun) (6.3.3)
BGM — Ses Merdiveni (Fonolojik Eşleme) (BGM-EQ-01)
BGM — Ses Birimi Ayırt Etme (SBA Turu) (BGM-EQ-02)
BGM — Hece ve Parçalar (El Çırparak Heceleme) (BGM-EQ-03)
BGM — Harf Tanıma ve Çizim (b/d-l İzleme) (BGM-EQ-04)
BGM — Söyleneni Yaz (Hata Sınıfı ile) (BGM-EQ-05)
BGM — Akıcı Okuma (Tekrarlı + M-4) (BGM-EQ-06)
BGM — Sözcük Çantası (Günün 5 Sözcüğü) (BGM-EQ-07)
BGM — Anlama Kartı (Okudunu Söyle) (BGM-EQ-08)
BGM — Sayı Blokları (Çokluk + Karıştırma Çifti) (BGM-EQ-09)
BGM — Süre Algısı (Kum Saati Tahmini) (BGM-EQ-10)
BGM — Transfer ve Serbest Okuma (BGM-EQ-11)
BGM — Okuma Özerkliği (Kendi Planım) (BGM-EQ-12)
[BGM] EQ-01 · Ses Merdiveni
[BGM] EQ-02 · Ses Birimi Ayırt Etme
[BGM] EQ-05 · Söyleneni Yaz
Kodlama
x / +
0-3
Evet / Hayır
Değer
Gözlenen ipucu-kademesi (K-571/A4)
— seçilmeyebilir —
Model
Sözel
Bağımsız
Girdi kaydet

Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.

• Hece ayırma çalışması → + (x / +)
• Sesli okuma — tekrarlı → 2 (0-3)
• Görsel dikkat eşleme → Evet (Evet / Hayır)
~~~~

### SUP-LEX-DOM-yonetici-nav-katalog

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Etkinlik ve hedef davranış kataloğu
36 / 36 etkinlik · DEP 24 · BGM 12
Tümü (36)
DEP-2026 (24)
BGM-12 (12)
Tümü
Öğrenmeye Destek
Dil ve İletişim
Okuma ve Yazma
Erken Matematik
Matematik
Sosyal Etkileşim
Yeni etkinlik ekle · kayıt bu cihazda saklanır
DEP-2026
BGM-12
M1 · Öğrenmeye Destek
M2 · Dil ve İletişim
M3 · Okuma ve Yazma
M4 · Erken Matematik
M5 · Matematik
M6 · Sosyal Etkileşim
Ekle
Varsayılana sıfırla
Hece ayırma çalışması
3.1.2
Okuma ve Yazma · DEP
İpucu kademesi: Sözel ipucu → model → bağımsız
Malzeme: hece kartları · çalışma yaprağı
Düzenle
Sil
Sesli okuma — tekrarlı
3.3.1
Okuma ve Yazma · DEP
İpucu kademesi: Eşli okuma → bağımsız
Malzeme: kısa metin · kronometre
Düzenle
Sil
Görsel dikkat eşleme
1.1.3
Öğrenmeye Destek · DEP
İpucu kademesi: İşaret → sözel → bağımsız
Malzeme: eşleme kartları
Düzenle
Sil
İşitsel bellek dizisi
1.2.1
Öğrenmeye Destek · DEP
İpucu kademesi: Model → gecikmeli model → bağımsız
Malzeme: ses kartları
Düzenle
Sil
Sözcük dağarcığı — nesne adlandırma
2.2.1
Dil ve İletişim · DEP
İpucu kademesi: Fiziksel ipucu → sözel → bağımsız
Malzeme: nesne resimleri
Düzenle
Sil
Nesne niteliği ayırt etme
4.1.2
Erken Matematik · DEP
İpucu kademesi: Model → kısmi ipucu → bağımsız
Malzeme: blok seti
Düzenle
Sil
Ritmik sayma (100 içinde)
5.1.4
Matematik · DEP
İpucu kademesi: Birlikte sayma → bağımsız
Malzeme: sayı doğrusu
Düzenle
Sil
Sıra alma ve bekleme
6.2.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → sözel hatırlatma → bağımsız
Malzeme: sıra kartı · kum saati
Düzenle
Sil
Sürdürülebilir dikkat — nesne takibi
1.3.2
Öğrenmeye Destek · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: renkli toplar · tepsi
Düzenle
Sil
Yönerge izleme (2 adımlı)
1.4.1
Öğrenmeye Destek · DEP
İpucu kademesi: Fiziksel rehber → sözel → bağımsız
Malzeme: yönerge kartları
Düzenle
Sil
Dinlediğini anlama — kısa öykü
2.1.3
Dil ve İletişim · DEP
İpucu kademesi: Sözel ipucu → soru-cevap → bağımsız
Malzeme: öykü kartı · soru listesi
Düzenle
Sil
Sözel ifade — cümle kurma
2.3.2
Dil ve İletişim · DEP
İpucu kademesi: Model cümle → tamamlama → bağımsız
Malzeme: kelime kartları
Düzenle
Sil
Karşılıklı konuşma sürdürme
2.4.1
Dil ve İletişim · DEP
İpucu kademesi: Sözel başlatma → sıra alma → bağımsız
Malzeme: konu kartları · kum saati
Düzenle
Sil
Harf-ses eşleme
3.2.1
Okuma ve Yazma · DEP
İpucu kademesi: Model → eşleme → bağımsız
Malzeme: harf kartları · ses kutusu
Düzenle
Sil
Yazma — harf dikte
3.4.2
Okuma ve Yazma · DEP
İpucu kademesi: Noktalı iz → kopya → bağımsız
Malzeme: dikte yaprağı · kalem
Düzenle
Sil
Gruplama / sınıflama
4.2.3
Erken Matematik · DEP
İpucu kademesi: Model → sözel ipucu → bağımsız
Malzeme: sınıflama kutuları · nesneler
Düzenle
Sil
Birebir eşleştirme
4.3.1
Erken Matematik · DEP
İpucu kademesi: Fiziksel rehber → bağımsız
Malzeme: eş kartları
Düzenle
Sil
Sıralama (büyük-küçük)
4.4.2
Erken Matematik · DEP
İpucu kademesi: Model → deneme-yanılma → bağımsız
Malzeme: sıralama şeridi
Düzenle
Sil
Sayı doğrusu ile toplama
5.2.2
Matematik · DEP
İpucu kademesi: Model → rehberli → bağımsız
Malzeme: sayı doğrusu · pul
Düzenle
Sil
Çıkarma (nesne ile)
5.2.4
Matematik · DEP
İpucu kademesi: Nesne desteği → zihinden
Malzeme: sayma pulları
Düzenle
Sil
Günlük yaşam problemi kurma
5.3.1
Matematik · DEP
İpucu kademesi: Sözel senaryo → model → bağımsız
Malzeme: problem kartları
Düzenle
Sil
Duygu tanıma
6.1.2
Sosyal Etkileşim · DEP
İpucu kademesi: Görsel ipucu → eşleme → bağımsız
Malzeme: duygu kartları
Düzenle
Sil
İş birliği oyunu
6.3.1
Sosyal Etkileşim · DEP
İpucu kademesi: Eşli oyun → sıra alma → bağımsız
Malzeme: kutu oyunu
Düzenle
Sil
Kurala uyma (oyun)
6.3.3
Sosyal Etkileşim · DEP
İpucu kademesi: Model → hatırlatma → bağımsız
Malzeme: kural kartı
Düzenle
Sil
BGM — Ses Merdiveni (Fonolojik Eşleme) BGM
BGM-EQ-01
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: merdiven şeması · ses kartları · kum saati
Düzenle
Sil
BGM — Ses Birimi Ayırt Etme (SBA Turu) BGM
BGM-EQ-02
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: ekran (SBA) · ses kartları
Düzenle
Sil
BGM — Hece ve Parçalar (El Çırparak Heceleme) BGM
BGM-EQ-03
BGM-12 · BGM
İpucu kademesi: Model (uzman bölür) → sözel → bağımsız
Malzeme: hece kartları · parçalama şeridi
Düzenle
Sil
BGM — Harf Tanıma ve Çizim (b/d-l İzleme) BGM
BGM-EQ-04
BGM-12 · BGM
İpucu kademesi: Fiziksel izleme → model → sözel
Malzeme: büyük puntolu sayfa · harf kartları
Düzenle
Sil
BGM — Söyleneni Yaz (Hata Sınıfı ile) BGM
BGM-EQ-05
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: yazım yaprağı · hata sınıfı kartları
Düzenle
Sil
BGM — Akıcı Okuma (Tekrarlı + M-4) BGM
BGM-EQ-06
BGM-12 · BGM
İpucu kademesi: Eşli okuma → tek başına
Malzeme: hedef metin · süre sayacı · M-4 formu
Düzenle
Sil
BGM — Sözcük Çantası (Günün 5 Sözcüğü) BGM
BGM-EQ-07
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: sözcük kartları (5) · çanta görseli
Düzenle
Sil
BGM — Anlama Kartı (Okudunu Söyle) BGM
BGM-EQ-08
BGM-12 · BGM
İpucu kademesi: Model → sözel → bağımsız
Malzeme: kısa metin kartı · anlama kartları (3)
Düzenle
Sil
BGM — Sayı Blokları (Çokluk + Karıştırma Çifti) BGM
BGM-EQ-09
BGM-12 · BGM
İpucu kademesi: Model → isaret → bağımsız
Malzeme: sayı blokları · sayı kartları
Düzenle
Sil
BGM — Süre Algısı (Kum Saati Tahmini) BGM
BGM-EQ-10
BGM-12 · BGM
İpucu kademesi: Görsel sayaç açık → yarı kapalı → kapalı
Malzeme: kum saati · tahmin kartı
Düzenle
Sil
BGM — Transfer ve Serbest Okuma BGM
BGM-EQ-11
BGM-12 · BGM
İpucu kademesi: Uzman yanımda → aynı odada → ayrı
Malzeme: serbest okuma metinleri · transfer kartı
Düzenle
Sil
BGM — Okuma Özerkliği (Kendi Planım) BGM
BGM-EQ-12
BGM-12 · BGM
İpucu kademesi: İstek üzerine → yok
Malzeme: 3 kutulu plan kartı · çocuğun kendi kitabı
Düzenle
Sil
Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.
~~~~

### SUP-LEX-DOM-yonetici-nav-cizelge

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz
Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil
DEP saat-izleri — girdilerden türetilmiş (K-571/A1)
YASA-2 deseni: elle çizilmez
Dosya	Tamamlanan oturum	Toplam süre	DEP girdisi
ÖĞR-4417	1	40 dk	3
ÖĞR-2903	0	0 dk	0

Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).

İzleme çizelgesi
girdilerden türetildi
Tümü
DEP-2026
BGM-12 (0)
+
2
Evet

Toplam girdi: 3 · Hedefe ulaşılan: 2

Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.

Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.

Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.
~~~~

### SUP-LEX-DOM-yonetici-nav-rapor

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYI BEKLİYOR
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=False, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

### SUP-LEX-DOM-yonetici-nav-hizalama

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
MEB destek eğitim programı modülleriyle hizalı çıktı
M1 · Öğrenmeye Destek (150 sa)
M2 · Dil ve İletişim (150 sa)
M3 · Okuma ve Yazma (300 sa)
M4 · Erken Matematik (200 sa)
M5 · Matematik (200 sa)
M6 · Sosyal Etkileşim (100 sa)

Seçili: Okuma ve Yazma — 6 bölüm · önerilen 300 ders saati

Toplam program: 1100 ders saati · 6 modül · giriş yalnız ELLE yapılır.

Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.

Resmî tavan (ÖEK Yön. md.24/4): aylık 12 bireysel · 4 grup · haftalık 4/2 · günlük toplam 3 saat.

Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
~~~~

### SUP-LEX-DOM-yonetici-nav-bgm

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Bilişsel Geliştirme Modülleri (BGM-12)
12 modül · menü
İki katman. Okuma menüsü (12), DEP-2021'in yerine geçmez. DEP = BEP/RAM saat hizası; menü = okuma/fonolojik içerik. Uzman ikisinden de seçer.
Modül seçimi serbesttir. Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. Persona sarmalı dayatılmaz.
TASLAK. Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez. Tam kartlar: LEXIVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md.
ÖĞR-4417
ÖĞR-2903

Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): EQ-01 → EQ-02 → EQ-05

Grup I — fonolojik temel (sıra değil)
EQ-01 · Ses Merdiveni
Fonolojik eşleme · Fonolojik farkındalık
çekirdek
Programdan çıkar
Kart
Tanım: Merdiven ardıl sırasıyla (sözcük→uyak→hece→sesbirimi) basamak basamak ilerleme pratiği (DEP 3.2.1: önce eşleme).
Amaç: Başlangıç-sesi farkındalığını merdiven üstünde izlenebilir kılmak; uzman hedefi BEP satırına taşır.
Ölçüm: Basamak isabeti (0–3) · eşleme/ayırt etme tutarlılığı. Bant/eşik ve tanı YOK (K-02).
Etkinlik: Merdiven şeması üzerinde 2 örnek eşleme (model), sonra 6 sözcük bağımsız tur. (5–7 dk)
Malzeme: merdiven şeması · ses kartları (6) · kum saati · İpucu: model → sözel ("ilk sesi yakala") → bağımsız · Girdi: 0-3
Ödev: Evde 5 sözcüğün başlangıç sesini eşleştirin (kavram; resmî form metni değil). Puanlanmaz.
Önlem: Masada yalnız merdiven şeması ve ses kartları; ekran görüş alanında olmasın.
Öneri: Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.
DEP köprüsü: M3 — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)
Dayanak: 2021 DEP 3.1/3.2.1 ardıl sıra · MEB Ses Farkındalık Öğretmen Kılavuzu (yapı atfı; K-08)
EQ-02 · Ses Birimi Ayırt Etme
Harf seçiciliği · Fonolojik farkındalık
çekirdek
Programdan çıkar
Kart
EQ-03 · Hece ve Parçalar
Sözcüğü bölme · Fonolojik parçalama
Programa al
Kart
EQ-04 · Harf Tanıma ve Çizim
b/d-l izleme · Görsel-tanım / yazım
Programa al
Kart
Grup II — okuma/yazma/matematik (sıra değil)
EQ-05 · Söyleneni Yaz
İşitsel yazım · Yazma
çekirdek
Programdan çıkar
Kart
EQ-06 · Akıcı Okuma
Tekrarlı okuma · Akıcılık (D-L2)
çekirdek
Programa al
Kart
EQ-07 · Sözcük Çantası
Kelime dağarcığı · Sözcük dağarcığı (DEP M2.2)
Programa al
Kart
EQ-08 · Anlama Kartı
Okudunu söyle · Anlama
Programa al
Kart
EQ-09 · Sayı Blokları
Çokluk ve karıştırma · Matematik (D-L4)
Programa al
Kart
EQ-10 · Süre Algısı
Süre tahmini · Süre tahmini (seans içi)
Programa al
Kart
Grup III — aktarım ve özerklik (sıra değil)
EQ-11 · Transfer ve Serbest Okuma
Yeni metine taşıma · Aktarım (D-L7)
Programa al
Kart
EQ-12 · Okuma Özerkliği
Dış iskeleti solma · Üstbiliş / otonomi
Programa al
Kart
LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.
~~~~

### SUP-LEX-DOM-yonetici-nav-rambep

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
RAM raporu ve kayıt hattı
ÖĞR-4417
ÖĞR-2903
Kayıt hattı: (a) Ücreti Bakanlıkça karşılanan
RAM raporu: ZORUNLU (rapor + ÖEDK planı + BKDS onamı) · Planlama: ÖEDK eğitim planı ekseninde
Rapor no
RAM-2025/1184
Rapor tarihi
2025-10-14
Geçerlilik
2026-10-14
EDİF durumu
İlk İnceleme tamamlandı (e-Rehberlik)
Sonraki izleme
2026-09-30
Portfolyo
Hazır
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
Resmî form ailesi — hangi girdi neyi besler
DEP-2026 EK-1…EK-7
Ek	Form	Doldurma anı	Supporta katkısı
EK-1	Ölçüt Bağımlı Test (ÖBT)	ilk / ara / son değ.	Tekrar ve deneme sayısı → Ölçüt alanı
EK-2	Kontrol Listesi	ilk / ara / son değ.	Evet/Hayır girdileri → Açıklamalar sütunu
EK-3	Dereceli Puanlama Anahtarı	değerlendirme	0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)
EK-4	Performans Kayıt Formu	her modülün başı ve sonu	x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)
EK-5	BEP Gelişimi İzleme Özet Formu	süreç + yıl sonu	Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler
EK-6	Portfolyo Kontrol Listesi	modül sonu / yıl sonu	Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)
EK-7	Portfolyo Dereceli Puanlama Anahtarı	portfolyo değ.	—
Sınır: Supporta bu formları DOLDURMAZ. x/+ işaretini, performans düzeyini ve “ulaşılamama nedenini” uzman belirler; portfolyo RAM onayına gider. Model: Supporta kanıt üretir · uzman karar verir · RAM onaylar.
Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
~~~~

### SUP-LEX-DOM-yonetici-nav-evodev

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Ev çalışmaları ve seans dışı görevler
kim · ne · ne zaman
Mutfakta hece avı (5 nesne)
ÖĞR-4417 · Veli · Hafta içi 3 gün · 10 dk
Not: Çocuk istekliydi; 4 nesne bağımsız heceledi.
verildi
yapıldı
yapılmadı
Gazete başlığı okuma
ÖĞR-4417 · Veli · Hafta sonu · 1 kez
verildi
yapıldı
yapılmadı
Sayı kartlarıyla eşleme
ÖĞR-2903 · Veli · Hafta içi 2 gün
Not: Aile yoğunluk bildirdi; süre kısaltıldı.
verildi
yapıldı
yapılmadı
Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz.
Seans başı izleme ritüeli
Ev çalışması gözden geçirilir (yapıldı/yapılmadı — yargı değil gözlem).
Bir önceki oturumun hedef davranışı hatırlatılır.
Bugünün etkinliği ve ipucu kademesi belirlenir.
Oturum sonunda veli için tek satırlık jargonsuz not yazılır.
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### SUP-LEX-DOM-yonetici-nav-aile

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Aile & Öğretmen İşbirliği

Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)
K-407 · 5+1 · TASLAK
ÖĞR-4417
ÖĞR-2903
A — Genel (5 mini-modül)
B — Analize Göre (uzman seçer)
Nasihat ve Kıyas Yok — Gözlem Dili
15 dk · Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili …
Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne
20 dk · Yazılı planla öngörülebilirlik sağlamak (Z-1).…
Görsel Ortam — Uyaran Yalıtımı
10 dk · Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görse…
İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge
10 dk · İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + …
Pekiştireç ve Kayıt — Hedef Davranış + İpucu
15 dk · Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 …
Nasihat ve Kıyas Yok — Gözlem Dili
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.
“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).
Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Yazdır / PDF
Kopyala

Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.

Bilgilendirme çıktısı

Yalnız onaylı raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).

Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
~~~~

### SUP-LEX-DOM-yonetici-nav-ayarlar

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Şerh kütüphanesi ve roller
OTURUM
Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.
CİZELGE
Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.
RAPOR
TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).
AİLE
Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
HİZALİ
Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.
K02
LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).

Kapsam dışı (bilinçli sınırlar)
Devam/yoklama takibi — BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.
Ödeme · fatura · idari-mali işleyiş — K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.
Resmî form üretimi — K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.
Yerel veri

Girdiler, oturum durumları ve rapor onayları yalnız bu cihazda saklanır (KVKK yerel-önce). Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: 7

Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
~~~~

### SUP-LEX-DOM-yonetici-rapor-onayli

~~~~text
S
LEXIVA Supporta™
Uzman Kokpiti · v2.10.0
Eğitmen Kürsüsü
Dosyalar
Takvim
Oturum Atölyesi
Etkinlik Kataloğu
İzleme Çizelgesi
Rapor Atölyesi
Program Hizalama
Bilişsel Geliştirme
RAM & BEP Takibi
Ev Çalışmaları
Aile & Öğretmen
Ayarlar
Rol: Yönetici · Sentetik demo verisi

LEXIVA Supporta: LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.

v2.10.0 · DEMO — jüri tanıtım
Seans özeti — Seans Özeti — 03.09.2026
UZMAN ONAYLI
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
Dışa aktar (2 kopya)
Aylık özet — Aylık Gelişim Özeti — Ağustos 2026
UZMAN ONAYLI
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
Dışa aktar (2 kopya)
Dönem sonu — Dönem Sonu Değerlendirme — 2026 Güz
UZMAN ONAYI BEKLİYOR
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
BEP ilerleme taslağı — BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık
UZMAN ONAYI BEKLİYOR
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
RAM izleme paketi — RAM İzleme Paketi Hazırlığı
UZMAN ONAYI BEKLİYOR
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
Human-Accountable AI (YZ Destek Asistanı)
Kanıtı İncele ve YZ Önerisi Al
Öneriyi Reddet ve Gerekçelendir

YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.

✓ Değişiklikleri Onayla ve İmzala
Dışa aktar (2 kopya)
Onaysız rapor dışa aktarılamaz.
Aile bilgilendirme — Aile Bilgilendirme Çıktısı — Eylül
UZMAN ONAYLI
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
Dışa aktar (2 kopya)
~~~~

Textarea 1, disabled=True, readOnly=False

~~~~text
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.
~~~~

Textarea 2, disabled=True, readOnly=False

~~~~text
Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.
~~~~

Textarea 3, disabled=False, readOnly=False

~~~~text
Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.
~~~~

Textarea 4, disabled=False, readOnly=False

~~~~text
Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.
~~~~

Textarea 5, disabled=False, readOnly=False

~~~~text
Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir.
~~~~

Textarea 6, disabled=True, readOnly=False

~~~~text
Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.
~~~~

## Yazdırma ve CSV çıktıları

Gerçek yazıcı kullanılmadı; metinler mevcut sentetik kayıtlarla üretildi.

### rapor / rol=uzman

~~~~text
Seans özeti — Seans Özeti — 03.09.2026
ONAYLI — Yönetici 2026-09-03
Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v2.10.0
~~~~

### aile-A / rol=uzman

~~~~text
Nasihat ve Kıyas Yok — Gözlem Dili — ÖĞR-4417
ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER
Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.

“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.
- “Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).
- Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).

Malzeme: A4 gözlem kartı, kalem
Yorum/değer yargısı yok — yalnızca gözlem.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v2.10.0 · Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### aile-B / rol=uzman

~~~~text
Analize Göre Aile Görevi (Uzman Seçer) — ÖĞR-4417
ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER
[UZMAN DOLDURUR — K-02]
Gözlem/Rapor bulgusu (tarihli, sayılabilir): ...
Aileye önerilen tek görev (1 cümle, bağlamlı): ...
İpucu kademesi (model/sözel/bağımsız): ...
Kayıt biçimi (tik/süre): ...
Sonraki izleme tarihi: ...


Görev: Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.
Ölçüm: Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.
Kopya 1/2 — Aile/Veli  |  Kopya 2/2 — Kurum arşivi · 2026-09-11 · Supporta v2.10.0 · Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).
~~~~

### CSV: R-1-seans.csv

~~~~csv
tur,baslik,durum,icerik
seans,"Seans Özeti — 03.09.2026",ONAYLI,"Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: 1 T1 seansı, 40 dk aktif izlem, 3 girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır."
~~~~

## AST kaynak adayları

ID kaynak anının satırına bağlıdır; JSX/template parçaları tek başına tam cümle değildir. Exact bağlam için ham dosya ve DOM birlikte okunur.

| ID | Dosya:satır | Tür | Ham parça (↵=satır sonu) | Görünürlük |
|---|---|---|---|---|
| SUP-LEX-0001 | `App.tsx:17` | JsxText | LEXIVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0002 | `App.tsx:18` | JsxText | Özel eğitim merkezi uzman kokpiti · v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0003 | `App.tsx:20` | JsxText | Devam etmek için rolünüzü seçin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0004 | `App.tsx:31` | JsxText | Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0005 | `App.tsx:39` | StringLiteral | PILOT — kısıtlı (takma ad, sunucusuz) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0006 | `App.tsx:39` | StringLiteral | TAM — MEB dersleri aktif | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0007 | `App.tsx:39` | StringLiteral | DEMO — jüri tanıtım | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0008 | `components/Ekranlar.tsx:25` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0009 | `components/Ekranlar.tsx:32` | JsxText | Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0010 | `components/Ekranlar.tsx:33` | JsxText | Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0011 | `components/Ekranlar.tsx:38` | StringLiteral | T1/T2 Transfer Kanıtı İzleme (Günün Oturumları) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0012 | `components/Ekranlar.tsx:42` | JsxText | dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0013 | `components/Ekranlar.tsx:44` | JsxText | T1 Merkezi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0014 | `components/Ekranlar.tsx:45` | JsxText | T2 Okul Bekleniyor | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0015 | `components/Ekranlar.tsx:51` | StringLiteral | Onay Bekleyen Raporlar (Human-Accountable AI) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0016 | `components/Ekranlar.tsx:53` | JsxText | YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0017 | `components/Ekranlar.tsx:67` | StringLiteral | Dosya listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0018 | `components/Ekranlar.tsx:77` | TemplateHead | Dosya kartı — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0019 | `components/Ekranlar.tsx:79` | StringLiteral | Ad (maskeli) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0020 | `components/Ekranlar.tsx:79` | StringLiteral | Doğum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0021 | `components/Ekranlar.tsx:79` | StringLiteral | Okul / Sınıf | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0022 | `components/Ekranlar.tsx:80` | StringLiteral | Devamsızlık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0023 | `components/Ekranlar.tsx:81` | StringLiteral | Rıza kaydı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0024 | `components/Ekranlar.tsx:81` | StringLiteral | Geçmiş BEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0025 | `components/Ekranlar.tsx:86` | StringLiteral | Program kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0026 | `components/Ekranlar.tsx:88` | JsxText | Seans sayısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0027 | `components/Ekranlar.tsx:89` | JsxText | Sıklık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0028 | `components/Ekranlar.tsx:90` | JsxText | Aile bileşeni | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0029 | `components/Ekranlar.tsx:91` | JsxText | RAM rapor ref. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0030 | `components/Ekranlar.tsx:125` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0031 | `components/Ekranlar.tsx:125` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0032 | `components/Ekranlar.tsx:133` | StringLiteral | Oturum takvimi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0033 | `components/Ekranlar.tsx:137` | JsxText | haftası | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0034 | `components/Ekranlar.tsx:143` | JsxText | Çakışma: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0035 | `components/Ekranlar.tsx:143` | JsxText | (KC12) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0036 | `components/Ekranlar.tsx:148` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0037 | `components/Ekranlar.tsx:148` | JsxText | Saat | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0038 | `components/Ekranlar.tsx:148` | JsxText | Dosya | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0039 | `components/Ekranlar.tsx:148` | JsxText | Uzman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0040 | `components/Ekranlar.tsx:148` | JsxText | Durum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0041 | `components/Ekranlar.tsx:165` | JsxText | Bu haftada oturum yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0042 | `components/Ekranlar.tsx:168` | JsxText | Durumlar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0043 | `components/Ekranlar.tsx:168` | JsxText | · değişiklikler bu cihazda saklanır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0044 | `components/Ekranlar.tsx:170` | StringLiteral | Veli görüşme-randevu defteri (K-571/A2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0045 | `components/Ekranlar.tsx:170` | JsxText | hatırlatma gönderilmez — K-334 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0046 | `components/Ekranlar.tsx:172` | JsxText | Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0047 | `components/Ekranlar.tsx:175` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0048 | `components/Ekranlar.tsx:177` | JsxText | Konu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0049 | `components/Ekranlar.tsx:178` | StringLiteral | örn. B yarı-dönem değerlendirme paylaşımı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0050 | `components/Ekranlar.tsx:180` | JsxText | Deftere ekle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0051 | `components/Ekranlar.tsx:183` | JsxText | Defter boş — ilk görüşme kaydını ekleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0052 | `components/Ekranlar.tsx:184` | JsxText | Tarih | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0053 | `components/Ekranlar.tsx:184` | JsxText | Konu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0054 | `components/Ekranlar.tsx:184` | JsxText | Durum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0055 | `components/Ekranlar.tsx:184` | JsxText | Not | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0056 | `components/Ekranlar.tsx:189` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0057 | `components/Ekranlar.tsx:189` | StringLiteral | gerçekleşti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0058 | `components/Ekranlar.tsx:190` | StringLiteral | kısa not (yapılandırılmamış) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0059 | `components/Ekranlar.tsx:192` | JsxText | Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0060 | `components/Ekranlar.tsx:206` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0061 | `components/Ekranlar.tsx:206` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0062 | `components/Ekranlar.tsx:214` | StringLiteral | Oturum kartı — OT-101 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0063 | `components/Ekranlar.tsx:215` | JsxText | Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0064 | `components/Ekranlar.tsx:217` | JsxText | Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0065 | `components/Ekranlar.tsx:222` | JsxText | Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0066 | `components/Ekranlar.tsx:225` | StringLiteral | Bu oturumda seçili BGM modülleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0067 | `components/Ekranlar.tsx:225` | JsxText | · sıra uzmanın | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0068 | `components/Ekranlar.tsx:227` | JsxText | Bu dosya için BGM seçilmedi (Bilişsel Geliştirme ekranından alınır). DEP etkinlikleri yine kullanılabilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0069 | `components/Ekranlar.tsx:232` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0070 | `components/Ekranlar.tsx:233` | JsxText | · girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0071 | `components/Ekranlar.tsx:233` | TemplateHead | · DEP köprüsü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0072 | `components/Ekranlar.tsx:239` | JsxText | Etkinlik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0073 | `components/Ekranlar.tsx:240` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0074 | `components/Ekranlar.tsx:240` | JsxText | İpucu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0075 | `components/Ekranlar.tsx:241` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0076 | `components/Ekranlar.tsx:246` | StringLiteral | Hızlı girdi paneli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0077 | `components/Ekranlar.tsx:246` | JsxText | YASA-1 etkin | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0078 | `components/Ekranlar.tsx:249` | JsxText | Etkinlik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0079 | `components/Ekranlar.tsx:249` | JsxText | *zorunlu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0080 | `components/Ekranlar.tsx:252` | JsxText | — etkinlik seçin — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0081 | `components/Ekranlar.tsx:253` | StringLiteral | DEP-2026 etkinlikleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0082 | `components/Ekranlar.tsx:257` | StringLiteral | BGM-12 (bu dosya için seçili) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0083 | `components/Ekranlar.tsx:258` | JsxText | [BGM] | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0084 | `components/Ekranlar.tsx:264` | JsxText | Kodlama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0085 | `components/Ekranlar.tsx:271` | JsxText | Değer | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0086 | `components/Ekranlar.tsx:276` | JsxText | Gözlenen ipucu-kademesi (K-571/A4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0087 | `components/Ekranlar.tsx:279` | JsxText | — seçilmeyebilir — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0088 | `components/Ekranlar.tsx:280` | JsxText | Model | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0089 | `components/Ekranlar.tsx:281` | JsxText | Sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0090 | `components/Ekranlar.tsx:282` | JsxText | Bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0091 | `components/Ekranlar.tsx:287` | JsxText | Planlı ipucu-kademesi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0092 | `components/Ekranlar.tsx:287` | JsxText | · gözlem kaydı uzmanın teyididir (K-02: ölçüm-değil-gözlem). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0093 | `components/Ekranlar.tsx:294` | JsxText | Girdi kaydet | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0094 | `components/Ekranlar.tsx:304` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0095 | `components/Ekranlar.tsx:306` | JsxText | · ipucu(gözlenen): | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0096 | `components/Ekranlar.tsx:306` | StringLiteral | Sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0097 | `components/Ekranlar.tsx:306` | StringLiteral | Bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0098 | `components/Ekranlar.tsx:328` | JsxText | Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0099 | `components/Ekranlar.tsx:329` | JsxText | Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0100 | `components/Ekranlar.tsx:331` | StringLiteral | DEP saat-izleri — girdilerden türetilmiş (K-571/A1) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0101 | `components/Ekranlar.tsx:331` | JsxText | YASA-2 deseni: elle çizilmez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0102 | `components/Ekranlar.tsx:333` | JsxText | Dosya | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0103 | `components/Ekranlar.tsx:333` | JsxText | Tamamlanan oturum | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0104 | `components/Ekranlar.tsx:333` | JsxText | Toplam süre | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0105 | `components/Ekranlar.tsx:333` | JsxText | DEP girdisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0106 | `components/Ekranlar.tsx:335` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0107 | `components/Ekranlar.tsx:341` | JsxText | Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0108 | `components/Ekranlar.tsx:344` | StringLiteral | İzleme çizelgesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0109 | `components/Ekranlar.tsx:344` | JsxText | girdilerden türetildi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0110 | `components/Ekranlar.tsx:349` | StringLiteral | Tümü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0111 | `components/Ekranlar.tsx:349` | TemplateHead | BGM-12 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0112 | `components/Ekranlar.tsx:363` | JsxText | Toplam girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0113 | `components/Ekranlar.tsx:363` | JsxText | · Hedefe ulaşılan: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0114 | `components/Ekranlar.tsx:364` | JsxText | Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0115 | `components/Ekranlar.tsx:374` | StringLiteral | Seans özeti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0116 | `components/Ekranlar.tsx:374` | StringLiteral | Aylık özet | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0117 | `components/Ekranlar.tsx:374` | StringLiteral | Dönem sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0118 | `components/Ekranlar.tsx:375` | StringLiteral | BEP ilerleme taslağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0119 | `components/Ekranlar.tsx:375` | StringLiteral | RAM izleme paketi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0120 | `components/Ekranlar.tsx:376` | StringLiteral | Aile bilgilendirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0121 | `components/Ekranlar.tsx:381` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0122 | `components/Ekranlar.tsx:384` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0123 | `components/Ekranlar.tsx:387` | TemplateHead | — YZ EĞİTİMSEL DESTEK ÖNERİSİ — ↵ (Kanıt Kaynağı: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0124 | `components/Ekranlar.tsx:390` | TemplateMiddle | T1 seansı, | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0125 | `components/Ekranlar.tsx:390` | TemplateMiddle | dk aktif izlem, | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0126 | `components/Ekranlar.tsx:390` | LastTemplateToken | girdi kaydı) ↵ Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir. ↵  ↵ ⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0127 | `components/Ekranlar.tsx:398` | FirstTemplateToken | — YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ — ↵ Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0128 | `components/Ekranlar.tsx:407` | TemplateHead | <!doctype html><title> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0129 | `components/Ekranlar.tsx:407` | TemplateMiddle | </title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:16px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0130 | `components/Ekranlar.tsx:407` | TemplateMiddle | </h1><div class=muhur>ONAYLI — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0131 | `components/Ekranlar.tsx:407` | TemplateMiddle | </pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;\|&nbsp; Kopya 2/2 — Kurum arşivi · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0132 | `components/Ekranlar.tsx:407` | TemplateMiddle | · Supporta v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0133 | `components/Ekranlar.tsx:409` | TemplateHead | tur,baslik,durum,icerik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0134 | `components/Ekranlar.tsx:419` | JsxText | UZMAN ONAYI BEKLİYOR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0135 | `components/Ekranlar.tsx:419` | JsxText | UZMAN ONAYLI | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0136 | `components/Ekranlar.tsx:433` | JsxText | Human-Accountable AI (YZ Destek Asistanı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0137 | `components/Ekranlar.tsx:437` | JsxText | Kanıtı İncele ve YZ Önerisi Al | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0138 | `components/Ekranlar.tsx:440` | JsxText | Öneriyi Reddet ve Gerekçelendir | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0139 | `components/Ekranlar.tsx:443` | JsxText | YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0140 | `components/Ekranlar.tsx:444` | StringLiteral | YZ EĞİTİMSEL DESTEK ÖNERİSİ | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0141 | `components/Ekranlar.tsx:445` | JsxText | YZ ÖNERİSİ KATMANI — uzman onayı gerektirir | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0142 | `components/Ekranlar.tsx:451` | JsxText | ✓ Değişiklikleri Onayla ve İmzala | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0143 | `components/Ekranlar.tsx:452` | JsxText | Dışa aktar (2 kopya) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0144 | `components/Ekranlar.tsx:453` | JsxText | Onaysız rapor dışa aktarılamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0145 | `components/Ekranlar.tsx:468` | StringLiteral | MEB destek eğitim programı modülleriyle hizalı çıktı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0146 | `components/Ekranlar.tsx:473` | JsxText | sa) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0147 | `components/Ekranlar.tsx:477` | JsxText | Seçili: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0148 | `components/Ekranlar.tsx:477` | JsxText | bölüm · önerilen | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0149 | `components/Ekranlar.tsx:477` | JsxText | ders saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0150 | `components/Ekranlar.tsx:478` | JsxText | Toplam program: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0151 | `components/Ekranlar.tsx:478` | JsxText | ders saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0152 | `components/Ekranlar.tsx:478` | JsxText | · 6 modül · giriş yalnız ELLE yapılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0153 | `components/Ekranlar.tsx:480` | JsxText | Modül seçimi serbesttir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0154 | `components/Ekranlar.tsx:483` | JsxText | Resmî tavan (ÖEK Yön. md.24/4): aylık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0155 | `components/Ekranlar.tsx:483` | JsxText | bireysel · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0156 | `components/Ekranlar.tsx:483` | JsxText | grup · ↵         haftalık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0157 | `components/Ekranlar.tsx:484` | JsxText | · günlük toplam | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0158 | `components/Ekranlar.tsx:484` | JsxText | saat. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0159 | `components/Ekranlar.tsx:496` | StringLiteral | Aile & Öğretmen İşbirliği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0160 | `components/Ekranlar.tsx:497` | JsxText | Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0161 | `components/Ekranlar.tsx:500` | StringLiteral | Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0162 | `components/Ekranlar.tsx:500` | JsxText | K-407 · 5+1 · TASLAK | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0163 | `components/Ekranlar.tsx:509` | StringLiteral | Bilgilendirme çıktısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0164 | `components/Ekranlar.tsx:510` | JsxText | Yalnız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0165 | `components/Ekranlar.tsx:510` | JsxText | onaylı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0166 | `components/Ekranlar.tsx:510` | JsxText | raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0167 | `components/Ekranlar.tsx:512` | JsxText | Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0168 | `components/Ekranlar.tsx:522` | StringLiteral | Şerh kütüphanesi ve roller | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0169 | `components/Ekranlar.tsx:528` | JsxText | Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0170 | `components/Ekranlar.tsx:530` | JsxText | Kapsam dışı (bilinçli sınırlar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0171 | `components/Ekranlar.tsx:540` | JsxText | Yerel veri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0172 | `components/Ekranlar.tsx:542` | JsxText | Girdiler, oturum durumları ve rapor onayları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0173 | `components/Ekranlar.tsx:542` | JsxText | yalnız bu cihazda | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0174 | `components/Ekranlar.tsx:542` | JsxText | saklanır (KVKK yerel-önce). ↵           Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0175 | `components/Ekranlar.tsx:548` | JsxText | Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0176 | `components/Ekranlar.tsx:564` | StringLiteral | RAM raporu ve kayıt hattı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0177 | `components/Ekranlar.tsx:572` | JsxText | Kayıt hattı: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0178 | `components/Ekranlar.tsx:572` | JsxText | RAM raporu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0179 | `components/Ekranlar.tsx:572` | JsxText | · Planlama: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0180 | `components/Ekranlar.tsx:575` | StringLiteral | Rapor no | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0181 | `components/Ekranlar.tsx:575` | StringLiteral | Rapor tarihi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0182 | `components/Ekranlar.tsx:575` | StringLiteral | Geçerlilik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0183 | `components/Ekranlar.tsx:576` | StringLiteral | EDİF durumu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0184 | `components/Ekranlar.tsx:576` | StringLiteral | Sonraki izleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0185 | `components/Ekranlar.tsx:577` | StringLiteral | Hazır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0186 | `components/Ekranlar.tsx:577` | StringLiteral | Hazır değil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0187 | `components/Ekranlar.tsx:583` | StringLiteral | Resmî form ailesi — hangi girdi neyi besler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0188 | `components/Ekranlar.tsx:584` | JsxText | DEP-2026 EK-1…EK-7 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0189 | `components/Ekranlar.tsx:587` | JsxText | Form | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0190 | `components/Ekranlar.tsx:587` | JsxText | Doldurma anı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0191 | `components/Ekranlar.tsx:587` | JsxText | Supporta katkısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0192 | `components/Ekranlar.tsx:600` | JsxText | Sınır: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0193 | `components/Ekranlar.tsx:600` | JsxText | Supporta bu formları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0194 | `components/Ekranlar.tsx:600` | JsxText | DOLDURMAZ | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0195 | `components/Ekranlar.tsx:600` | JsxText | . x/+ işaretini, performans düzeyini ve ↵           “ulaşılamama nedenini” | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0196 | `components/Ekranlar.tsx:601` | JsxText | uzman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0197 | `components/Ekranlar.tsx:601` | JsxText | belirler; portfolyo | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0198 | `components/Ekranlar.tsx:601` | JsxText | RAM onayına | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0199 | `components/Ekranlar.tsx:601` | JsxText | gider. ↵           Model: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0200 | `components/Ekranlar.tsx:602` | JsxText | Supporta kanıt üretir · uzman karar verir · RAM onaylar. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0201 | `components/Ekranlar.tsx:605` | JsxText | Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0202 | `components/Ekranlar.tsx:619` | StringLiteral | Ev çalışmaları ve seans dışı görevler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0203 | `components/Ekranlar.tsx:620` | JsxText | kim · ne · ne zaman | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0204 | `components/Ekranlar.tsx:628` | JsxText | Not: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0205 | `components/Ekranlar.tsx:636` | JsxText | verildi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0206 | `components/Ekranlar.tsx:636` | JsxText | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0207 | `components/Ekranlar.tsx:636` | JsxText | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0208 | `components/Ekranlar.tsx:642` | StringLiteral | Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0209 | `components/Ekranlar.tsx:644` | StringLiteral | Seans başı izleme ritüeli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0210 | `components/Ekranlar.tsx:646` | JsxText | Ev çalışması gözden geçirilir (yapıldı/yapılmadı — | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0211 | `components/Ekranlar.tsx:646` | JsxText | yargı değil gözlem | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0212 | `components/Ekranlar.tsx:647` | JsxText | Bir önceki oturumun hedef davranışı hatırlatılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0213 | `components/Ekranlar.tsx:648` | JsxText | Bugünün etkinliği ve ipucu kademesi belirlenir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0214 | `components/Ekranlar.tsx:649` | JsxText | Oturum sonunda veli için tek satırlık jargonsuz not yazılır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0215 | `components/Ekranlar.tsx:660` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0216 | `components/Ekranlar.tsx:660` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0217 | `components/Ekranlar.tsx:664` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0218 | `components/Ekranlar.tsx:664` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0219 | `components/Ekranlar.tsx:664` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0220 | `components/Ekranlar.tsx:665` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0221 | `components/Ekranlar.tsx:667` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0222 | `components/Ekranlar.tsx:670` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0223 | `components/Ekranlar.tsx:670` | StringLiteral | Model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0224 | `components/Ekranlar.tsx:673` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0225 | `components/Ekranlar.tsx:675` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0226 | `components/Ekranlar.tsx:675` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0227 | `components/Ekranlar.tsx:675` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0228 | `components/Ekranlar.tsx:679` | StringLiteral | Etkinlik ve hedef davranış kataloğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0229 | `components/Ekranlar.tsx:679` | JsxText | etkinlik · DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0230 | `components/Ekranlar.tsx:679` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0231 | `components/Ekranlar.tsx:679` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0232 | `components/Ekranlar.tsx:679` | JsxText | · BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0233 | `components/Ekranlar.tsx:679` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0234 | `components/Ekranlar.tsx:681` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0235 | `components/Ekranlar.tsx:681` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0236 | `components/Ekranlar.tsx:684` | TemplateHead | Tümü ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0237 | `components/Ekranlar.tsx:684` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0238 | `components/Ekranlar.tsx:684` | TemplateHead | DEP-2026 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0239 | `components/Ekranlar.tsx:684` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0240 | `components/Ekranlar.tsx:684` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0241 | `components/Ekranlar.tsx:684` | TemplateHead | BGM-12 ( | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0242 | `components/Ekranlar.tsx:684` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0243 | `components/Ekranlar.tsx:693` | StringLiteral | Tümü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0244 | `components/Ekranlar.tsx:698` | StringLiteral | Etkinliği düzenle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0245 | `components/Ekranlar.tsx:698` | StringLiteral | Yeni etkinlik ekle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0246 | `components/Ekranlar.tsx:698` | JsxText | · kayıt bu cihazda saklanır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0247 | `components/Ekranlar.tsx:700` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0248 | `components/Ekranlar.tsx:700` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0249 | `components/Ekranlar.tsx:700` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0250 | `components/Ekranlar.tsx:701` | JsxText | DEP-2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0251 | `components/Ekranlar.tsx:701` | JsxText | BGM-12 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0252 | `components/Ekranlar.tsx:703` | StringLiteral | Etkinlik adı * | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0253 | `components/Ekranlar.tsx:704` | StringLiteral | Hedef kod (örn 3.1.2 / BGM-EQ-01) * | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0254 | `components/Ekranlar.tsx:705` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0255 | `components/Ekranlar.tsx:706` | StringLiteral | İpucu kademesi (örn Model→bağımsız) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0256 | `components/Ekranlar.tsx:707` | StringLiteral | Malzeme (virgülle ayır) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0257 | `components/Ekranlar.tsx:710` | StringLiteral | Güncelle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0258 | `components/Ekranlar.tsx:711` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0259 | `components/Ekranlar.tsx:711` | JsxText | İptal | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0260 | `components/Ekranlar.tsx:712` | JsxText | Varsayılana sıfırla | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0261 | `components/Ekranlar.tsx:719` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0262 | `components/Ekranlar.tsx:719` | JsxText | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0263 | `components/Ekranlar.tsx:722` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0264 | `components/Ekranlar.tsx:723` | JsxText | İpucu kademesi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0265 | `components/Ekranlar.tsx:724` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0266 | `components/Ekranlar.tsx:726` | JsxText | Düzenle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0267 | `components/Ekranlar.tsx:727` | JsxText | Sil | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0268 | `components/Ekranlar.tsx:732` | JsxText | Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0269 | `components/Ekranlar.tsx:732` | JsxText | — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0270 | `components/Ekranlar.tsx:742` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0271 | `components/Ekranlar.tsx:743` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0272 | `components/Ekranlar.tsx:752` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0273 | `components/Ekranlar.tsx:755` | StringLiteral | Bilişsel Geliştirme Modülleri (BGM-12) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0274 | `components/Ekranlar.tsx:756` | JsxText | modül · menü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0275 | `components/Ekranlar.tsx:758` | JsxText | İki katman. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0276 | `components/Ekranlar.tsx:761` | JsxText | Modül seçimi serbesttir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0277 | `components/Ekranlar.tsx:761` | JsxText | Persona sarmalı dayatılmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0278 | `components/Ekranlar.tsx:764` | JsxText | TASLAK. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0279 | `components/Ekranlar.tsx:764` | JsxText | Tam kartlar: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0280 | `components/Ekranlar.tsx:764` | JsxText | LEXIVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0281 | `components/Ekranlar.tsx:775` | JsxText | Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil): | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0282 | `components/Ekranlar.tsx:776` | StringLiteral | henüz seçilmedi — 1-2-3 atlanabilir | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0283 | `components/Ekranlar.tsx:793` | JsxText | çekirdek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0284 | `components/Ekranlar.tsx:798` | JsxText | Programdan çıkar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0285 | `components/Ekranlar.tsx:800` | JsxText | Programa al | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0286 | `components/Ekranlar.tsx:802` | JsxText | Kart | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0287 | `components/Ekranlar.tsx:806` | JsxText | Tanım: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0288 | `components/Ekranlar.tsx:807` | JsxText | Amaç: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0289 | `components/Ekranlar.tsx:808` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0290 | `components/Ekranlar.tsx:809` | JsxText | Etkinlik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0291 | `components/Ekranlar.tsx:810` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0292 | `components/Ekranlar.tsx:810` | JsxText | İpucu: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0293 | `components/Ekranlar.tsx:810` | JsxText | Girdi: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0294 | `components/Ekranlar.tsx:811` | JsxText | Ödev: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0295 | `components/Ekranlar.tsx:812` | JsxText | Önlem: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0296 | `components/Ekranlar.tsx:813` | JsxText | Öneri: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0297 | `components/Ekranlar.tsx:814` | JsxText | DEP köprüsü: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0298 | `components/Ekranlar.tsx:814` | LastTemplateToken | — kanıt satırı önerisi; BEP birimi kararı değildir (K-263) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0299 | `components/Ekranlar.tsx:814` | StringLiteral | yok (bütünleştirme turu) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0300 | `components/Ekranlar.tsx:815` | JsxText | Dayanak: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0301 | `components/Kabuk.tsx:7` | StringLiteral | Eğitmen Kürsüsü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0302 | `components/Kabuk.tsx:10` | StringLiteral | Oturum Atölyesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0303 | `components/Kabuk.tsx:11` | StringLiteral | Etkinlik Kataloğu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0304 | `components/Kabuk.tsx:12` | StringLiteral | İzleme Çizelgesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0305 | `components/Kabuk.tsx:13` | StringLiteral | Rapor Atölyesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0306 | `components/Kabuk.tsx:14` | StringLiteral | Program Hizalama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0307 | `components/Kabuk.tsx:15` | StringLiteral | Bilişsel Geliştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0308 | `components/Kabuk.tsx:16` | StringLiteral | RAM & BEP Takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0309 | `components/Kabuk.tsx:17` | StringLiteral | Ev Çalışmaları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0310 | `components/Kabuk.tsx:18` | StringLiteral | Aile & Öğretmen | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0311 | `components/Kabuk.tsx:32` | JsxText | LEXIVA Supporta™ | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0312 | `components/Kabuk.tsx:33` | JsxText | Uzman Kokpiti · v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0313 | `components/Kabuk.tsx:50` | JsxText | Rol: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0314 | `components/Kabuk.tsx:50` | JsxText | · Sentetik demo verisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0315 | `components/Kabuk.tsx:63` | JsxText | LEXIVA Supporta: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0316 | `components/Sherh.tsx:3` | StringLiteral | nötr | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0317 | `components/Sherh.tsx:3` | StringLiteral | nötr | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0318 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateHead | <!doctype html><title> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0319 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px;border:1px solid #e2e8f0;padding:12px;border-radius:10px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:12px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0320 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </h1><div class=muhur>ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER</div><pre> | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0321 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | </pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;\|&nbsp; Kopya 2/2 — Kurum arşivi · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0322 | `components/aile/AileEgitimMerkezi.tsx:14` | TemplateMiddle | · Supporta v | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0323 | `components/aile/AileEgitimMerkezi.tsx:28` | JsxText | A — Genel (5 mini-modül) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0324 | `components/aile/AileEgitimMerkezi.tsx:36` | JsxText | B — Analize Göre (uzman seçer) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0325 | `components/aile/AileEgitimMerkezi.tsx:52` | JsxText | dk · | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0326 | `components/aile/AileEgitimMerkezi.tsx:64` | JsxText | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0327 | `components/aile/AileEgitimMerkezi.tsx:70` | TemplateMiddle | Malzeme: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0328 | `components/aile/AileEgitimMerkezi.tsx:73` | JsxText | Yazdır / PDF | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0329 | `components/aile/AileEgitimMerkezi.tsx:81` | StringLiteral | Kopyalandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0330 | `components/aile/AileEgitimMerkezi.tsx:86` | JsxText | Kopyala | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0331 | `components/aile/AileEgitimMerkezi.tsx:90` | JsxText | · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0332 | `components/aile/AileEgitimMerkezi.tsx:97` | JsxText | Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0333 | `components/aile/AileEgitimMerkezi.tsx:102` | JsxText | Tetik: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0334 | `components/aile/AileEgitimMerkezi.tsx:108` | JsxText | Aileye görev örneği: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0335 | `components/aile/AileEgitimMerkezi.tsx:110` | JsxText | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0336 | `components/aile/AileEgitimMerkezi.tsx:115` | TemplateMiddle | Görev: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0337 | `components/aile/AileEgitimMerkezi.tsx:115` | TemplateMiddle | Ölçüm: | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0338 | `components/aile/AileEgitimMerkezi.tsx:118` | JsxText | Şablonu Yazdır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0339 | `components/aile/AileEgitimMerkezi.tsx:121` | JsxText | · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0340 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Can B. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0341 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Görsel İpucu | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0342 | `components/egitmen/EgitmenDestekPaneli.tsx:15` | StringLiteral | Düşük Uyaranlı Görev | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0343 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Ali Y. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0344 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Görev Parçalama | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0345 | `components/egitmen/EgitmenDestekPaneli.tsx:16` | StringLiteral | Sözel Yönerge | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0346 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Elif S. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0347 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Zamanlayıcı | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0348 | `components/egitmen/EgitmenDestekPaneli.tsx:17` | StringLiteral | Hareketli Mola | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0349 | `components/egitmen/EgitmenDestekPaneli.tsx:29` | JsxText | Eğitmen Destek Paneli (Supporta) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0350 | `components/egitmen/EgitmenDestekPaneli.tsx:35` | JsxText | Öğrenci Listesi | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0351 | `components/egitmen/EgitmenDestekPaneli.tsx:59` | JsxText | Destek Profili | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0352 | `components/egitmen/EgitmenDestekPaneli.tsx:60` | JsxText | Şu an uygulanan destek stratejisi ve performansı. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0353 | `components/egitmen/EgitmenDestekPaneli.tsx:65` | JsxText | Aktif Destek (Müdahale) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0354 | `components/egitmen/EgitmenDestekPaneli.tsx:69` | JsxText | İstikrarlı Başarı Serisi | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0355 | `components/egitmen/EgitmenDestekPaneli.tsx:70` | JsxText | Görev | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0356 | `components/egitmen/EgitmenDestekPaneli.tsx:79` | JsxText | Desteği Geri Çekme Önerisi (Support Fading) | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0357 | `components/egitmen/EgitmenDestekPaneli.tsx:81` | JsxText | Bu öğrenci | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0358 | `components/egitmen/EgitmenDestekPaneli.tsx:81` | JsxText | stratejisinde uzmanlaştı. Bağımsızlığı artırmak adına,  ↵                     sonraki seansta desteği bir alt seviyeye indirmeyi (Fading) deneyebilirsiniz. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0359 | `components/egitmen/EgitmenDestekPaneli.tsx:85` | JsxText | Desteği Azalt / Kaldır | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0360 | `components/egitmen/EgitmenDestekPaneli.tsx:94` | JsxText | Toparlanma (Recovery) Zekası | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0361 | `components/egitmen/EgitmenDestekPaneli.tsx:95` | JsxText | Öğrencinin moladan veya kriz anından sonra en hızlı toparlandığı koşullar. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0362 | `components/egitmen/EgitmenDestekPaneli.tsx:99` | JsxText | En Verimli Dönüş (Transition) Aracı: | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0363 | `components/egitmen/EgitmenDestekPaneli.tsx:105` | JsxText | Öneri: Mola dönüşlerinde yüksek uyaranlı veya zor görevlerden kaçının. Başlangıçta | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0364 | `components/egitmen/EgitmenDestekPaneli.tsx:105` | JsxText | vererek bilişsel geçişi (transition) kolaylaştırın. | BAĞLI DEĞİL — kaynak rezervi |
| SUP-LEX-0365 | `data/aile/genel.ts:19` | StringLiteral | Nasihat ve Kıyas Yok — Gözlem Dili | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0366 | `data/aile/genel.ts:20` | StringLiteral | Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0367 | `data/aile/genel.ts:22` | StringLiteral | “Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0368 | `data/aile/genel.ts:23` | StringLiteral | “Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0369 | `data/aile/genel.ts:24` | StringLiteral | Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0370 | `data/aile/genel.ts:27` | StringLiteral | A4 gözlem kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0371 | `data/aile/genel.ts:28` | StringLiteral | Yorum/değer yargısı yok — yalnızca gözlem. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0372 | `data/aile/genel.ts:32` | StringLiteral | Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0373 | `data/aile/genel.ts:33` | StringLiteral | Yazılı planla öngörülebilirlik sağlamak (Z-1). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0374 | `data/aile/genel.ts:35` | StringLiteral | Akşam rutinini 5 soruyla duvara asın: ne yapılacak · ne zaman · nerede · ne kadar · sonra ne var (Tablo 9/10 kavramı). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0375 | `data/aile/genel.ts:36` | StringLiteral | Resimli/renkli kartta her adım tek satır, tik kutusu ekleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0376 | `data/aile/genel.ts:37` | StringLiteral | Planı çocukla birlikte hazırlayın, her gün aynı yerde tutun. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0377 | `data/aile/genel.ts:40` | StringLiteral | rutin şablonu (A4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0378 | `data/aile/genel.ts:40` | StringLiteral | renkli kalem | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0379 | `data/aile/genel.ts:44` | StringLiteral | Görsel Ortam — Uyaran Yalıtımı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0380 | `data/aile/genel.ts:45` | StringLiteral | Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görsel). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0381 | `data/aile/genel.ts:47` | StringLiteral | Masada yalnızca o derste gerekli materyal kalsın, fazlası kutuya. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0382 | `data/aile/genel.ts:48` | StringLiteral | Dersten önce yüzey toplama ritüeli: 1 dk birlikte toplayın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0383 | `data/aile/genel.ts:49` | StringLiteral | Duvarlarda hareketli/ışıklı uyaranı çalışma anında kaldırın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0384 | `data/aile/genel.ts:52` | StringLiteral | toplama kutusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0385 | `data/aile/genel.ts:56` | StringLiteral | İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0386 | `data/aile/genel.ts:57` | StringLiteral | İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + Z-7 işitsel). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0387 | `data/aile/genel.ts:59` | StringLiteral | Çalışma anında TV/arka plan sesini kapatın, kapıyı kapalı tutun. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0388 | `data/aile/genel.ts:60` | StringLiteral | Yönergeyi göz hizasında, tek cümle, 2 adımı geçmeden söyleyin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0389 | `data/aile/genel.ts:61` | StringLiteral | Gerekirse söze değil, hafif dokunarak (omuz) ilgisini çekin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0390 | `data/aile/genel.ts:68` | StringLiteral | Pekiştireç ve Kayıt — Hedef Davranış + İpucu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0391 | `data/aile/genel.ts:69` | StringLiteral | Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 uyumlu çerçeve, Z-2). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0392 | `data/aile/genel.ts:71` | StringLiteral | Tek hedef seçin: “ödevin ilk 10 dk’sında masada kalma”. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0393 | `data/aile/genel.ts:72` | StringLiteral | İpucu kademesi: model → sözel hatırlatma → bağımsız; ipucunu kademeli çekin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0394 | `data/aile/genel.ts:73` | StringLiteral | Her gün “yaptı / yapmadı” tik kartına işleyin, haftalık uzmana getirin (dijital puan yok). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0395 | `data/aile/genel.ts:76` | StringLiteral | hedef kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0396 | `data/aile/genel.ts:76` | StringLiteral | tik tablosu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0397 | `data/aile/genel.ts:77` | StringLiteral | Pekiştireç maddi değil, etkinlik/övgü temelli olabilir — uzman belirler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0398 | `data/aile/kisisel.ts:18` | StringLiteral | İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0399 | `data/aile/kisisel.ts:19` | StringLiteral | Analize Göre Aile Görevi (Uzman Seçer) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0400 | `data/aile/kisisel.ts:20` | FirstTemplateToken | [UZMAN DOLDURUR — K-02] ↵ Gözlem/Rapor bulgusu (tarihli, sayılabilir): ... ↵ Aileye önerilen tek görev (1 cümle, bağlamlı): ... ↵ İpucu kademesi (model/sözel/bağımsız): ... ↵ Kayıt biçimi (tik/süre): ... ↵ Sonraki izleme tarihi: ... | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0401 | `data/aile/kisisel.ts:21` | StringLiteral | Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0402 | `data/aile/kisisel.ts:22` | StringLiteral | Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0403 | `data/aile/kisisel.ts:27` | StringLiteral | Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0404 | `data/aile/kisisel.ts:27` | StringLiteral | Çizelgede kopma > eşik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0405 | `data/aile/kisisel.ts:28` | StringLiteral | Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0406 | `data/aile/kisisel.ts:28` | StringLiteral | Ev Çalışmaları “yapılmadı” >2 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0407 | `data/aile/kisisel.ts:29` | StringLiteral | Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0408 | `data/aile/kisisel.ts:29` | StringLiteral | Girdi “0/3” yoğun | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0409 | `data/bgm.ts:15` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0410 | `data/bgm.ts:47` | StringLiteral | Grup I — fonolojik temel (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0411 | `data/bgm.ts:48` | StringLiteral | Grup II — okuma/yazma/matematik (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0412 | `data/bgm.ts:49` | StringLiteral | Grup III — aktarım ve özerklik (sıra değil) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0413 | `data/bgm.ts:54` | StringLiteral | Ses Merdiveni | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0414 | `data/bgm.ts:54` | StringLiteral | Fonolojik eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0415 | `data/bgm.ts:55` | StringLiteral | Fonolojik farkındalık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0416 | `data/bgm.ts:56` | StringLiteral | Merdiven ardıl sırasıyla (sözcük→uyak→hece→sesbirimi) basamak basamak ilerleme pratiği (DEP 3.2.1: önce eşleme). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0417 | `data/bgm.ts:57` | StringLiteral | Başlangıç-sesi farkındalığını merdiven üstünde izlenebilir kılmak; uzman hedefi BEP satırına taşır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0418 | `data/bgm.ts:58` | StringLiteral | Basamak isabeti (0–3) · eşleme/ayırt etme tutarlılığı. Bant/eşik ve tanı YOK (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0419 | `data/bgm.ts:59` | StringLiteral | Merdiven şeması üzerinde 2 örnek eşleme (model), sonra 6 sözcük bağımsız tur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0420 | `data/bgm.ts:60` | StringLiteral | Evde 5 sözcüğün başlangıç sesini eşleştirin (kavram; resmî form metni değil). Puanlanmaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0421 | `data/bgm.ts:61` | StringLiteral | Masada yalnız merdiven şeması ve ses kartları; ekran görüş alanında olmasın. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0422 | `data/bgm.ts:62` | StringLiteral | Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0423 | `data/bgm.ts:64` | StringLiteral | 5–7 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0424 | `data/bgm.ts:65` | StringLiteral | merdiven şeması | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0425 | `data/bgm.ts:65` | StringLiteral | ses kartları (6) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0426 | `data/bgm.ts:65` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0427 | `data/bgm.ts:66` | StringLiteral | model → sözel ("ilk sesi yakala") → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0428 | `data/bgm.ts:68` | StringLiteral | 2021 DEP 3.1/3.2.1 ardıl sıra · MEB Ses Farkındalık Öğretmen Kılavuzu (yapı atfı; K-08) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0429 | `data/bgm.ts:71` | StringLiteral | Ses Birimi Ayırt Etme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0430 | `data/bgm.ts:71` | StringLiteral | Harf seçiciliği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0431 | `data/bgm.ts:72` | StringLiteral | Fonolojik farkındalık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0432 | `data/bgm.ts:73` | StringLiteral | Karışık harf dizisinde hedef dışı uyaranı (X) seçip durma pratiği — fonolojik seçicilik. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0433 | `data/bgm.ts:74` | StringLiteral | Harf düzeyinde seçiciliği (okumaya taşınan çekirdek) seans içi verilerle izlemek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0434 | `data/bgm.ts:75` | StringLiteral | Isabet / kaçırma · erken basış adedi (SBA deseni). Yüzdelik yorumu ve tanı YOK (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0435 | `data/bgm.ts:76` | StringLiteral | SBA turu: X dışındaki harflerde BOŞLUK, X’te bekle (Persona ile aynı motor). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0436 | `data/bgm.ts:77` | StringLiteral | Evde 3 heceli sözcükleri hecederken ilk sesi vurgulama. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0437 | `data/bgm.ts:78` | StringLiteral | Kısa tur (5–7 dk); ardışık zorlamada mola (çocuk kontrol çubuğu). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0438 | `data/bgm.ts:79` | StringLiteral | Seans sonu yansıma: “Hangi harfi bekledin?” — sistem yorumlamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0439 | `data/bgm.ts:81` | StringLiteral | 5–7 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0440 | `data/bgm.ts:82` | StringLiteral | ekran (SBA) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0441 | `data/bgm.ts:82` | StringLiteral | ses kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0442 | `data/bgm.ts:83` | StringLiteral | model → sözel ("X’te bekle") → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0443 | `data/bgm.ts:85` | StringLiteral | 2021 DEP 3.2.1 ayırt etme basamağı · D-L1 merdiven (LEXIVA müfredat matrisi v0.3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0444 | `data/bgm.ts:88` | StringLiteral | Hece ve Parçalar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0445 | `data/bgm.ts:88` | StringLiteral | Sözcüğü bölme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0446 | `data/bgm.ts:89` | StringLiteral | Fonolojik parçalama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0447 | `data/bgm.ts:90` | StringLiteral | Sözcüğün hecelere/ses birimlerine bölünmesi — yönetilebilir birimlere ayırma. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0448 | `data/bgm.ts:91` | StringLiteral | Parçalama-tamamlama döngüsünü görür kılmak; “büyük sözcük” direncini ilk adımla kırmak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0449 | `data/bgm.ts:92` | StringLiteral | Hece bölme doğruluğu (x/+) · parça sayısı (betimleyici). Ölçüm yorumunu uzman yazar. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0450 | `data/bgm.ts:93` | StringLiteral | El çırparak heceleme: mar-tı (2), ke-le-bek (3); 8 kartlık bağımsız tur. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0451 | `data/bgm.ts:94` | StringLiteral | Yarınki okuma kartındaki 3 sözcüğü heceleyin. Sistem puanlamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0452 | `data/bgm.ts:95` | StringLiteral | Yönerge en fazla 2 adım; vurgulu söyleme modeli önce. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0453 | `data/bgm.ts:96` | StringLiteral | İpucu kademesi: model → sözel → bağımsız; silikleştirme notu uzmanda. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0454 | `data/bgm.ts:98` | StringLiteral | 6–8 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0455 | `data/bgm.ts:99` | StringLiteral | hece kartları (8) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0456 | `data/bgm.ts:99` | StringLiteral | parçalama şeridi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0457 | `data/bgm.ts:100` | StringLiteral | model (uzman bölür) → sözel → bağımsız (çocuk bölür) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0458 | `data/bgm.ts:102` | StringLiteral | 2021 DEP 3.1 (hece basamağı) · MEB Ses Farkındalık (yapı atfı; K-08) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0459 | `data/bgm.ts:105` | StringLiteral | Harf Tanıma ve Çizim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0460 | `data/bgm.ts:105` | StringLiteral | b/d-l izleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0461 | `data/bgm.ts:106` | StringLiteral | Görsel-tanım / yazım | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0462 | `data/bgm.ts:107` | StringLiteral | Harf şeklinin tanınması ve karışım çiftlerinde (b/d, p/q, l/g) kinestetik izleme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0463 | `data/bgm.ts:108` | StringLiteral | Harf şekli → ses eşlemesine görsel taban hazırlamak; ters çevirme gözlemi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0464 | `data/bgm.ts:109` | StringLiteral | Çizim isabeti (x/+) · karışım çifti hata adedi (betimleyici). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0465 | `data/bgm.ts:110` | StringLiteral | Havada/parmakla model çizim → büyük puntolu sayfada 4× b-d-l izleme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0466 | `data/bgm.ts:111` | StringLiteral | Evde harf kartlarıyla 10 dk eşleştirme. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0467 | `data/bgm.ts:112` | StringLiteral | Tek harf başına kısa tur; karışım çiftinde sözel onay ("bu b, b-b-b"). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0468 | `data/bgm.ts:113` | StringLiteral | Karışım çifti sıklığı yalnız gözlem; "becerememe" dili yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0469 | `data/bgm.ts:115` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0470 | `data/bgm.ts:116` | StringLiteral | büyük puntolu çizim sayfası | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0471 | `data/bgm.ts:116` | StringLiteral | harf kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0472 | `data/bgm.ts:117` | StringLiteral | fiziksel izleme → model → sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0473 | `data/bgm.ts:119` | StringLiteral | 2021 DEP 1.4/3.2 · LEXIVA Harf Çizim görevi (müfredat matrisi v0.3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0474 | `data/bgm.ts:122` | StringLiteral | Söyleneni Yaz | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0475 | `data/bgm.ts:122` | StringLiteral | İşitsel yazım | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0476 | `data/bgm.ts:124` | StringLiteral | Söylenen sözcükleri yazma + hataları sınıflandırma (atlama/ters/ekleme/karıştırma). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0477 | `data/bgm.ts:125` | StringLiteral | Yazım üretimini cezasız tekrar hakkıyla destekleyip hata sınıfını verilebilir kılmak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0478 | `data/bgm.ts:126` | StringLiteral | Sözcük isabeti (x/+) · hata sınıfı dağılımı (ÖGG Gözlem Formu Yazma deseni). Yorum uzmanda. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0479 | `data/bgm.ts:127` | StringLiteral | 6 sözcük söylene yazılır; hatalı yazımlar hata sınıfı kartına tiklenir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0480 | `data/bgm.ts:128` | StringLiteral | Kapıya asılı 3 sözcüklük "yanına al" listesi. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0481 | `data/bgm.ts:129` | StringLiteral | Sözcük başına 1 tekrar hakkı; düzeltme değil, işaretleme + birlikte inceleme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0482 | `data/bgm.ts:130` | StringLiteral | Hata sınıfı trendi telemetriye işlenir; bant/eşik üretilmez (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0483 | `data/bgm.ts:132` | StringLiteral | 6 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0484 | `data/bgm.ts:133` | StringLiteral | yazım yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0485 | `data/bgm.ts:133` | StringLiteral | hata sınıfı kartları (4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0486 | `data/bgm.ts:134` | StringLiteral | model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0487 | `data/bgm.ts:136` | StringLiteral | MEB ÖGG Gözlem Formu Yazma m.2/5/6/7 · DEP 1.4 (yapı atfı; K-08) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0488 | `data/bgm.ts:139` | StringLiteral | Akıcı Okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0489 | `data/bgm.ts:139` | StringLiteral | Tekrarlı okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0490 | `data/bgm.ts:140` | StringLiteral | Akıcılık (D-L2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0491 | `data/bgm.ts:141` | StringLiteral | Hedef metinde tekrarlı okuma; doğru sözcük/dk kaydı + M-4 veli işaretleme köprüsü. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0492 | `data/bgm.ts:142` | StringLiteral | Akıcılık turunu ev-okul ortak kaydıyla (M-4) izlenebilir kılmak. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0493 | `data/bgm.ts:143` | StringLiteral | Doğru sözcük/dk (doğru×60/sn) · tur içi kazanım. Bant/eşik YOK (K-02). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0494 | `data/bgm.ts:144` | StringLiteral | Tanıt (uzman okur) → 2–3 tekrarlı tur (süre tutulur) → M-4 formu hazırlanır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0495 | `data/bgm.ts:145` | StringLiteral | Günde 5–10 dk sesli okuma (AG-2); M-4 formuna işaret. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0496 | `data/bgm.ts:146` | StringLiteral | Metin bant düzeyi çocuğun düzeyine göre; zorlayıcı metin seçilmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0497 | `data/bgm.ts:147` | StringLiteral | M-4 ev kaydı ile seans verisi aynı zaman çizgisinde karşılaştırılır (yalnız uzman). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0498 | `data/bgm.ts:149` | StringLiteral | 8–10 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0499 | `data/bgm.ts:150` | StringLiteral | hedef metin (bantlı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0500 | `data/bgm.ts:150` | StringLiteral | süre sayacı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0501 | `data/bgm.ts:150` | StringLiteral | M-4 formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0502 | `data/bgm.ts:151` | StringLiteral | eşli okuma → tek başına (süre tutulur) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0503 | `data/bgm.ts:153` | StringLiteral | D-L2 tekrarlı okuma · MEB akıcılık formülü (2025 kit deseni; K-08) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0504 | `data/bgm.ts:156` | StringLiteral | Sözcük Çantası | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0505 | `data/bgm.ts:156` | StringLiteral | Kelime dağarcığı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0506 | `data/bgm.ts:157` | StringLiteral | Sözcük dağarcığı (DEP M2.2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0507 | `data/bgm.ts:158` | StringLiteral | Günün 5 yeni sözcüğünün anlam + üretim döngüsüyle kalıcı belleğe taşınması. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0508 | `data/bgm.ts:159` | StringLiteral | Sözcüğü tanıma → üretim → tekrar üçlüsüyle izlemek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0509 | `data/bgm.ts:160` | StringLiteral | Üretim isabeti (0–3) · tekrar turunda geri çağırma (betimleyici). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0510 | `data/bgm.ts:161` | StringLiteral | Çantaya ekleme → anlam kartı → "çantadan al, cümleye koy" üretimi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0511 | `data/bgm.ts:162` | StringLiteral | Yarının 5 sözcüğü akşam yemeğinde cümle içinde kullanılır. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0512 | `data/bgm.ts:163` | StringLiteral | Sözcük sayısı 5 ile sınırlı; aşırı yükleme yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0513 | `data/bgm.ts:164` | StringLiteral | Çanta içeriği veliyle paylaşılır; karşılaştırma dili yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0514 | `data/bgm.ts:166` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0515 | `data/bgm.ts:167` | StringLiteral | sözcük kartları (5) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0516 | `data/bgm.ts:167` | StringLiteral | çanta görseli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0517 | `data/bgm.ts:168` | StringLiteral | model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0518 | `data/bgm.ts:170` | StringLiteral | 2021 DEP M2.2 (sözcük dağarcığı) · LEXIVA kelime görevi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0519 | `data/bgm.ts:173` | StringLiteral | Anlama Kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0520 | `data/bgm.ts:173` | StringLiteral | Okudunu söyle | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0521 | `data/bgm.ts:175` | StringLiteral | Kısa bantlı metin okuma/dinleme sonrası 3 soruda (ne/kim/nerede) anlamı ifade etme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0522 | `data/bgm.ts:176` | StringLiteral | Anlamanın sözel ayağını (ifade) kısa ve güven veren biçimde izlemek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0523 | `data/bgm.ts:177` | StringLiteral | Anlama kartı isabeti (E/H) · cümleyle ifade (gözlem). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0524 | `data/bgm.ts:178` | StringLiteral | 4–5 cümlelik metin (2 geçiş) → 3 anlama kartı; her kart 1 cümle. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0525 | `data/bgm.ts:179` | StringLiteral | Evde okunan kitap için 1 soru (aile sorusu). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0526 | `data/bgm.ts:180` | StringLiteral | Uzun yanıt beklenmez; 1 cümle yeterli (Z-15 dili). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0527 | `data/bgm.ts:181` | StringLiteral | Anlama zorlanmasında metin bant düzeyi gözden geçirilir (uzman). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0528 | `data/bgm.ts:183` | StringLiteral | 6 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0529 | `data/bgm.ts:184` | StringLiteral | kısa metin kartı (bantlı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0530 | `data/bgm.ts:184` | StringLiteral | anlama kartları (3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0531 | `data/bgm.ts:185` | StringLiteral | model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0532 | `data/bgm.ts:187` | StringLiteral | D-L2 anlama alt ayağı · LEXIVA anlama görevi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0533 | `data/bgm.ts:190` | StringLiteral | Sayı Blokları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0534 | `data/bgm.ts:190` | StringLiteral | Çokluk ve karıştırma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0535 | `data/bgm.ts:191` | StringLiteral | Matematik (D-L4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0536 | `data/bgm.ts:192` | StringLiteral | Çokluk-sayı eşlemesi + karıştırma çiftleri (6/9, 1/7) ayırt etme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0537 | `data/bgm.ts:193` | StringLiteral | Somuttan soyuta köprüyü ve karıştırma seçiciliğini izlemek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0538 | `data/bgm.ts:194` | StringLiteral | Eşleme isabeti (E/H) · karıştırma çifti hata adedi (betimleyici). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0539 | `data/bgm.ts:195` | StringLiteral | 8 blok say → sayı kartıyla eşle; "6 mı 9 mu?" karıştırma çifti kartları. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0540 | `data/bgm.ts:196` | StringLiteral | Yemek masasında "kaç tabak?" sayma pratiği. Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0541 | `data/bgm.ts:197` | StringLiteral | Karıştırım çiftinde somut blok gösterilir; sözel onay ile pekiştirme. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0542 | `data/bgm.ts:198` | StringLiteral | Sayı blokları telemetrisi MENTORIA raporuna işlenir (yalnız uzman yorumu). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0543 | `data/bgm.ts:200` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0544 | `data/bgm.ts:201` | StringLiteral | sayı blokları (8) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0545 | `data/bgm.ts:201` | StringLiteral | sayı kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0546 | `data/bgm.ts:201` | StringLiteral | karıştırma çifti kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0547 | `data/bgm.ts:202` | StringLiteral | model → isaret → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0548 | `data/bgm.ts:204` | StringLiteral | 2021 DEP 4.3/5.1 · ÖGG Gözlem Formu Mat m.3 (yapı atfı; K-08) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0549 | `data/bgm.ts:207` | StringLiteral | Süre Algısı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0550 | `data/bgm.ts:207` | StringLiteral | Süre tahmini | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0551 | `data/bgm.ts:208` | StringLiteral | Süre tahmini (seans içi) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0552 | `data/bgm.ts:209` | StringLiteral | Bir işin ne kadar süreceğini tahmin etme ve gerçek süreyle karşılaştırma. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0553 | `data/bgm.ts:210` | StringLiteral | “Az kaldı / çok kaldı” hissini sayılabilir süreyle eşlemek (seans içi süre; takvim değil). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0554 | `data/bgm.ts:211` | StringLiteral | Tahmin − gerçek süre farkı (sn). Persona “Süre Algısı (Ritim)” ile aynı aile. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0555 | `data/bgm.ts:212` | StringLiteral | Kum saati tahmini: uzman 30/60/90 sn tutar, çocuk işaretler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0556 | `data/bgm.ts:213` | StringLiteral | Akşam rutininin bir adımına süre koyun (ör. çanta hazırlığı). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0557 | `data/bgm.ts:214` | StringLiteral | Görünür analog saat veya kum saati; "acele et" yerine süre göstergesi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0558 | `data/bgm.ts:215` | StringLiteral | Geçiş uyarısı (Z-13) seans bitimine 5 ve 1 dk kala — utançsız dil. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0559 | `data/bgm.ts:217` | StringLiteral | 5 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0560 | `data/bgm.ts:218` | StringLiteral | kum saati / analog kronometre | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0561 | `data/bgm.ts:218` | StringLiteral | tahmin kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0562 | `data/bgm.ts:219` | StringLiteral | görsel sayaç açık → yarı kapalı → kapalı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0563 | `data/bgm.ts:221` | StringLiteral | süre tahmini görev ailesı · PMC 5-küme ③ rutin-zamanlama (literatür atfı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0564 | `data/bgm.ts:224` | StringLiteral | Transfer ve Serbest Okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0565 | `data/bgm.ts:224` | StringLiteral | Yeni metine taşıma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0566 | `data/bgm.ts:225` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0567 | `data/bgm.ts:225` | StringLiteral | Aktarım (D-L7) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0568 | `data/bgm.ts:226` | StringLiteral | Kazanılan okuma becerisinin farklı metin/ortam/kişiye taşınma gözlemi (T2/T3). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0569 | `data/bgm.ts:227` | StringLiteral | Kazanımın yeni metin türlerinde (serbest okuma, günlük) ortaya çıkmasını izlemek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0570 | `data/bgm.ts:228` | StringLiteral | Yeni metinde akıcılık (doğru sözcük/dk) · Transfer Gözlem Kartı notu (uzman). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0571 | `data/bgm.ts:229` | StringLiteral | Bant dışı kısa metinlerle serbest okuma turları; çocuk kendi metnini seçer. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0572 | `data/bgm.ts:230` | StringLiteral | Kendi seçtiği kitapla 10 dk sesli okuma (AG-2). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0573 | `data/bgm.ts:231` | StringLiteral | Yeni metinde zorlanma olursa bant düzeyine dönülür (yükleme artırmaz). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0574 | `data/bgm.ts:232` | StringLiteral | Transfer kartı MENTORIA rapor akışına besler (BATARYA §5). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0575 | `data/bgm.ts:234` | StringLiteral | 6–8 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0576 | `data/bgm.ts:235` | StringLiteral | serbest okuma metinleri (bant dışı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0577 | `data/bgm.ts:235` | StringLiteral | transfer gözlem kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0578 | `data/bgm.ts:236` | StringLiteral | uzman yanımda → aynı odada → ayrı (kademeli) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0579 | `data/bgm.ts:238` | StringLiteral | D-L7 aktarım ayağı · LEXIVA serbest okuma görevi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0580 | `data/bgm.ts:241` | StringLiteral | Okuma Özerkliği | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0581 | `data/bgm.ts:241` | StringLiteral | Dış iskeleti solma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0582 | `data/bgm.ts:242` | StringLiteral | III | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0583 | `data/bgm.ts:242` | StringLiteral | Üstbiliş / otonomi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0584 | `data/bgm.ts:243` | StringLiteral | Hazır görevi çocuğun kendi planlaması; hatırlatıcı kademeli azalır (metakognisyon ONAYLI konum). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0585 | `data/bgm.ts:244` | StringLiteral | Platform iskeletini solmak; günlük 10 dk sesli okuma rutinine (AG-2) yerleştirmek. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0586 | `data/bgm.ts:245` | StringLiteral | Hatırlatıcısız başlama (E/H) · planladığı okumaya dönüş. Öz-başlatma betimleyicidir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0587 | `data/bgm.ts:246` | StringLiteral | Çocuk bugünkü gerçek işini (kitap/ödev) planlar; uzman yalnız izler, ipucu isterse verir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0588 | `data/bgm.ts:247` | StringLiteral | Kendi yazdığı 3 kutuluk planı odasına asmak (yazılı plan kavramı). Puan yok. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0589 | `data/bgm.ts:248` | StringLiteral | Karşılaştırma dili yok; her geribildirimde en az bir güçlü yön (Z-15). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0590 | `data/bgm.ts:249` | StringLiteral | Sistem otonomi ilan etmez; karar uzman + ailededir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0591 | `data/bgm.ts:251` | StringLiteral | 8–10 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0592 | `data/bgm.ts:252` | StringLiteral | 3 kutulu plan kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0593 | `data/bgm.ts:252` | StringLiteral | çocuğun kendi kitabı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0594 | `data/bgm.ts:253` | StringLiteral | istek üzerine → yok | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0595 | `data/bgm.ts:255` | StringLiteral | metakognisyon konumlandırma v1.0 (K-118/119) · ipucu silikleştirme deseni | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0596 | `data/bgm.ts:261` | StringLiteral | Okuma menüsü (12), DEP-2021'in yerine geçmez. DEP = BEP/RAM saat hizası; menü = okuma/fonolojik içerik. Uzman ikisinden de seçer. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0597 | `data/bgm.ts:265` | StringLiteral | Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0598 | `data/kisitlar.ts:8` | StringLiteral | Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0599 | `data/kisitlar.ts:10` | StringLiteral | Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0600 | `data/kisitlar.ts:12` | StringLiteral | Rapor taslaktır; uzman onayı olmadan geçerli belge değildir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0601 | `data/kisitlar.ts:16` | StringLiteral | Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0602 | `data/kisitlar.ts:17` | StringLiteral | Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0603 | `data/kisitlar.ts:18` | StringLiteral | TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0604 | `data/kisitlar.ts:19` | StringLiteral | Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296). | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0605 | `data/kisitlar.ts:20` | StringLiteral | Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0606 | `data/kisitlar.ts:21` | StringLiteral | LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0607 | `data/kisitlar.ts:26` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0608 | `data/kisitlar.ts:27` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0609 | `data/kisitlar.ts:28` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0610 | `data/kisitlar.ts:29` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0611 | `data/kisitlar.ts:31` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0612 | `data/kisitlar.ts:34` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0613 | `data/kisitlar.ts:38` | StringLiteral | x / + | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0614 | `data/kisitlar.ts:38` | StringLiteral | x: hedeflenen · +: ulaşılan (PKF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0615 | `data/kisitlar.ts:39` | StringLiteral | ölçüt düzeyi (PBF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0616 | `data/kisitlar.ts:40` | StringLiteral | Evet / Hayır | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0617 | `data/kisitlar.ts:40` | StringLiteral | gözlendi / gözlenmedi (KDF deseni) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0618 | `data/kisitlar.ts:44` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0619 | `data/kisitlar.ts:44` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0620 | `data/kisitlar.ts:55` | StringLiteral | Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0621 | `data/kisitlar.ts:59` | StringLiteral | Devam/yoklama takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0622 | `data/kisitlar.ts:59` | StringLiteral | BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0623 | `data/kisitlar.ts:60` | StringLiteral | Ödeme · fatura · idari-mali işleyiş | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0624 | `data/kisitlar.ts:60` | StringLiteral | K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0625 | `data/kisitlar.ts:61` | StringLiteral | Resmî form üretimi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0626 | `data/kisitlar.ts:61` | StringLiteral | K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0627 | `data/kisitlar.ts:76` | StringLiteral | Ölçüt Bağımlı Test (ÖBT) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0628 | `data/kisitlar.ts:76` | StringLiteral | ilk / ara / son değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0629 | `data/kisitlar.ts:77` | StringLiteral | Tekrar ve deneme sayısı → Ölçüt alanı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0630 | `data/kisitlar.ts:77` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0631 | `data/kisitlar.ts:78` | StringLiteral | Kontrol Listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0632 | `data/kisitlar.ts:78` | StringLiteral | ilk / ara / son değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0633 | `data/kisitlar.ts:79` | StringLiteral | Evet/Hayır girdileri → Açıklamalar sütunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0634 | `data/kisitlar.ts:79` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0635 | `data/kisitlar.ts:80` | StringLiteral | Dereceli Puanlama Anahtarı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0636 | `data/kisitlar.ts:80` | StringLiteral | değerlendirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0637 | `data/kisitlar.ts:81` | StringLiteral | 0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0638 | `data/kisitlar.ts:81` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0639 | `data/kisitlar.ts:82` | StringLiteral | Performans Kayıt Formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0640 | `data/kisitlar.ts:82` | StringLiteral | her modülün başı ve sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0641 | `data/kisitlar.ts:83` | StringLiteral | x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0642 | `data/kisitlar.ts:83` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0643 | `data/kisitlar.ts:84` | StringLiteral | BEP Gelişimi İzleme Özet Formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0644 | `data/kisitlar.ts:84` | StringLiteral | süreç + yıl sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0645 | `data/kisitlar.ts:85` | StringLiteral | Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0646 | `data/kisitlar.ts:85` | StringLiteral | kanıt | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0647 | `data/kisitlar.ts:86` | StringLiteral | Portfolyo Kontrol Listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0648 | `data/kisitlar.ts:86` | StringLiteral | modül sonu / yıl sonu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0649 | `data/kisitlar.ts:87` | StringLiteral | Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0650 | `data/kisitlar.ts:88` | StringLiteral | Portfolyo Dereceli Puanlama Anahtarı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0651 | `data/kisitlar.ts:88` | StringLiteral | portfolyo değ. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0652 | `data/kisitlar.ts:89` | StringLiteral | kapsam dışı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0653 | `data/kisitlar.ts:94` | StringLiteral | (a) Ücreti Bakanlıkça karşılanan | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0654 | `data/kisitlar.ts:94` | StringLiteral | ZORUNLU (rapor + ÖEDK planı + BKDS onamı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0655 | `data/kisitlar.ts:95` | StringLiteral | ÖEDK eğitim planı ekseninde | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0656 | `data/kisitlar.ts:96` | StringLiteral | (b) Ücretini kendisi/velisi karşılayan | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0657 | `data/kisitlar.ts:96` | StringLiteral | İSTENMİYOR | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0658 | `data/kisitlar.ts:97` | StringLiteral | Kayıttaki ölçme sonuçlarıyla BEP birimince (md.24/6 · md.26/3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0659 | `data/kisitlar.ts:103` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0660 | `data/kisitlar.ts:103` | StringLiteral | Tüm dosyalar · rapor onayı · dışa aktarma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0661 | `data/kisitlar.ts:104` | StringLiteral | Uzman / Eğitimci | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0662 | `data/kisitlar.ts:104` | StringLiteral | Kendi dosyaları · oturum · girdi · rapor taslağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0663 | `data/mock.ts:6` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0664 | `data/mock.ts:6` | StringLiteral | Öğrenci A. (2. Sınıf) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0665 | `data/mock.ts:6` | StringLiteral | Atatürk İlkokulu / 2-B | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0666 | `data/mock.ts:7` | StringLiteral | Son ayda 2 gün | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0667 | `data/mock.ts:7` | StringLiteral | RAM eğitsel değerlendirme mevcut (2025) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0668 | `data/mock.ts:8` | StringLiteral | Veli A. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0669 | `data/mock.ts:8` | StringLiteral | 05xx xxx 41 17 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0670 | `data/mock.ts:8` | StringLiteral | İzmir / Bornova | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0671 | `data/mock.ts:9` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0672 | `data/mock.ts:9` | StringLiteral | Öğrenci B. (3. Sınıf) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0673 | `data/mock.ts:9` | StringLiteral | Cumhuriyet İlkokulu / 3-A | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0674 | `data/mock.ts:10` | StringLiteral | BEP dosyası okuldan bekleniyor | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0675 | `data/mock.ts:11` | StringLiteral | Veli B. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0676 | `data/mock.ts:11` | StringLiteral | 05xx xxx 29 03 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0677 | `data/mock.ts:11` | StringLiteral | İzmir / Karşıyaka | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0678 | `data/mock.ts:15` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0679 | `data/mock.ts:15` | StringLiteral | Haftada 1 (40 dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0680 | `data/mock.ts:16` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0681 | `data/mock.ts:17` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0682 | `data/mock.ts:17` | StringLiteral | Haftada 1 (40 dk) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0683 | `data/mock.ts:18` | StringLiteral | DEP-2026 (ORGM 2026_01) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0684 | `data/mock.ts:22` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0685 | `data/mock.ts:22` | StringLiteral | tamamlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0686 | `data/mock.ts:23` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0687 | `data/mock.ts:23` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0688 | `data/mock.ts:24` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0689 | `data/mock.ts:24` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0690 | `data/mock.ts:25` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0691 | `data/mock.ts:29` | StringLiteral | Hece ayırma çalışması | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0692 | `data/mock.ts:29` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0693 | `data/mock.ts:30` | StringLiteral | Sözel ipucu → model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0694 | `data/mock.ts:30` | StringLiteral | hece kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0695 | `data/mock.ts:30` | StringLiteral | çalışma yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0696 | `data/mock.ts:30` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0697 | `data/mock.ts:31` | StringLiteral | Sesli okuma — tekrarlı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0698 | `data/mock.ts:31` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0699 | `data/mock.ts:32` | StringLiteral | Eşli okuma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0700 | `data/mock.ts:32` | StringLiteral | kısa metin | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0701 | `data/mock.ts:32` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0702 | `data/mock.ts:33` | StringLiteral | Görsel dikkat eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0703 | `data/mock.ts:33` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0704 | `data/mock.ts:34` | StringLiteral | İşaret → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0705 | `data/mock.ts:34` | StringLiteral | eşleme kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0706 | `data/mock.ts:34` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0707 | `data/mock.ts:35` | StringLiteral | İşitsel bellek dizisi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0708 | `data/mock.ts:35` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0709 | `data/mock.ts:36` | StringLiteral | Model → gecikmeli model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0710 | `data/mock.ts:36` | StringLiteral | ses kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0711 | `data/mock.ts:36` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0712 | `data/mock.ts:37` | StringLiteral | Sözcük dağarcığı — nesne adlandırma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0713 | `data/mock.ts:37` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0714 | `data/mock.ts:38` | StringLiteral | Fiziksel ipucu → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0715 | `data/mock.ts:38` | StringLiteral | nesne resimleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0716 | `data/mock.ts:38` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0717 | `data/mock.ts:39` | StringLiteral | Nesne niteliği ayırt etme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0718 | `data/mock.ts:39` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0719 | `data/mock.ts:40` | StringLiteral | Model → kısmi ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0720 | `data/mock.ts:40` | StringLiteral | blok seti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0721 | `data/mock.ts:40` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0722 | `data/mock.ts:41` | StringLiteral | Ritmik sayma (100 içinde) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0723 | `data/mock.ts:42` | StringLiteral | Birlikte sayma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0724 | `data/mock.ts:42` | StringLiteral | sayı doğrusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0725 | `data/mock.ts:42` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0726 | `data/mock.ts:43` | StringLiteral | Sıra alma ve bekleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0727 | `data/mock.ts:43` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0728 | `data/mock.ts:44` | StringLiteral | Model → sözel hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0729 | `data/mock.ts:44` | StringLiteral | sıra kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0730 | `data/mock.ts:44` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0731 | `data/mock.ts:44` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0732 | `data/mock.ts:46` | StringLiteral | Sürdürülebilir dikkat — nesne takibi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0733 | `data/mock.ts:46` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0734 | `data/mock.ts:47` | StringLiteral | Model → sözel ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0735 | `data/mock.ts:47` | StringLiteral | renkli toplar | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0736 | `data/mock.ts:47` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0737 | `data/mock.ts:48` | StringLiteral | Yönerge izleme (2 adımlı) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0738 | `data/mock.ts:48` | StringLiteral | Öğrenmeye Destek | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0739 | `data/mock.ts:49` | StringLiteral | Fiziksel rehber → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0740 | `data/mock.ts:49` | StringLiteral | yönerge kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0741 | `data/mock.ts:49` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0742 | `data/mock.ts:50` | StringLiteral | Dinlediğini anlama — kısa öykü | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0743 | `data/mock.ts:50` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0744 | `data/mock.ts:51` | StringLiteral | Sözel ipucu → soru-cevap → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0745 | `data/mock.ts:51` | StringLiteral | öykü kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0746 | `data/mock.ts:51` | StringLiteral | soru listesi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0747 | `data/mock.ts:51` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0748 | `data/mock.ts:52` | StringLiteral | Sözel ifade — cümle kurma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0749 | `data/mock.ts:52` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0750 | `data/mock.ts:53` | StringLiteral | Model cümle → tamamlama → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0751 | `data/mock.ts:53` | StringLiteral | kelime kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0752 | `data/mock.ts:53` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0753 | `data/mock.ts:54` | StringLiteral | Karşılıklı konuşma sürdürme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0754 | `data/mock.ts:54` | StringLiteral | Dil ve İletişim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0755 | `data/mock.ts:55` | StringLiteral | Sözel başlatma → sıra alma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0756 | `data/mock.ts:55` | StringLiteral | konu kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0757 | `data/mock.ts:55` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0758 | `data/mock.ts:55` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0759 | `data/mock.ts:56` | StringLiteral | Harf-ses eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0760 | `data/mock.ts:56` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0761 | `data/mock.ts:57` | StringLiteral | Model → eşleme → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0762 | `data/mock.ts:57` | StringLiteral | harf kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0763 | `data/mock.ts:57` | StringLiteral | ses kutusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0764 | `data/mock.ts:57` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0765 | `data/mock.ts:58` | StringLiteral | Yazma — harf dikte | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0766 | `data/mock.ts:58` | StringLiteral | Okuma ve Yazma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0767 | `data/mock.ts:59` | StringLiteral | Noktalı iz → kopya → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0768 | `data/mock.ts:59` | StringLiteral | dikte yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0769 | `data/mock.ts:59` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0770 | `data/mock.ts:60` | StringLiteral | Gruplama / sınıflama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0771 | `data/mock.ts:60` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0772 | `data/mock.ts:61` | StringLiteral | Model → sözel ipucu → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0773 | `data/mock.ts:61` | StringLiteral | sınıflama kutuları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0774 | `data/mock.ts:61` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0775 | `data/mock.ts:62` | StringLiteral | Birebir eşleştirme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0776 | `data/mock.ts:62` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0777 | `data/mock.ts:63` | StringLiteral | Fiziksel rehber → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0778 | `data/mock.ts:63` | StringLiteral | eş kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0779 | `data/mock.ts:63` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0780 | `data/mock.ts:64` | StringLiteral | Sıralama (büyük-küçük) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0781 | `data/mock.ts:64` | StringLiteral | Erken Matematik | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0782 | `data/mock.ts:65` | StringLiteral | Model → deneme-yanılma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0783 | `data/mock.ts:65` | StringLiteral | sıralama şeridi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0784 | `data/mock.ts:65` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0785 | `data/mock.ts:66` | StringLiteral | Sayı doğrusu ile toplama | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0786 | `data/mock.ts:67` | StringLiteral | Model → rehberli → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0787 | `data/mock.ts:67` | StringLiteral | sayı doğrusu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0788 | `data/mock.ts:67` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0789 | `data/mock.ts:68` | StringLiteral | Çıkarma (nesne ile) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0790 | `data/mock.ts:69` | StringLiteral | Nesne desteği → zihinden | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0791 | `data/mock.ts:69` | StringLiteral | sayma pulları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0792 | `data/mock.ts:69` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0793 | `data/mock.ts:70` | StringLiteral | Günlük yaşam problemi kurma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0794 | `data/mock.ts:71` | StringLiteral | Sözel senaryo → model → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0795 | `data/mock.ts:71` | StringLiteral | problem kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0796 | `data/mock.ts:71` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0797 | `data/mock.ts:72` | StringLiteral | Duygu tanıma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0798 | `data/mock.ts:72` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0799 | `data/mock.ts:73` | StringLiteral | Görsel ipucu → eşleme → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0800 | `data/mock.ts:73` | StringLiteral | duygu kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0801 | `data/mock.ts:73` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0802 | `data/mock.ts:74` | StringLiteral | İş birliği oyunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0803 | `data/mock.ts:74` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0804 | `data/mock.ts:75` | StringLiteral | Eşli oyun → sıra alma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0805 | `data/mock.ts:75` | StringLiteral | kutu oyunu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0806 | `data/mock.ts:75` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0807 | `data/mock.ts:76` | StringLiteral | Kurala uyma (oyun) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0808 | `data/mock.ts:76` | StringLiteral | Sosyal Etkileşim | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0809 | `data/mock.ts:77` | StringLiteral | Model → hatırlatma → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0810 | `data/mock.ts:77` | StringLiteral | kural kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0811 | `data/mock.ts:77` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0812 | `data/mock.ts:80` | StringLiteral | BGM — Ses Merdiveni (Fonolojik Eşleme) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0813 | `data/mock.ts:80` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0814 | `data/mock.ts:80` | StringLiteral | merdiven şeması | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0815 | `data/mock.ts:80` | StringLiteral | ses kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0816 | `data/mock.ts:80` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0817 | `data/mock.ts:80` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0818 | `data/mock.ts:81` | StringLiteral | BGM — Ses Birimi Ayırt Etme (SBA Turu) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0819 | `data/mock.ts:81` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0820 | `data/mock.ts:81` | StringLiteral | ekran (SBA) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0821 | `data/mock.ts:81` | StringLiteral | ses kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0822 | `data/mock.ts:81` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0823 | `data/mock.ts:82` | StringLiteral | BGM — Hece ve Parçalar (El Çırparak Heceleme) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0824 | `data/mock.ts:82` | StringLiteral | Model (uzman bölür) → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0825 | `data/mock.ts:82` | StringLiteral | hece kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0826 | `data/mock.ts:82` | StringLiteral | parçalama şeridi | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0827 | `data/mock.ts:82` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0828 | `data/mock.ts:83` | StringLiteral | BGM — Harf Tanıma ve Çizim (b/d-l İzleme) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0829 | `data/mock.ts:83` | StringLiteral | Fiziksel izleme → model → sözel | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0830 | `data/mock.ts:83` | StringLiteral | büyük puntolu sayfa | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0831 | `data/mock.ts:83` | StringLiteral | harf kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0832 | `data/mock.ts:83` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0833 | `data/mock.ts:84` | StringLiteral | BGM — Söyleneni Yaz (Hata Sınıfı ile) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0834 | `data/mock.ts:84` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0835 | `data/mock.ts:84` | StringLiteral | yazım yaprağı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0836 | `data/mock.ts:84` | StringLiteral | hata sınıfı kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0837 | `data/mock.ts:84` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0838 | `data/mock.ts:85` | StringLiteral | BGM — Akıcı Okuma (Tekrarlı + M-4) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0839 | `data/mock.ts:85` | StringLiteral | Eşli okuma → tek başına | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0840 | `data/mock.ts:85` | StringLiteral | hedef metin | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0841 | `data/mock.ts:85` | StringLiteral | süre sayacı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0842 | `data/mock.ts:85` | StringLiteral | M-4 formu | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0843 | `data/mock.ts:85` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0844 | `data/mock.ts:86` | StringLiteral | BGM — Sözcük Çantası (Günün 5 Sözcüğü) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0845 | `data/mock.ts:86` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0846 | `data/mock.ts:86` | StringLiteral | sözcük kartları (5) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0847 | `data/mock.ts:86` | StringLiteral | çanta görseli | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0848 | `data/mock.ts:86` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0849 | `data/mock.ts:87` | StringLiteral | BGM — Anlama Kartı (Okudunu Söyle) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0850 | `data/mock.ts:87` | StringLiteral | Model → sözel → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0851 | `data/mock.ts:87` | StringLiteral | kısa metin kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0852 | `data/mock.ts:87` | StringLiteral | anlama kartları (3) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0853 | `data/mock.ts:87` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0854 | `data/mock.ts:88` | StringLiteral | BGM — Sayı Blokları (Çokluk + Karıştırma Çifti) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0855 | `data/mock.ts:88` | StringLiteral | Model → isaret → bağımsız | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0856 | `data/mock.ts:88` | StringLiteral | sayı blokları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0857 | `data/mock.ts:88` | StringLiteral | sayı kartları | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0858 | `data/mock.ts:88` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0859 | `data/mock.ts:89` | StringLiteral | BGM — Süre Algısı (Kum Saati Tahmini) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0860 | `data/mock.ts:89` | StringLiteral | Görsel sayaç açık → yarı kapalı → kapalı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0861 | `data/mock.ts:89` | StringLiteral | kum saati | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0862 | `data/mock.ts:89` | StringLiteral | tahmin kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0863 | `data/mock.ts:89` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0864 | `data/mock.ts:90` | StringLiteral | BGM — Transfer ve Serbest Okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0865 | `data/mock.ts:90` | StringLiteral | Uzman yanımda → aynı odada → ayrı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0866 | `data/mock.ts:90` | StringLiteral | serbest okuma metinleri | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0867 | `data/mock.ts:90` | StringLiteral | transfer kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0868 | `data/mock.ts:90` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0869 | `data/mock.ts:91` | StringLiteral | BGM — Okuma Özerkliği (Kendi Planım) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0870 | `data/mock.ts:91` | StringLiteral | İstek üzerine → yok | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0871 | `data/mock.ts:91` | StringLiteral | 3 kutulu plan kartı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0872 | `data/mock.ts:91` | StringLiteral | çocuğun kendi kitabı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0873 | `data/mock.ts:91` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0874 | `data/mock.ts:101` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0875 | `data/mock.ts:101` | StringLiteral | Seans Özeti — 03.09.2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0876 | `data/mock.ts:103` | StringLiteral | Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0877 | `data/mock.ts:104` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0878 | `data/mock.ts:104` | StringLiteral | Aylık Gelişim Özeti — Ağustos 2026 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0879 | `data/mock.ts:105` | StringLiteral | Yönetici | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0880 | `data/mock.ts:106` | StringLiteral | Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0881 | `data/mock.ts:107` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0882 | `data/mock.ts:107` | StringLiteral | Dönem Sonu Değerlendirme — 2026 Güz | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0883 | `data/mock.ts:109` | StringLiteral | Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0884 | `data/mock.ts:110` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0885 | `data/mock.ts:110` | StringLiteral | BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0886 | `data/mock.ts:112` | StringLiteral | Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0887 | `data/mock.ts:113` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0888 | `data/mock.ts:113` | StringLiteral | RAM İzleme Paketi Hazırlığı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0889 | `data/mock.ts:115` | StringLiteral | Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM'a iletilir; iki kopya üretilir. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0890 | `data/mock.ts:116` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0891 | `data/mock.ts:116` | StringLiteral | Aile Bilgilendirme Çıktısı — Eylül | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0892 | `data/mock.ts:117` | StringLiteral | Uzman / Eğitimci | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0893 | `data/mock.ts:118` | StringLiteral | Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0894 | `data/mock.ts:122` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0895 | `data/mock.ts:122` | StringLiteral | Mutfakta hece avı (5 nesne) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0896 | `data/mock.ts:123` | StringLiteral | Hafta içi 3 gün · 10 dk | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0897 | `data/mock.ts:123` | StringLiteral | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0898 | `data/mock.ts:123` | StringLiteral | Çocuk istekliydi; 4 nesne bağımsız heceledi. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0899 | `data/mock.ts:124` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0900 | `data/mock.ts:124` | StringLiteral | Gazete başlığı okuma | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0901 | `data/mock.ts:125` | StringLiteral | Hafta sonu · 1 kez | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0902 | `data/mock.ts:126` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0903 | `data/mock.ts:126` | StringLiteral | Sayı kartlarıyla eşleme | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0904 | `data/mock.ts:127` | StringLiteral | Hafta içi 2 gün | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0905 | `data/mock.ts:127` | StringLiteral | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0906 | `data/mock.ts:127` | StringLiteral | Aile yoğunluk bildirdi; süre kısaltıldı. | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0907 | `data/mock.ts:131` | StringLiteral | ÖĞR-4417 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0908 | `data/mock.ts:132` | StringLiteral | İlk İnceleme tamamlandı (e-Rehberlik) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0909 | `data/mock.ts:133` | StringLiteral | ÖĞR-2903 | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0910 | `data/mock.ts:134` | StringLiteral | (b) hattı — RAM raporu istenmiyor (ÖEKY md.20/2) | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0911 | `data/tipler.ts:11` | StringLiteral | yapıldı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0912 | `data/tipler.ts:11` | StringLiteral | yapılmadı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0913 | `data/tipler.ts:29` | StringLiteral | DEP | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0914 | `data/tipler.ts:29` | StringLiteral | BGM | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0915 | `data/tipler.ts:42` | StringLiteral | planlandı | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |
| SUP-LEX-0916 | `data/tipler.ts:42` | StringLiteral | gerçekleşti | Kaynak adayı; koşullu görünürlük DOM/çağrıyla teyit edilir |

## Tam16 TS/TSX kaynak dosyası

Bu bölüm UI listesi değil; teknik alan/yorum/kullanılmayan kod ayrımı korunmalıdır. Satır numarası her bloğun ilk satırından başlar.

### `App.tsx`
3244 B ·SHA `68126594428514f6a75e8e87c52d2c94165981253c51ee4ea4ac6003e3cb7a7f`

~~~~tsx
import { useState } from 'react';
import Kabuk, { type EkranId } from './components/Kabuk';
import { Pano, Dosyalar, Takvim, OturumAtolyesi, Cizelge, RaporAtolyesi, Hizalama, Aile, Ayarlar, RamBep, EvOdevleri, EtkinlikKatalogu, BgmMenu } from './components/Ekranlar';
import { ROLLER, type RolId } from './data/kisitlar';

export default function App() {
  const [ekran, setEkran] = useState<EkranId>('pano');
  const [rol, setRol] = useState<RolId | null>(null);

  // Rol seçimi (spec §4-①). VELİ ROLÜ YOKTUR (K-296/KC7).
  if (!rol) {
    return (
      <div className="min-h-screen grid place-items-center p-6">
        <div className="max-w-lg w-full bg-white rounded-3xl border border-slate-200 p-8 space-y-5">
          <div className="text-center space-y-1">
            <div className="w-12 h-12 rounded-2xl bg-teal-600 text-white grid place-items-center font-black text-xl mx-auto">S</div>
            <h1 className="text-xl font-black">LEXIVA Supporta™ MVP (Adaptif Eğitimsel Destek Ekosistemi)</h1>
            <p className="text-xs text-slate-500">Özel eğitim merkezi uzman kokpiti · v{__SURUM__}</p>
          </div>
          <p className="text-sm text-slate-600 text-center">Devam etmek için rolünüzü seçin.</p>
          <div className="grid gap-2">
            {ROLLER.map((r) => (
              <button key={r.id} type="button" data-testid={`rol-${r.id}`} onClick={() => setRol(r.id)}
                className="text-left px-4 py-3 rounded-2xl border-2 border-slate-200 hover:border-teal-500 transition-colors">
                <div className="font-bold text-sm">{r.ad}</div>
                <div className="text-xs text-slate-500">{r.yetki}</div>
              </button>
            ))}
          </div>
          <p data-testid="veli-yok" className="text-[11px] text-slate-500 text-center border-t border-slate-100 pt-3">
            Veli rolü bulunmamaktadır: veli bilgilendirilen taraftır, sisteme giriş yapmaz (K-296).
          </p>
        </div>
      </div>
    );
  }
  const rolAd = ROLLER.find((r) => r.id === rol)!.ad;
  // üç-sınıf taksonomi (K-251): __PILOT__ kısıtlı, __TAM__ tam ürün, ikisi false ise DEMO
  const modEtiket = (typeof __PILOT__ !== 'undefined' && __PILOT__) ? 'PILOT — kısıtlı (takma ad, sunucusuz)' : (typeof __TAM__ !== 'undefined' && __TAM__) ? 'TAM — MEB dersleri aktif' : 'DEMO — jüri tanıtım';
  return (
    <Kabuk ekran={ekran} setEkran={setEkran} rol={rolAd}>
      <div data-testid="surum-modu" className="mb-3 rounded-xl border px-3 py-2 text-[11px] font-semibold text-center bg-slate-50 border-slate-200 text-slate-700">v{__SURUM__} · {modEtiket}</div>
      {ekran === 'pano' && <Pano />}
      {ekran === 'dosyalar' && <Dosyalar />}
      {ekran === 'takvim' && <Takvim />}
      {ekran === 'oturum' && <OturumAtolyesi />}
      {ekran === 'katalog' && <EtkinlikKatalogu />}
      {ekran === 'cizelge' && <Cizelge />}
      {ekran === 'rapor' && <RaporAtolyesi />}
      {ekran === 'hizalama' && <Hizalama />}
      {ekran === 'bgm' && <BgmMenu />}
      {ekran === 'rambep' && <RamBep />}
      {ekran === 'evodev' && <EvOdevleri />}
      {ekran === 'aile' && <Aile />}
      {ekran === 'ayarlar' && <Ayarlar />}
    </Kabuk>
  );
}

~~~~

### `components/Ekranlar.tsx`
57416 B ·SHA `bc23f55b5a922127ddacb45082ec12b63f6cb64954f1fd517a92c621d04942b4`

~~~~tsx
/** LEXIVA Supporta™ ekranları — spec §4 · 13 sekme (K-700 ÖÖG uyarlama: BGM okuma menüsü, EQ kodları). */
import { useMemo, useState } from 'react';
import { Brain, CheckCircle2, AlertTriangle, Printer, Plus, Trash2, Database, ChevronLeft, ChevronRight } from 'lucide-react';
import { useKalici } from '../lib/kullan';
import { temizle, kayitSayisi } from '../lib/depo';
import Sherh from './Sherh';
import { SHERHLER, YASA_1, YASA_2, DEP_MODULLER, DEP_TOPLAM_SAAT, KODLAMA, OTURUM_DURUM, MODUL_TERIM_NOTU, DERS_TAVAN, KAPSAM_DISI, RESMI_FORMLAR, KAYIT_HATTI } from '../data/kisitlar';
import { BGM_MODULLER, BGM_FAZ_ETIKET, BGM_KATMAN_NOTU, BGM_SAYI, BGM_TASLAK_NOTU, bgmEtkinlikId, bgmEtkinlikMi, bgmModulden, type BgmFaz } from '../data/bgm';
import { DOSYALAR, PROGRAMLAR, OTURUMLAR, ETKINLIKLER, GIRDILER, RAPORLAR, EV_ODEVLERI, RAM_KAYITLARI } from '../data/mock';
import AileEgitimMerkezi from './aile/AileEgitimMerkezi';
import type { Girdi, Rapor, EvOdevi, Gorusme, IpucuGozlem } from '../data/tipler';
import type { OturumDurum } from '../data/kisitlar';

const Kart = ({ baslik, children, ek }: { baslik: string; children: React.ReactNode; ek?: React.ReactNode }) => (
  <section className="bg-white rounded-2xl border border-slate-200 p-5 space-y-3">
    <div className="flex items-center justify-between gap-3">
      <h2 className="font-bold text-slate-900">{baslik}</h2>{ek}
    </div>
    {children}
  </section>
);

/* ---------- PANO ---------- */
export function Pano() {
  const bugun = OTURUMLAR.filter((o) => o.durum === 'planlandı');
  const bekleyen = RAPORLAR.filter((r) => r.taslak);
  return (
    <div className="space-y-4">
      <div className="bg-teal-50 border border-teal-200 rounded-2xl p-4 flex items-start gap-3">
        <Database className="w-5 h-5 text-teal-600 shrink-0 mt-0.5" />
        <div>
          <h3 className="font-bold text-teal-900 text-sm">Shared Evidence Protocol (Yetkili Kanıt Protokolü) Aktif</h3>
          <p className="text-xs text-teal-700 leading-relaxed mt-1">Eğitmen kürsüsü, T1 (Merkez) ve T2 (Okul) bağlamlarından gelen transfer kanıtlarını anlık derler. Hiçbir modül diğerinin doğrudan veritabanına bağlanmaz; yalnızca pedagojik gelişim kanıtları (Evidence Provenance) okunur.</p>
        </div>
      </div>
      
      <div className="grid sm:grid-cols-2 gap-4">
        <Kart baslik="T1/T2 Transfer Kanıtı İzleme (Günün Oturumları)">
          <ul className="text-sm space-y-2">
            {bugun.map((o) => (
              <li key={o.id} data-testid="pano-oturum" className="flex items-center justify-between p-2 rounded-lg bg-slate-50 border border-slate-100">
                <span>{o.tarih} {o.saat} — {o.dosyaUid} ({o.sureDk} dk)</span>
                <div className="flex gap-1">
                    <span className="text-[10px] font-bold text-slate-500 bg-slate-200 px-1.5 py-0.5 rounded">T1 Merkezi</span>
                    <span className="text-[10px] font-bold text-indigo-500 bg-indigo-50 border border-indigo-200 px-1.5 py-0.5 rounded">T2 Okul Bekleniyor</span>
                </div>
              </li>
            ))}
          </ul>
        </Kart>
        <Kart baslik="Onay Bekleyen Raporlar (Human-Accountable AI)" ek={<span className="text-xs font-bold text-amber-700 bg-amber-50 border border-amber-200 rounded-full px-2 py-0.5">{bekleyen.length}</span>}>
          <ul className="text-sm space-y-1">{bekleyen.map((r) => <li key={r.id}>• {r.baslik}</li>)}</ul>
          <p className="text-[11px] text-slate-500 mt-2 italic">YZ önerileri taslaktır; uzman incelemesi ve onayı olmadan kullanılamaz (K-02).</p>
        </Kart>
      </div>
    </div>
  );
}

/* ---------- DOSYALAR ---------- */
export function Dosyalar() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const d = DOSYALAR.find((x) => x.uid === sec)!;
  const p = PROGRAMLAR.find((x) => x.dosyaUid === sec)!;
  return (
    <>
      <Kart baslik="Dosya listesi">
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((x) => (
            <button key={x.uid} data-testid={`dosya-${x.uid}`} onClick={() => setSec(x.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === x.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {x.uid}
            </button>
          ))}
        </div>
      </Kart>
      <Kart baslik={`Dosya kartı — ${d.uid}`}>
        <dl className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          {[['Ad (maskeli)', d.ad], ['Doğum', d.dogum], ['Okul / Sınıf', d.okulSinif],
            ['Devamsızlık', d.devamsizlikNotu], ['Veli', `${d.veli.ad} · ${d.veli.tel}`],
            ['Rıza kaydı', d.veli.rizaTarihi ?? '—'], ['Geçmiş BEP', d.gecmisBepNotu]].map(([k, v]) => (
            <div key={k as string}><dt className="text-slate-500 text-xs">{k}</dt><dd className="font-medium">{v}</dd></div>
          ))}
        </dl>
      </Kart>
      <Kart baslik="Program kartı">
        <div className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          <div><span className="text-slate-500 text-xs block">Seans sayısı</span>{p.seansSayisi}</div>
          <div><span className="text-slate-500 text-xs block">Sıklık</span>{p.siklik}</div>
          <div><span className="text-slate-500 text-xs block">Aile bileşeni</span>{p.aileBileseni ? 'Var' : 'Yok'}</div>
          <div><span className="text-slate-500 text-xs block">RAM rapor ref.</span>{p.ramRaporRef}</div>
        </div>
        <Sherh metin={SHERHLER.aile} />
      </Kart>
    </>
  );
}

/* ---------- TAKVİM (etkileşimli + kalıcı) ---------- */
export function Takvim() {
  const [oturumlar, setOturumlar] = useKalici('oturumlar', OTURUMLAR);
  const [hafta, setHafta] = useState(0);            // 0 = 03.09 haftası
  const HAFTA_BAS = ['2026-08-27', '2026-09-03', '2026-09-10'];
  const aktifTarih = HAFTA_BAS[hafta + 1] ?? HAFTA_BAS[1];

  const gorunen = useMemo(
    () => oturumlar.filter((o) => Math.abs(new Date(o.tarih).getTime() - new Date(aktifTarih).getTime()) <= 6 * 864e5),
    [oturumlar, aktifTarih]);

  const cakisma = useMemo(() => {
    const m = new Map<string, number>();
    oturumlar.forEach((o) => { const k = `${o.tarih} ${o.saat} ${o.uzmanId}`; m.set(k, (m.get(k) ?? 0) + 1); });
    return [...m.entries()].filter(([, n]) => n > 1).map(([k]) => k);
  }, [oturumlar]);

  const durumDegistir = (id: string, d: OturumDurum) =>
    setOturumlar(oturumlar.map((o) => (o.id === id ? { ...o, durum: d } : o)));

  // K-571/A2: veli görüşme-randevu defteri (hatırlatma GÖNDERİLMEZ — K-334; yalnız yerel — K-05)
  const [gorusmeler, setGorusmeler] = useKalici<Gorusme[]>('gorusmeler', []);
  const [gTarih, setGTarih] = useState('2026-09-17');
  const [gKonu, setGKonu] = useState('');
  const gEkle = () => {
    if (!gKonu.trim()) return;
    setGorusmeler([...gorusmeler, { id: `GR-${gorusmeler.length + 1}`, dosyaUid: 'ÖĞR-4417', tarih: gTarih, konu: gKonu.trim(), durum: 'planlandı', not: '' }]);
    setGKonu('');
  };
  const gDurum = (id: string, d: Gorusme['durum']) => setGorusmeler(gorusmeler.map((g) => (g.id === id ? { ...g, durum: d } : g)));
  const gNot = (id: string, n: string) => setGorusmeler(gorusmeler.map((g) => (g.id === id ? { ...g, not: n } : g)));

  return (
    <>
    <Kart baslik="Oturum takvimi"
      ek={<div className="flex items-center gap-1">
        <button type="button" data-testid="hafta-geri" onClick={() => setHafta((h) => Math.max(-1, h - 1))}
          className="p-1.5 rounded-lg border border-slate-200 hover:bg-slate-50"><ChevronLeft className="w-4 h-4" /></button>
        <span data-testid="hafta-etiket" className="text-xs font-semibold px-2">{aktifTarih} haftası</span>
        <button type="button" data-testid="hafta-ileri" onClick={() => setHafta((h) => Math.min(1, h + 1))}
          className="p-1.5 rounded-lg border border-slate-200 hover:bg-slate-50"><ChevronRight className="w-4 h-4" /></button>
      </div>}>
      {cakisma.length > 0 && (
        <div data-testid="cakisma-uyari" className="flex items-center gap-2 text-xs font-semibold text-rose-700 bg-rose-50 border border-rose-200 rounded-xl px-3 py-2">
          <AlertTriangle className="w-4 h-4" /> Çakışma: {cakisma.join(' · ')} (KC12)
        </div>
      )}
      <table className="w-full text-sm">
        <thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200">
          <th className="py-2">Tarih</th><th>Saat</th><th>Dosya</th><th>Uzman</th><th>Durum</th></tr></thead>
        <tbody>
          {gorunen.map((o) => (
            <tr key={o.id} data-testid="takvim-satir" className="border-b border-slate-100">
              <td className="py-2">{o.tarih}</td><td>{o.saat}</td><td>{o.dosyaUid}</td><td>{o.uzmanId}</td>
              <td>
                <select data-testid={`durum-${o.id}`} value={o.durum}
                  onChange={(e) => durumDegistir(o.id, e.target.value as OturumDurum)}
                  className={`text-[11px] font-bold rounded-full px-2 py-1 border ${
                    o.durum === 'tamamlandı' ? 'bg-emerald-50 text-emerald-700 border-emerald-200' :
                    o.durum === 'planlandı' ? 'bg-sky-50 text-sky-700 border-sky-200' :
                    o.durum === 'gelmedi' ? 'bg-rose-50 text-rose-700 border-rose-200' : 'bg-slate-100 text-slate-600 border-slate-200'}`}>
                  {OTURUM_DURUM.map((d) => <option key={d} value={d}>{d}</option>)}
                </select>
              </td>
            </tr>
          ))}
          {gorunen.length === 0 && <tr><td colSpan={5} className="py-4 text-center text-slate-400 text-sm">Bu haftada oturum yok.</td></tr>}
        </tbody>
      </table>
      <p className="text-[11px] text-slate-500">Durumlar: {OTURUM_DURUM.join(' · ')} · değişiklikler bu cihazda saklanır.</p>
    </Kart>
    <Kart baslik="Veli görüşme-randevu defteri (K-571/A2)" ek={<span className="text-[11px] text-slate-500">hatırlatma gönderilmez — K-334</span>}>
      <div className="rounded-xl bg-amber-50 border border-amber-200 px-3 py-2 text-[11px] font-semibold text-amber-900" data-testid="gorusme-serit">
        Bu ekran bir DEFTERDİR: randevu/görüşme kayıtları yalnız bu cihazda tutulur (K-05) · sistem veliye mesaj/hatırlatma GÖNDERMEZ (K-334) · kimlik bilgisi tutulmaz, yalnız dosya-kodu.
      </div>
      <div className="grid sm:grid-cols-3 gap-3 mt-3" data-testid="gorusme-form">
        <label className="text-sm space-y-1"><span className="text-xs text-slate-500 block">Tarih</span>
          <input data-testid="gorusme-tarih" type="date" value={gTarih} onChange={(e) => setGTarih(e.target.value)} className="w-full rounded-xl border border-slate-300 px-3 py-2" /></label>
        <label className="text-sm space-y-1"><span className="text-xs text-slate-500 block">Konu</span>
          <input data-testid="gorusme-konu" value={gKonu} onChange={(e) => setGKonu(e.target.value)} placeholder="örn. B yarı-dönem değerlendirme paylaşımı" className="w-full rounded-xl border border-slate-300 px-3 py-2" /></label>
        <div className="flex items-end"><button type="button" data-testid="gorusme-ekle" onClick={gEkle}
          className="px-4 py-2 rounded-xl bg-teal-600 text-white text-sm font-semibold">Deftere ekle</button></div>
      </div>
      {gorusmeler.length === 0
        ? <p data-testid="gorusme-bos" className="text-sm text-slate-500 mt-3">Defter boş — ilk görüşme kaydını ekleyin.</p>
        : <table className="w-full text-sm mt-3"><thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200"><th className="py-2">Tarih</th><th>Konu</th><th>Durum</th><th>Not</th></tr></thead>
          <tbody>{gorusmeler.map((g) => (
            <tr key={g.id} data-testid="gorusme-satir" className="border-b border-slate-100">
              <td className="py-2">{g.tarih}</td><td>{g.konu}</td>
              <td><select data-testid="gorusme-durum" value={g.durum} onChange={(e) => gDurum(g.id, e.target.value as Gorusme['durum'])} className="rounded-lg border border-slate-300 px-2 py-1 text-xs">
                {['planlandı', 'gerçekleşti', 'ertelendi', 'iptal'].map((d) => <option key={d} value={d}>{d}</option>)}</select></td>
              <td><input data-testid="gorusme-not" value={g.not} onChange={(e) => gNot(g.id, e.target.value)} placeholder="kısa not (yapılandırılmamış)" className="w-full rounded-lg border border-slate-200 px-2 py-1 text-xs" /></td>
            </tr>))}</tbody></table>}
      <p className="text-[11px] text-slate-400 mt-2">Durum-döngüsü: planlandı → gerçekleşti / ertelendi / iptal · görüşme-notu uzmanın serbest kaydıdır (K-02).</p>
    </Kart>
    </>
  );
}

/* ---------- OTURUM ATÖLYESİ (YASA-1 burada zorlanır) ---------- */
export function OturumAtolyesi() {
  const [etkinlik, setEtkinlik] = useState<string>('');
  const [tip, setTip] = useState<Girdi['kodlamaTipi']>('xArti');
  const [deger, setDeger] = useState('');
  const [ipucu, setIpucu] = useState<IpucuGozlem | ''>(''); // K-571/A4: gözlenen-ipucu-kademesi
  const [kayitlar, setKayitlar] = useKalici<Girdi[]>('girdiler', GIRDILER);
  // K-400: bu dosya için uzmanın seçtiği BGM modülleri (bgm-secim) oturumda ETKİNLİK olarak listelenir (YASA-1 işler).
  const [bgmSecim] = useKalici<Record<string, string[]>>('bgm-secim', { 'ÖĞR-4417': ['EQ-01', 'EQ-02', 'EQ-05'], 'ÖĞR-2903': [] });
  const dosyaUid = OTURUMLAR[0].dosyaUid; // OT-101
  const bgmSecili = BGM_MODULLER.filter((m) => (bgmSecim[dosyaUid] ?? []).includes(m.id));
  const secBgm = (id: string) => { setEtkinlik(id); const m = bgmModulden(id); if (m) setTip(m.girdiTipi); };
  const girilebilir = etkinlik !== '' && deger !== '';   // YASA-1
  const aktifBgm = bgmModulden(etkinlik);
  return (
    <>
      <Kart baslik="Oturum kartı — OT-101">
        <p className="text-sm text-slate-600">Amaç: hece farkındalığı · Süre: 40 dk · Malzeme: hece kartları, çalışma yaprağı</p>
        <p className="text-xs text-slate-500" data-testid="oturum-akis">
          Akış: açılış (ödev izleme) → ana etkinlik (DEP 0…n + BGM 0…n, uzman seçer) → girdi → kapanış (ödev + güçlü yön)
        </p>
        <Sherh metin={SHERHLER.oturum} />
        <div className="rounded-xl border border-slate-300 bg-slate-50 px-3 py-2 text-[11px] font-semibold text-slate-700 flex items-start gap-2">
          <span className="shrink-0">ⓘ</span>
          <span>Seçim uzmandadır; sistem otomatik zorluk değiştirmez — kanıtı gösterir, kararı uzman verir. (K2 hizalaması · MVP’de adaptasyon yok, P2 kalemidir)</span>
        </div>
      </Kart>
      <Kart baslik="Bu oturumda seçili BGM modülleri" ek={<span className="text-[11px] text-slate-500">{dosyaUid} · sıra uzmanın</span>}>
        {bgmSecili.length === 0
          ? <p className="text-sm text-slate-500" data-testid="oturum-bgm-bos">Bu dosya için BGM seçilmedi (Bilişsel Geliştirme ekranından alınır). DEP etkinlikleri yine kullanılabilir.</p>
          : <div className="flex flex-wrap gap-2">
              {bgmSecili.map((m) => (
                <button key={m.id} type="button" data-testid={`oturum-bgm-${m.id}`} onClick={() => secBgm(bgmEtkinlikId(m.id))}
                  className={`text-left rounded-xl border px-3 py-2 text-xs ${etkinlik === bgmEtkinlikId(m.id) ? 'border-sky-500 bg-sky-50' : 'border-slate-200 bg-white'}`}>
                  <div className="font-semibold">{m.id} · {m.ad} <span className="text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5 ml-1">BGM</span></div>
                  <div className="text-slate-500">{m.sureDk} · girdi: {KODLAMA[m.girdiTipi].ad}{m.depKoprusu ? ` · DEP köprüsü ${m.depKoprusu}` : ''}</div>
                </button>
              ))}
            </div>}
        {aktifBgm && (
          <div data-testid="oturum-bgm-detay" className="rounded-xl bg-slate-50 border border-slate-200 px-3 py-2 text-[11px] text-slate-700 space-y-0.5">
            <div><b>Etkinlik:</b> {aktifBgm.etkinlik}</div>
            <div><b>Malzeme:</b> {aktifBgm.malzeme.join(' · ')} · <b>İpucu:</b> {aktifBgm.ipucu}</div>
            <div><b>Ölçüm:</b> {aktifBgm.olcum}</div>
          </div>
        )}
        <p className="text-[11px] text-slate-400">{BGM_TASLAK_NOTU}</p>
      </Kart>
      <Kart baslik="Hızlı girdi paneli" ek={<span className="text-[11px] text-slate-500">YASA-1 etkin</span>}>
        <div className="grid sm:grid-cols-3 gap-3">
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Etkinlik <b className="text-rose-600">*zorunlu</b></span>
            <select data-testid="girdi-etkinlik" value={etkinlik} onChange={(e) => setEtkinlik(e.target.value)}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              <option value="">— etkinlik seçin —</option>
              <optgroup label="DEP-2026 etkinlikleri">
                {ETKINLIKLER.map((e) => <option key={e.id} value={e.id}>{e.ad} ({e.hedefKod})</option>)}
              </optgroup>
              {bgmSecili.length > 0 && (
                <optgroup label="BGM-12 (bu dosya için seçili)">
                  {bgmSecili.map((m) => <option key={m.id} value={bgmEtkinlikId(m.id)}>[BGM] {m.id} · {m.ad}</option>)}
                </optgroup>
              )}
            </select>
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Kodlama</span>
            <select data-testid="girdi-tip" value={tip} onChange={(e) => setTip(e.target.value as Girdi['kodlamaTipi'])}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              {Object.entries(KODLAMA).map(([k, v]) => <option key={k} value={k}>{v.ad}</option>)}
            </select>
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Değer</span>
            <input data-testid="girdi-deger" value={deger} onChange={(e) => setDeger(e.target.value)}
              placeholder={KODLAMA[tip].aciklama} className="w-full rounded-xl border border-slate-300 px-3 py-2" />
          </label>
          <label className="text-sm space-y-1">
            <span className="text-xs text-slate-500 block">Gözlenen ipucu-kademesi (K-571/A4)</span>
            <select data-testid="girdi-ipucu" value={ipucu} onChange={(e) => setIpucu(e.target.value as IpucuGozlem | '')}
              className="w-full rounded-xl border border-slate-300 px-3 py-2">
              <option value="">— seçilmeyebilir —</option>
              <option value="model">Model</option>
              <option value="sozel">Sözel</option>
              <option value="bagimsiz">Bağımsız</option>
            </select>
          </label>
        </div>
        {(() => { const e = ETKINLIKLER.find((x) => x.id === etkinlik); return e
          ? <p data-testid="girdi-kademe-plan" className="text-[11px] text-slate-500">Planlı ipucu-kademesi: {e.ipucuKademesi} · gözlem kaydı uzmanın teyididir (K-02: ölçüm-değil-gözlem).</p>
          : null; })()}
        <button type="button" data-testid="girdi-kaydet" disabled={!girilebilir}
          onClick={() => { setKayitlar([...kayitlar, { id: `G-${kayitlar.length + 1}`, oturumId: 'OT-101',
            etkinlikId: etkinlik, kodlamaTipi: tip, deger, tarih: '2026-09-03', girenRol: 'uzman', ipucuGozlem: ipucu || undefined }]); setDeger(''); }}
          className={`inline-flex items-center gap-1.5 px-4 py-2 rounded-xl text-sm font-semibold ${
            girilebilir ? 'bg-teal-600 text-white hover:bg-teal-700' : 'bg-slate-200 text-slate-400 cursor-not-allowed'}`}>
          <Plus className="w-4 h-4" /> Girdi kaydet
        </button>
        {!girilebilir && <p data-testid="yasa1-uyari" className="text-[11px] text-rose-600">{YASA_1}</p>}
        <ul className="text-sm space-y-1 pt-2 border-t border-slate-100">
          {kayitlar.map((g) => {
            const bgm = bgmModulden(g.etkinlikId);
            const e = ETKINLIKLER.find((x) => x.id === g.etkinlikId);
            const ad = bgm ? `${bgm.id} · ${bgm.ad}` : (e?.ad ?? g.etkinlikId);
            return (
              <li key={g.id} data-testid="girdi-satir" data-katman={bgm ? 'bgm' : 'dep'}>
                • {ad} {bgm && <span className="text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5">BGM</span>} → <b>{g.deger}</b>{' '}
                <span className="text-slate-400 text-xs">({KODLAMA[g.kodlamaTipi].ad})</span>
                {g.ipucuGozlem && <span className="text-slate-400 text-xs"> · ipucu(gözlenen): {{ model: 'Model', sozel: 'Sözel', bagimsiz: 'Bağımsız' }[g.ipucuGozlem]}</span>}
              </li>
            );
          })}
        </ul>
      </Kart>
    </>
  );
}

/* ---------- ÇİZELGE (YASA-2) ---------- */
export function Cizelge() {
  const [tum] = useKalici<Girdi[]>('girdiler', GIRDILER);
  // K-400: DEP ve BGM girdileri AYRI filtrelenir — iki katman karıştırılmaz (K-398 kuyruğu).
  const [katman, setKatman] = useState<'hepsi' | 'dep' | 'bgm'>('hepsi');
  const girdiler = tum.filter((g) => katman === 'hepsi' ? true : katman === 'bgm' ? bgmEtkinlikMi(g.etkinlikId) : !bgmEtkinlikMi(g.etkinlikId));
  const sayim = girdiler.length;
  const basari = girdiler.filter((g) => g.deger === '+' || g.deger === 'Evet' || g.deger === '3').length;
  const bgmSayi = tum.filter((g) => bgmEtkinlikMi(g.etkinlikId)).length;
  return (
    <>
      <div className="rounded-xl border border-amber-300 bg-amber-50 px-3 py-2 text-[11px] font-semibold text-amber-900 flex flex-col gap-1" data-testid="k4-serit">
        <span>Tek seansla genelleme yok · İzlem süresi: __ hafta · Uyum dönemi (ilk 2 hafta) tek başına yorumlanmaz</span>
        <span>Kaynak: etkinlik girdileri (YASA-1) · Akran karşılaştırması yok · Z-9: kesintisiz odak süresi 12→18 dk — ilerleme dili, eşik değil</span>
      </div>
    <Kart baslik="DEP saat-izleri — girdilerden türetilmiş (K-571/A1)" ek={<span className="text-[11px] text-slate-500">YASA-2 deseni: elle çizilmez</span>}>
      <div data-testid="dep-saat-izleri">
        <table className="w-full text-sm"><thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200"><th className="py-2">Dosya</th><th>Tamamlanan oturum</th><th>Toplam süre</th><th>DEP girdisi</th></tr></thead>
        <tbody>{DOSYALAR.map((d) => {
          const ot = OTURUMLAR.filter((o) => o.dosyaUid === d.uid && o.durum === 'tamamlandı');
          const dk = ot.reduce((t, o) => t + o.sureDk, 0);
          const gdSayi = GIRDILER.filter((g) => { const o = OTURUMLAR.find((x) => x.id === g.oturumId); return o?.dosyaUid === d.uid && !bgmEtkinlikMi(g.etkinlikId); }).length;
          return <tr key={d.uid} data-testid="dep-saat-satir" className="border-b border-slate-100">
            <td className="py-2">{d.uid}</td><td>{ot.length}</td><td><b>{dk} dk</b></td><td>{gdSayi}</td></tr>;
        })}</tbody></table>
        <p className="text-[11px] text-slate-400 mt-2">Ders-saati dönüşümü uzmanın işidir (dk-olarak izlenir) · hedef değil iz-süresidir · modül-dökümü, girdi-oturum eşlemesi genişlediğinde (P2) · yalnız yerel, kimliksiz (K-05).</p>
      </div>
    </Kart>
    <Kart baslik="İzleme çizelgesi" ek={<span className="text-[11px] text-slate-500">girdilerden türetildi</span>}>
      <div className="flex gap-1.5">
        {(['hepsi', 'dep', 'bgm'] as const).map((k) => (
          <button key={k} type="button" data-testid={`cizelge-filtre-${k}`} onClick={() => setKatman(k)}
            className={`px-2.5 py-1 rounded-lg text-[11px] border ${katman === k ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
            {k === 'hepsi' ? 'Tümü' : k === 'dep' ? 'DEP-2026' : `BGM-12 (${bgmSayi})`}
          </button>
        ))}
      </div>
      <div className="flex items-end gap-2 h-28" data-testid="cizelge-grafik">
        {girdiler.map((g, i) => (
          <div key={g.id} className="flex-1 flex flex-col items-center justify-end gap-1 h-full" data-katman={bgmEtkinlikMi(g.etkinlikId) ? 'bgm' : 'dep'}>
            {/* v0.8.0: yükseklik px — yüzde yükseklik esnek satırda 0'a çöküyordu (v0.7.0 görsel hatası) */}
            <div data-testid="cizelge-cubuk" className={`w-full rounded-t-lg ${bgmEtkinlikMi(g.etkinlikId) ? 'bg-sky-500' : 'bg-teal-500'}`}
              style={{ height: `${Math.min(96, 28 + i * 16)}px` }} />
            <span className="text-[10px] text-slate-500">{g.deger}</span>
          </div>
        ))}
      </div>
      <p className="text-sm">Toplam girdi: <b data-testid="cizelge-toplam">{sayim}</b> · Hedefe ulaşılan: <b>{basari}</b></p>
      <p className="text-[11px] text-slate-500" data-testid="cizelge-katman-notu">Yeşil: DEP-2026 · Mavi: BGM-12. İki katman ayrı izlenir; birbirinin yerine sayılmaz.</p>
      <Sherh metin={SHERHLER.cizelge} />
      <p className="text-[11px] text-slate-400">{YASA_2}</p>
    </Kart>
    </>
  );
}

/* ---------- RAPOR ATÖLYESİ (YASA-3) ---------- */
const TUR_ETIKET: Record<string, string> = {
  seans: 'Seans özeti', aylik: 'Aylık özet', donem: 'Dönem sonu',
  'bep-ilerleme': 'BEP ilerleme taslağı', 'ram-paketi': 'RAM izleme paketi',
  'aile-bilgilendirme': 'Aile bilgilendirme',
};

export function RaporAtolyesi() {
  const [liste, setListe] = useKalici<Rapor[]>('raporlar', RAPORLAR);
  const onayla = (id: string) => setListe(liste.map((r) => r.id === id ? { ...r, taslak: false, onayKim: 'Yönetici', onayTarih: '2026-09-03' } : r));

  const sistemOnerisi = (r: Rapor) => {
    const ot = OTURUMLAR.filter((o) => o.dosyaUid === r.dosyaUid && o.durum === 'tamamlandı');
    const dk = ot.reduce((t, o) => t + o.sureDk, 0);
    const gd = GIRDILER.filter((g) => OTURUMLAR.find((o) => o.id === g.oturumId)?.dosyaUid === r.dosyaUid).length;
    const ozet = `

— YZ EĞİTİMSEL DESTEK ÖNERİSİ —
(Kanıt Kaynağı: ${ot.length} T1 seansı, ${dk} dk aktif izlem, ${gd} girdi kaydı)
Çocuğun okuma görevi sürekliliğinde %20'lik varyans gözlemlendi. Scaffold Fading (Destek Çekme) seviyesinin Sembolik'ten Fiziksel'e esnetilmesi önerilir.

⚠️ BELİRSİZLİK BİLDİRİMİ: Bu %82 güven aralığına sahip istatistiksel bir öneridir. Hiçbir koşulda klinik bir yönlendirme veya teşhis değildir (K-02). Uzmanın pedagojik onayı ve gerekçelendirmesi esastır.`;
    setListe(liste.map((x) => (x.id === r.id ? { ...x, icerik: x.icerik + ozet } : x)));
  };

  const reddetVeGerekcelendir = (r: Rapor) => {
    const ozet = `

— YZ ÖNERİSİ UZMAN TARAFINDAN REDDEDİLDİ —
Gerekçe: Çocuğun ev (T2) bağlamından gelen yorgunluk verisi sistemde eksiktir. Destek seviyesi korunacaktır.`;
    setListe(liste.map((x) => (x.id === r.id ? { ...x, icerik: x.icerik + ozet } : x)));
  };

  const disaAktar = (r: Rapor) => {
    if (r.taslak) return;
    const html = `<!doctype html><title>${r.baslik}</title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:16px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1>${TUR_ETIKET[r.tur] ?? r.tur} — ${r.baslik}</h1><div class=muhur>ONAYLI — ${r.onayKim ?? ''} ${r.onayTarih ?? ''}</div><pre>${r.icerik}</pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;|&nbsp; Kopya 2/2 — Kurum arşivi · ${new Date().toISOString().slice(0,10)} · Supporta v${typeof __SURUM__!=='undefined'?__SURUM__:'0.8.1'}</div><script>window.print()<\/script>`;
    const w = window.open('', '_blank'); if (w) { w.document.write(html); w.document.close(); }
    const csv = `tur,baslik,durum,icerik
${r.tur},"${r.baslik.replace(/"/g,'""')}",ONAYLI,"${r.icerik.replace(/"/g,'""')}"`;
    const blob = new Blob([csv], { type: 'text/csv;charset=utf-8;' });
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a'); a.href = url; a.download = `${r.id}-${r.tur}.csv`; a.click(); URL.revokeObjectURL(url);
  };
  
  return (
    <div className="space-y-4">
      {liste.map((r) => (
        <Kart key={r.id} baslik={`${TUR_ETIKET[r.tur] ?? r.tur} — ${r.baslik}`} ek={r.taslak ? <span data-testid="muhur-taslak" className="text-[11px] font-black tracking-wider text-amber-700 bg-amber-50 border border-amber-300 rounded-lg px-2 py-1">UZMAN ONAYI BEKLİYOR</span> : <span data-testid="muhur-onayli" className="inline-flex items-center gap-1 text-[11px] font-bold text-emerald-700 bg-emerald-50 border border-emerald-200 rounded-lg px-2 py-1"><CheckCircle2 className="w-3.5 h-3.5" /> UZMAN ONAYLI</span>}>
          <textarea 
            value={r.icerik} 
            onChange={(e) => setListe(liste.map(x => x.id === r.id ? {...x, icerik: e.target.value} : x))}
            disabled={!r.taslak}
            className="w-full h-40 p-3 text-sm text-slate-700 bg-slate-50 border border-slate-200 rounded-xl font-mono focus:ring-2 focus:ring-teal-500 outline-none"
          />
          <span data-testid="rapor-icerik" className="sr-only">{r.icerik}</span>
          
          <div className="flex flex-col gap-3 mt-3">
            {r.taslak && (
              <div className="bg-indigo-50 border border-indigo-100 p-3 rounded-xl space-y-3">
                <div className="flex items-center gap-2">
                  <Brain className="w-4 h-4 text-indigo-600" />
                  <span className="text-xs font-bold text-indigo-900">Human-Accountable AI (YZ Destek Asistanı)</span>
                </div>
                <div className="flex flex-wrap gap-2">
                  <button type="button" data-testid={`oneri-al-${r.id}`} onClick={() => sistemOnerisi(r)} className="px-3 py-1.5 rounded-lg bg-white border border-indigo-200 text-indigo-700 hover:bg-indigo-100 text-xs font-semibold shadow-sm transition-colors">
                    Kanıtı İncele ve YZ Önerisi Al
                  </button>
                  <button type="button" data-testid={`oneri-red-${r.id}`} onClick={() => reddetVeGerekcelendir(r)} className="px-3 py-1.5 rounded-lg bg-white border border-rose-200 text-rose-700 hover:bg-rose-50 text-xs font-semibold shadow-sm transition-colors">
                    Öneriyi Reddet ve Gerekçelendir
                  </button>
                </div>
                <p className="text-[10px] text-indigo-600 italic">YZ yalnızca pedagojik verileri derler; hiçbir zaman tek başına karar almaz.</p>
                {r.icerik.includes('YZ EĞİTİMSEL DESTEK ÖNERİSİ') && (
                  <div data-testid="oneri-etiket" className="text-[10px] font-bold text-indigo-800 bg-indigo-100 border border-indigo-300 rounded-lg px-2 py-1 inline-block">YZ ÖNERİSİ KATMANI — uzman onayı gerektirir</div>
                )}
              </div>
            )}
            
            <div className="flex items-center gap-2 flex-wrap pt-2 border-t border-slate-100">
              {r.taslak && <button type="button" data-testid={`onayla-${r.id}`} onClick={() => onayla(r.id)} className="px-4 py-2 rounded-xl bg-teal-600 hover:bg-teal-700 text-white text-xs font-bold shadow-sm transition-colors">✓ Değişiklikleri Onayla ve İmzala</button>}
              <button type="button" data-testid={`disa-${r.id}`} disabled={r.taslak} onClick={()=>disaAktar(r)} className={`inline-flex items-center gap-1 px-4 py-2 rounded-xl text-xs font-bold shadow-sm transition-colors ${r.taslak ? 'bg-slate-100 text-slate-400 cursor-not-allowed border border-slate-200' : 'bg-slate-900 text-white hover:bg-black'}`}><Printer className="w-4 h-4" /> Dışa aktar (2 kopya)</button>
              {r.taslak && <span className="text-[11px] text-rose-600 font-semibold" data-testid="kc10">Onaysız rapor dışa aktarılamaz.</span>}
            </div>
          </div>
        </Kart>
      ))}
    </div>
  );
}

/* ---------- PROGRAM HİZALAMA (Y2-A / KC13) ---------- */
export function Hizalama() {
  const [modul, setModul] = useState<string>('M3');
  const m = DEP_MODULLER.find((x) => x.id === modul)!;
  const toplam = DEP_TOPLAM_SAAT;
  return (
    <Kart baslik="MEB destek eğitim programı modülleriyle hizalı çıktı">
      <div className="flex gap-2 flex-wrap">
        {DEP_MODULLER.map((x) => (
          <button key={x.id} data-testid={`dep-${x.id}`} onClick={() => setModul(x.id)}
            className={`px-3 py-1.5 rounded-xl text-xs border ${modul === x.id ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
            {x.id} · {x.ad} <b>({x.saat} sa)</b>
          </button>
        ))}
      </div>
      <p className="text-sm">Seçili: <b>{m.ad}</b> — {m.bolum} bölüm · önerilen <b>{m.saat} ders saati</b></p>
      <p data-testid="dep-toplam" className="text-[11px] text-slate-500">Toplam program: <b>{toplam} ders saati</b> · 6 modül · giriş yalnız ELLE yapılır.</p>
      <div data-testid="modul-serbest" className="rounded-xl bg-teal-50 border border-teal-200 px-3 py-2 text-[11px] text-teal-900">
        <b>Modül seçimi serbesttir.</b> {MODUL_TERIM_NOTU}
      </div>
      <p data-testid="ders-tavan" className="text-[11px] text-slate-500">
        Resmî tavan (ÖEK Yön. md.24/4): aylık <b>{DERS_TAVAN.aylikBireysel}</b> bireysel · <b>{DERS_TAVAN.aylikGrup}</b> grup ·
        haftalık <b>{DERS_TAVAN.haftalikBireysel}</b>/<b>{DERS_TAVAN.haftalikGrup}</b> · günlük toplam <b>{DERS_TAVAN.gunlukToplam}</b> saat.
      </p>
      <Sherh metin={SHERHLER.hizali} ton="uyari" />
    </Kart>
  );
}

/* ---------- AİLE & ÖĞRETMEN + AİLE EĞİTİM MERKEZİ (v0.8.4 A/B) ---------- */
export function Aile() {
  const [secAile, setSecAile] = useState(DOSYALAR[0].uid);
  return (
    <>
      <Kart baslik="Aile & Öğretmen İşbirliği">
        <p className="text-sm text-slate-700">Görüşme notu · öneri bloğu (kim · ne · ne zaman) · ev görevi · okul-ev not hattı.</p>
        <Sherh metin={SHERHLER.aile} ton="uyari" />
      </Kart>
      <Kart baslik="Aile Eğitim Merkezi — A Genel + B Analize Göre (v0.8.4)" ek={<span className="text-[11px] text-slate-500">K-407 · 5+1 · TASLAK</span>}>
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} type="button" data-testid={`aile-dosya-${d.uid}`} onClick={() => setSecAile(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${secAile === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>{d.uid}</button>
          ))}
        </div>
        <AileEgitimMerkezi dosyaUid={secAile} />
      </Kart>
      <Kart baslik="Bilgilendirme çıktısı">
        <p className="text-sm text-slate-600">Yalnız <b>onaylı</b> raporlardan üretilir; hatırlatma metninde çocuk adı ve tanı bilgisi yer almaz (KC9).</p>
        <div className="rounded-xl bg-slate-50 border border-slate-200 p-3 text-xs font-mono" data-testid="sms-taslak">
          Sayın veli, 10.09.2026 10:00 randevunuzu hatırlatırız. — Merkez
        </div>
      </Kart>
    </>
  );
}

/* ---------- AYARLAR ---------- */
export function Ayarlar() {
  return (
    <Kart baslik="Şerh kütüphanesi ve roller">
      <ul className="text-sm space-y-2">
        {Object.entries(SHERHLER).map(([k, v]) => (
          <li key={k}><span className="text-xs font-bold text-slate-500 uppercase">{k}</span><Sherh metin={v} /></li>
        ))}
      </ul>
      <p className="text-[11px] text-slate-500">Şerhler sabittir; kullanıcı tarafından kaldırılamaz (KC3).</p>
      <div className="pt-3 border-t border-slate-100 space-y-2">
        <h3 className="font-bold text-sm">Kapsam dışı (bilinçli sınırlar)</h3>
        <ul data-testid="kapsam-disi" className="text-xs space-y-1.5">
          {KAPSAM_DISI.map((k) => (
            <li key={k.ad} className="rounded-xl bg-slate-50 border border-slate-200 px-3 py-2">
              <b>{k.ad}</b> — <span className="text-slate-600">{k.gerekce}</span>
            </li>
          ))}
        </ul>
      </div>
      <div className="pt-3 border-t border-slate-100 space-y-2">
        <h3 className="font-bold text-sm flex items-center gap-1.5"><Database className="w-4 h-4 text-slate-500" /> Yerel veri</h3>
        <p className="text-xs text-slate-600">
          Girdiler, oturum durumları ve rapor onayları <b>yalnız bu cihazda</b> saklanır (KVKK yerel-önce).
          Buluta hiçbir veri gönderilmez. Kayıtlı anahtar: <b data-testid="kayit-sayisi">{kayitSayisi()}</b>
        </p>
        <button type="button" data-testid="veri-sil"
          onClick={() => { temizle(); location.reload(); }}
          className="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-xl bg-rose-50 text-rose-700 border border-rose-200 text-xs font-semibold hover:bg-rose-100">
          <Trash2 className="w-3.5 h-3.5" /> Yerel veriyi sil (K-79 çocuk katılımı kuralı — çocuk katılımı içeren herhangi bir kullanım, PCV'nin uzman/paydaş doğrulama kapsamından ayrı bir insan katılımlı saha kullanım senaryosudur ve ilgili etik, hukuki, kurumsal ve veri yönetişimi gereklilikleri ayrıca doğrulanmadan etkinleştirilemez)
        </button>
      </div>
    </Kart>
  );
}


/* ---------- RAM & BEP TAKİBİ (K-395) ---------- */
export function RamBep() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const r = RAM_KAYITLARI.find((x) => x.dosyaUid === sec)!;
  const pr = PROGRAMLAR.find((x) => x.dosyaUid === sec)!;
  const hat = KAYIT_HATTI.find((h) => h.id === pr.kayitHatti)!;
  return (
    <>
      <Kart baslik="RAM raporu ve kayıt hattı">
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} data-testid={`ram-dosya-${d.uid}`} onClick={() => setSec(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>{d.uid}</button>
          ))}
        </div>
        <div data-testid="kayit-hatti" className="rounded-xl bg-sky-50 border border-sky-200 px-3 py-2 text-xs text-sky-900">
          <b>Kayıt hattı: {hat.ad}</b><br />RAM raporu: <b>{hat.ram}</b> · Planlama: {hat.planlama}
        </div>
        <dl className="grid grid-cols-2 gap-x-6 gap-y-1.5 text-sm">
          {[['Rapor no', r.raporNo], ['Rapor tarihi', r.tarih], ['Geçerlilik', r.gecerlilik],
            ['EDİF durumu', r.edifDurumu], ['Sonraki izleme', r.sonrakiIzleme],
            ['Portfolyo', r.portfolyoHazir ? 'Hazır' : 'Hazır değil']].map(([k, v]) => (
            <div key={k as string}><dt className="text-slate-500 text-xs">{k}</dt><dd className="font-medium">{v}</dd></div>
          ))}
        </dl>
        <Sherh metin={SHERHLER.hizali} ton="uyari" />
      </Kart>
      <Kart baslik="Resmî form ailesi — hangi girdi neyi besler"
        ek={<span className="text-[11px] text-slate-500">DEP-2026 EK-1…EK-7</span>}>
        <table className="w-full text-sm" data-testid="resmi-formlar">
          <thead><tr className="text-left text-xs text-slate-500 border-b border-slate-200">
            <th className="py-2 w-16">Ek</th><th>Form</th><th className="hidden sm:table-cell">Doldurma anı</th><th>Supporta katkısı</th></tr></thead>
          <tbody>
            {RESMI_FORMLAR.map((f) => (
              <tr key={f.ek} className="border-b border-slate-100 align-top">
                <td className="py-2 font-bold">{f.ek}</td>
                <td className="pr-2">{f.ad}</td>
                <td className="pr-2 text-slate-500 text-xs hidden sm:table-cell">{f.an}</td>
                <td className="text-xs text-slate-600">{f.besleyen}</td>
              </tr>
            ))}
          </tbody>
        </table>
        <div data-testid="form-sinir" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900">
          <b>Sınır:</b> Supporta bu formları <b>DOLDURMAZ</b>. x/+ işaretini, performans düzeyini ve
          “ulaşılamama nedenini” <b>uzman</b> belirler; portfolyo <b>RAM onayına</b> gider.
          Model: <b>Supporta kanıt üretir · uzman karar verir · RAM onaylar.</b>
        </div>
        <div className="rounded-xl border border-slate-300 bg-slate-50 px-3 py-2 text-[11px] font-semibold text-slate-700" data-testid="k1-serit">
          Bu alan kanıtı yapılandırır; pedagojik kararı üretmez — “ulaşılamama nedeni / öneri / analize göre aile görevi”ni uzman yazar, sistem önermez.
        </div>
      </Kart>
    </>
  );
}

/* ---------- EV ÖDEVLERİ / SEANS DIŞI (K-395) ---------- */
export function EvOdevleri() {
  const [liste, setListe] = useKalici<EvOdevi[]>('evodev', EV_ODEVLERI);
  const durumDegis = (id: string, d: EvOdevi['durum']) =>
    setListe(liste.map((o) => (o.id === id ? { ...o, durum: d } : o)));
  return (
    <>
      <Kart baslik="Ev çalışmaları ve seans dışı görevler"
        ek={<span className="text-[11px] text-slate-500">kim · ne · ne zaman</span>}>
        <ul className="space-y-2">
          {liste.map((o) => (
            <li key={o.id} data-testid="evodev-satir" className="rounded-xl border border-slate-200 px-3 py-2">
              <div className="flex items-start justify-between gap-3">
                <div>
                  <div className="font-semibold text-sm">{o.baslik}</div>
                  <div className="text-xs text-slate-500">{o.dosyaUid} · {o.kim} · {o.neZaman}</div>
                  {o.not && <div className="text-xs text-slate-600 mt-1">Not: {o.not}</div>}
                </div>
                <select data-testid={`evodev-durum-${o.id}`} value={o.durum}
                  onChange={(e) => durumDegis(o.id, e.target.value as EvOdevi['durum'])}
                  className={`text-[11px] font-bold rounded-full px-2 py-1 border shrink-0 ${
                    o.durum === 'yapıldı' ? 'bg-emerald-50 text-emerald-700 border-emerald-200' :
                    o.durum === 'yapılmadı' ? 'bg-rose-50 text-rose-700 border-rose-200' :
                    'bg-sky-50 text-sky-700 border-sky-200'}`}>
                  <option value="verildi">verildi</option><option value="yapıldı">yapıldı</option><option value="yapılmadı">yapılmadı</option>
                </select>
              </div>
            </li>
          ))}
        </ul>
        <Sherh metin="Ev çalışması süreci destekler; ödev performansı puanlanmaz, akran karşılaştırması yapılmaz." />
      </Kart>
      <Kart baslik="Seans başı izleme ritüeli">
        <ol className="text-sm space-y-1 list-decimal list-inside text-slate-700">
          <li>Ev çalışması gözden geçirilir (yapıldı/yapılmadı — <b>yargı değil gözlem</b>).</li>
          <li>Bir önceki oturumun hedef davranışı hatırlatılır.</li>
          <li>Bugünün etkinliği ve ipucu kademesi belirlenir.</li>
          <li>Oturum sonunda veli için tek satırlık jargonsuz not yazılır.</li>
        </ol>
        <Sherh metin={SHERHLER.aile} />
      </Kart>
    </>
  );
}


/* ---------- M4: ETKİNLİK & HEDEF KATALOĞU (K-396) — düzenlenebilir (v0.8.1) + BGM ayrı filtre (v0.8.3 K-403 kuyruğu E2) ---------- */
export function EtkinlikKatalogu() {
  const [katman, setKatman] = useState<'hepsi' | 'DEP' | 'BGM'>('hepsi');
  const [modul, setModul] = useState<string>('hepsi');
  const [katalog, setKatalog] = useKalici<import('../data/tipler').Etkinlik[]>('etkinlikler', ETKINLIKLER);
  const [duzenId, setDuzenId] = useState<string | null>(null);
  const [form, setForm] = useState<{ ad: string; hedefKod: string; modulAdi: string; ipucuKademesi: string; malzeme: string; katman: 'DEP' | 'BGM' }>({ ad: '', hedefKod: '', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi: '', malzeme: '', katman: 'DEP' });
  const katmanFiltreli = katman === 'hepsi' ? katalog : katalog.filter((e) => (e.katman ?? 'DEP') === katman);
  const liste = modul === 'hepsi' ? katmanFiltreli : katmanFiltreli.filter((e) => e.modulAdi === modul);
  const moduller = katman === 'BGM' ? ['hepsi', 'BGM-12'] : ['hepsi', ...DEP_MODULLER.map((m) => m.ad)];
  const kaydet = () => {
    if (!form.ad.trim() || !form.hedefKod.trim()) return;
    const yeni: import('../data/tipler').Etkinlik = { id: duzenId ?? `ET-${Date.now()}`, ad: form.ad.trim(), hedefKod: form.hedefKod.trim(), modulAdi: form.katman==='BGM' ? 'BGM-12' : form.modulAdi, ipucuKademesi: form.ipucuKademesi.trim() || 'Model → bağımsız', malzeme: form.malzeme.split(',').map((s)=>s.trim()).filter(Boolean), katman: form.katman };
    if (duzenId) setKatalog(katalog.map((e)=> e.id===duzenId ? yeni : e));
    else setKatalog([...katalog, yeni]);
    setDuzenId(null); setForm({ ad: '', hedefKod: '', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi: '', malzeme: '', katman: 'DEP' });
  };
  const duzenle = (id: string) => { const e = katalog.find((x)=>x.id===id)!; setDuzenId(id); setForm({ ad: e.ad, hedefKod: e.hedefKod, modulAdi: e.modulAdi, ipucuKademesi: e.ipucuKademesi, malzeme: e.malzeme.join(', '), katman: (e.katman ?? 'DEP') as 'DEP'|'BGM' }); };
  const sil = (id: string) => setKatalog(katalog.filter((e)=>e.id!==id));
  return (
    <>
      <Kart baslik="Etkinlik ve hedef davranış kataloğu" ek={<span className="text-[11px] text-slate-500">{liste.length} / {katalog.length} etkinlik · DEP {katalog.filter(e=>(e.katman??'DEP')==='DEP').length} · BGM {katalog.filter(e=>e.katman==='BGM').length}</span>}>
        <div className="flex gap-1.5 flex-wrap">
          {(['hepsi','DEP','BGM'] as const).map((k)=> (
            <button key={k} data-testid={`katman-${k}`} onClick={()=>{setKatman(k); setModul('hepsi');}}
              className={`px-3 py-1 rounded-full text-[11px] font-bold border ${katman===k?'bg-slate-900 text-white border-slate-900':'bg-white border-slate-200'}`}>
              {k==='hepsi'?`Tümü (${katalog.length})`:k==='DEP'?`DEP-2026 (${katalog.filter(e=>(e.katman??'DEP')==='DEP').length})`:`BGM-12 (${katalog.filter(e=>e.katman==='BGM').length})`}
            </button>
          ))}
        </div>
        <div className="flex gap-1.5 flex-wrap">
          {moduller.map((m) => (
            <button key={m} data-testid={`kat-filtre-${m === 'hepsi' ? 'hepsi' : m.split(' ')[0]}`}
              onClick={() => setModul(m)}
              className={`px-2.5 py-1 rounded-lg text-[11px] border ${modul === m ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {m === 'hepsi' ? 'Tümü' : m}
            </button>
          ))}
        </div>
        <div className="rounded-2xl border border-slate-200 bg-slate-50 p-3 space-y-2">
          <div className="text-xs font-bold text-slate-700">{duzenId ? 'Etkinliği düzenle' : 'Yeni etkinlik ekle'} <span className="font-normal text-slate-500">· kayıt bu cihazda saklanır</span></div>
          <div className="grid sm:grid-cols-2 gap-2">
            <select data-testid="etk-katman" value={form.katman} onChange={(e)=>setForm({...form, katman:e.target.value as 'DEP'|'BGM', modulAdi: e.target.value==='BGM' ? 'BGM-12' : DEP_MODULLER[0].ad})} className="rounded-xl border border-slate-300 px-3 py-2 text-sm">
              <option value="DEP">DEP-2026</option><option value="BGM">BGM-12</option>
            </select>
            <input data-testid="etk-ad" value={form.ad} onChange={(e)=>setForm({...form, ad:e.target.value})} placeholder="Etkinlik adı *" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            <input data-testid="etk-kod" value={form.hedefKod} onChange={(e)=>setForm({...form, hedefKod:e.target.value})} placeholder="Hedef kod (örn 3.1.2 / BGM-EQ-01) *" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            {form.katman==='DEP' && <select data-testid="etk-modul" value={form.modulAdi} onChange={(e)=>setForm({...form, modulAdi:e.target.value})} className="rounded-xl border border-slate-300 px-3 py-2 text-sm">{DEP_MODULLER.map((m)=><option key={m.id} value={m.ad}>{m.id} · {m.ad}</option>)}</select>}
            <input data-testid="etk-ipucu" value={form.ipucuKademesi} onChange={(e)=>setForm({...form, ipucuKademesi:e.target.value})} placeholder="İpucu kademesi (örn Model→bağımsız)" className="rounded-xl border border-slate-300 px-3 py-2 text-sm" />
            <input data-testid="etk-malzeme" value={form.malzeme} onChange={(e)=>setForm({...form, malzeme:e.target.value})} placeholder="Malzeme (virgülle ayır)" className="sm:col-span-2 rounded-xl border border-slate-300 px-3 py-2 text-sm" />
          </div>
          <div className="flex gap-2">
            <button type="button" data-testid="etk-kaydet" onClick={kaydet} disabled={!form.ad.trim()||!form.hedefKod.trim()} className={`px-3 py-1.5 rounded-xl text-xs font-semibold ${!form.ad.trim()||!form.hedefKod.trim() ? 'bg-slate-200 text-slate-400 cursor-not-allowed' : 'bg-teal-600 text-white hover:bg-teal-700'}`}>{duzenId ? 'Güncelle' : 'Ekle'}</button>
            {duzenId && <button type="button" data-testid="etk-iptal" onClick={()=>{setDuzenId(null); setForm({ ad:'', hedefKod:'', modulAdi: DEP_MODULLER[0].ad, ipucuKademesi:'', malzeme:'', katman:'DEP'});}} className="px-3 py-1.5 rounded-xl text-xs border border-slate-300 bg-white">İptal</button>}
            <button type="button" data-testid="etk-sifirla" onClick={()=>{ setKatalog(ETKINLIKLER); setDuzenId(null); }} className="ml-auto text-[11px] text-slate-500 underline">Varsayılana sıfırla</button>
          </div>
        </div>
        <div className="grid sm:grid-cols-2 gap-3">
          {liste.map((e) => (
            <div key={e.id} data-testid="etkinlik-karti" className="rounded-xl border border-slate-200 p-3 space-y-1.5 bg-white">
              <div className="flex items-start justify-between gap-2">
                <span className="font-semibold text-sm">{e.ad} {(e.katman==='BGM') && <span className="ml-1 text-[10px] font-bold bg-sky-50 text-sky-700 border border-sky-200 rounded-full px-1.5">BGM</span>}</span>
                <span className={`text-[10px] font-bold border rounded-full px-2 py-0.5 shrink-0 ${e.katman==='BGM'?'bg-sky-50 text-sky-700 border-sky-200':'bg-teal-50 text-teal-700 border-teal-200'}`}>{e.hedefKod}</span>
              </div>
              <div className="text-[11px] text-slate-500">{e.modulAdi} · <span className={`text-[10px] font-bold px-1.5 py-0.5 rounded-full border ${e.katman==='BGM'?'bg-sky-50 text-sky-700 border-sky-200':'bg-emerald-50 text-emerald-700 border-emerald-200'}`}>{e.katman ?? 'DEP'}</span></div>
              <div className="text-xs"><b>İpucu kademesi:</b> {e.ipucuKademesi}</div>
              <div className="text-xs text-slate-600"><b>Malzeme:</b> {e.malzeme.join(' · ')}</div>
              <div className="flex gap-1.5 pt-1">
                <button type="button" data-testid={`etk-duzenle-${e.id}`} onClick={()=>duzenle(e.id)} className="text-[11px] px-2 py-1 rounded-lg border border-slate-200 bg-white">Düzenle</button>
                <button type="button" data-testid={`etk-sil-${e.id}`} onClick={()=>sil(e.id)} className="text-[11px] px-2 py-1 rounded-lg border border-rose-200 bg-rose-50 text-rose-700">Sil</button>
              </div>
            </div>
          ))}
        </div>
        <div data-testid="katalog-sinir" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900"><b>Hedef davranış kodları DEP-2026 terminolojisine REFERANSTIR</b> — program içeriği kopyalanmaz (K-83). Etkinlikler özgün içeriktir; kodlar yalnız BEP eşlemesini kolaylaştırmak için gösterilir.</div>
      </Kart>
    </>
  );
}

/* ---------- BGM-12 MENÜ (K-398) — sıra uzmanında, atlanabilir ---------- */
export function BgmMenu() {
  const [sec, setSec] = useState(DOSYALAR[0].uid);
  const [secim, setSecim] = useKalici<Record<string, string[]>>('bgm-secim', {
    'ÖĞR-4417': ['EQ-01', 'EQ-02', 'EQ-05'],
    'ÖĞR-2903': [],
  });
  const [acik, setAcik] = useState<string | null>('EQ-01');
  const siradaki = secim[sec] ?? [];
  const al = (id: string) => {
    if (siradaki.includes(id)) return;
    setSecim({ ...secim, [sec]: [...siradaki, id] });
  };
  const cikar = (id: string) => setSecim({ ...secim, [sec]: siradaki.filter((x) => x !== id) });
  const fazlar: BgmFaz[] = ['I', 'II', 'III'];
  return (
    <>
      <Kart baslik="Bilişsel Geliştirme Modülleri (BGM-12)"
        ek={<span className="text-[11px] text-slate-500">{BGM_SAYI} modül · menü</span>}>
        <div data-testid="bgm-katman" className="rounded-xl bg-sky-50 border border-sky-200 px-3 py-2 text-[11px] text-sky-900">
          <b>İki katman.</b> {BGM_KATMAN_NOTU}
        </div>
        <div data-testid="bgm-serbest" className="rounded-xl bg-teal-50 border border-teal-200 px-3 py-2 text-[11px] text-teal-900">
          <b>Modül seçimi serbesttir.</b> {MODUL_TERIM_NOTU} Persona sarmalı dayatılmaz.
        </div>
        <div data-testid="bgm-taslak" className="rounded-xl bg-amber-50 border border-amber-300 px-3 py-2 text-[11px] text-amber-900">
          <b>TASLAK.</b> {BGM_TASLAK_NOTU} Tam kartlar: <code>LEXIVA_K08-ICERIK/BGM-KARTLARI-SUPPORTA_v0.1.md</code>.
        </div>
        <div className="flex gap-2 flex-wrap">
          {DOSYALAR.map((d) => (
            <button key={d.uid} type="button" data-testid={`bgm-dosya-${d.uid}`} onClick={() => setSec(d.uid)}
              className={`px-3 py-1.5 rounded-xl text-sm border ${sec === d.uid ? 'bg-teal-600 text-white border-teal-600' : 'bg-white border-slate-200'}`}>
              {d.uid}
            </button>
          ))}
        </div>
        <p className="text-xs text-slate-600">
          Bu dosya için seçilen sıra (uzmanın sırası, müfredat sırası değil):{' '}
          <b data-testid="bgm-secili-liste">{siradaki.length ? siradaki.join(' → ') : 'henüz seçilmedi — 1-2-3 atlanabilir'}</b>
        </p>
      </Kart>
      {fazlar.map((f) => (
        <Kart key={f} baslik={BGM_FAZ_ETIKET[f]}>
          <div className="grid sm:grid-cols-2 gap-3">
            {BGM_MODULLER.filter((m) => m.faz === f).map((m) => {
              const secili = siradaki.includes(m.id);
              const ac = acik === m.id;
              return (
                <div key={m.id} data-testid={`bgm-kart-${m.id}`}
                  className={`rounded-xl border p-3 space-y-2 ${secili ? 'border-teal-400 bg-teal-50/40' : 'border-slate-200'}`}>
                  <div className="flex items-start justify-between gap-2">
                    <button type="button" className="text-left" onClick={() => setAcik(ac ? null : m.id)}>
                      <div className="font-semibold text-sm">{m.id} · {m.ad}</div>
                      <div className="text-[11px] text-slate-500">{m.kisa} · {m.okumaAlani}</div>
                    </button>
                    {m.oncelikli && <span className="text-[10px] font-bold bg-amber-50 text-amber-800 border border-amber-200 rounded-full px-2 py-0.5 shrink-0">çekirdek</span>}
                  </div>
                  <div className="flex gap-1.5">
                    {secili
                      ? <button type="button" data-testid={`bgm-cikar-${m.id}`} onClick={() => cikar(m.id)}
                          className="text-[11px] font-semibold px-2 py-1 rounded-lg bg-white border border-slate-300">Programdan çıkar</button>
                      : <button type="button" data-testid={`bgm-al-${m.id}`} onClick={() => al(m.id)}
                          className="text-[11px] font-semibold px-2 py-1 rounded-lg bg-teal-600 text-white">Programa al</button>}
                    <button type="button" data-testid={`bgm-ac-${m.id}`} onClick={() => setAcik(ac ? null : m.id)}
                      className="text-[11px] px-2 py-1 rounded-lg border border-slate-200">Kart</button>
                  </div>
                  {ac && (
                    <dl data-testid={`bgm-yuva-${m.id}`} className="text-[11px] space-y-1 text-slate-700 border-t border-slate-200 pt-2">
                      <div><b>Tanım:</b> {m.tanim}</div>
                      <div><b>Amaç:</b> {m.amac}</div>
                      <div><b>Ölçüm:</b> {m.olcum}</div>
                      <div><b>Etkinlik:</b> {m.etkinlik} <span className="text-slate-500">({m.sureDk})</span></div>
                      <div><b>Malzeme:</b> {m.malzeme.join(' · ')} · <b>İpucu:</b> {m.ipucu} · <b>Girdi:</b> {KODLAMA[m.girdiTipi].ad}</div>
                      <div><b>Ödev:</b> {m.odev}</div>
                      <div><b>Önlem:</b> {m.onlem}</div>
                      <div><b>Öneri:</b> {m.oneri}</div>
                      <div><b>DEP köprüsü:</b> {m.depKoprusu ? `${m.depKoprusu} — kanıt satırı önerisi; BEP birimi kararı değildir (K-263)` : 'yok (bütünleştirme turu)'}</div>
                      <div className="text-slate-500"><b>Dayanak:</b> {m.dayanak}</div>
                    </dl>
                  )}
                </div>
              );
            })}
          </div>
        </Kart>
      ))}
      <Sherh metin={SHERHLER.k02} ton="uyari" />
    </>
  );
}


~~~~

### `components/Kabuk.tsx`
3094 B ·SHA `374246402a4510fbd977ceaf62d62b5db43d3641fd54520fb7e3a6e6a6c12985`

~~~~tsx
/** Uygulama kabuğu: sol menü + üst bant. Veli rolü YOKTUR (K-296/KC7). */
import type { ReactNode } from 'react';
import { FolderOpen, CalendarDays, ClipboardList, BarChart3, FileText, Users, Settings, LayoutDashboard, BookOpen, FileCheck2, Home, Library, Brain } from 'lucide-react';
import { SHERHLER } from '../data/kisitlar';

export const EKRANLAR = [
  { id: 'pano', ad: 'Eğitmen Kürsüsü', ikon: LayoutDashboard },
  { id: 'dosyalar', ad: 'Dosyalar', ikon: FolderOpen },
  { id: 'takvim', ad: 'Takvim', ikon: CalendarDays },
  { id: 'oturum', ad: 'Oturum Atölyesi', ikon: ClipboardList },
  { id: 'katalog', ad: 'Etkinlik Kataloğu', ikon: Library },
  { id: 'cizelge', ad: 'İzleme Çizelgesi', ikon: BarChart3 },
  { id: 'rapor', ad: 'Rapor Atölyesi', ikon: FileText },
  { id: 'hizalama', ad: 'Program Hizalama', ikon: BookOpen },
  { id: 'bgm', ad: 'Bilişsel Geliştirme', ikon: Brain },
  { id: 'rambep', ad: 'RAM & BEP Takibi', ikon: FileCheck2 },
  { id: 'evodev', ad: 'Ev Çalışmaları', ikon: Home },
  { id: 'aile', ad: 'Aile & Öğretmen', ikon: Users },
  { id: 'ayarlar', ad: 'Ayarlar', ikon: Settings },
] as const;
export type EkranId = (typeof EKRANLAR)[number]['id'];

export default function Kabuk({ ekran, setEkran, rol, children }:
  { ekran: EkranId; setEkran: (e: EkranId) => void; rol: string; children: ReactNode }) {
  return (
    <div className="min-h-screen flex">
      <aside className="w-60 bg-white border-r border-slate-200 flex flex-col shrink-0">
        <div className="px-4 py-4 border-b border-slate-100">
          <div className="flex items-center gap-2">
            <div className="w-8 h-8 rounded-xl bg-teal-600 text-white grid place-items-center font-black">S</div>
            <div>
              <div className="font-bold text-sm">LEXIVA Supporta™</div>
              <div className="text-[10px] text-slate-500">Uzman Kokpiti · v{__SURUM__}</div>
            </div>
          </div>
        </div>
        <nav className="flex-1 p-2 space-y-0.5">
          {EKRANLAR.map((e) => {
            const I = e.ikon; const akt = ekran === e.id;
            return (
              <button key={e.id} type="button" data-testid={`nav-${e.id}`} onClick={() => setEkran(e.id)}
                className={`w-full flex items-center gap-2 px-3 py-2 rounded-xl text-sm transition-colors ${
                  akt ? 'bg-teal-600 text-white font-semibold' : 'text-slate-700 hover:bg-slate-100'}`}>
                <I className="w-4 h-4" /> {e.ad}
              </button>
            );
          })}
        </nav>
        <div className="p-3 border-t border-slate-100 text-[10px] text-slate-500">
          Rol: <b>{rol}</b> · Sentetik demo verisi
        </div>
      </aside>
      <main className="flex-1 min-w-0">
        <div className="bg-white border-b border-slate-200 px-6 py-2">
          <Sherhli />
        </div>
        <div className="p-6 space-y-5 max-w-6xl">{children}</div>
      </main>
    </div>
  );
}
function Sherhli() {
  return <p className="text-[11px] text-slate-600"><b>LEXIVA Supporta:</b> {SHERHLER.k02}</p>;
}

~~~~

### `components/Sherh.tsx`
628 B ·SHA `0270e18645a0065ba9acb123afda1e9936ab96b44e7bc1cf5cd262c0f93f391a`

~~~~tsx
/** Silinemez şerh bloğu (spec §7 · KC3: kullanıcı kapatamaz). */
import { ShieldAlert } from 'lucide-react';
export default function Sherh({ metin, ton = 'nötr' }: { metin: string; ton?: 'nötr' | 'uyari' }) {
  const s = ton === 'uyari'
    ? 'bg-amber-50 border-amber-300 text-amber-900'
    : 'bg-slate-50 border-slate-200 text-slate-600';
  return (
    <div data-testid="sherh" data-silinemez="true"
         className={`flex items-start gap-2 rounded-xl border px-3 py-2 text-[11px] leading-relaxed ${s}`}>
      <ShieldAlert className="w-3.5 h-3.5 shrink-0 mt-0.5" />
      <span>{metin}</span>
    </div>
  );
}

~~~~

### `components/aile/AileEgitimMerkezi.tsx`
6806 B ·SHA `bf6e90d5ee035a78f9a2a6a0c858c26e115ca301f29f02b4ea7074ca799a0699`

~~~~tsx
import { useState } from 'react';
import { AILE_GENEL_5 } from '../../data/aile/genel';
import { AILE_KISISEL_SABLON, AILE_KISISEL_HAVUZ } from '../../data/aile/kisisel';
import { SHERHLER } from '../../data/kisitlar';

export default function AileEgitimMerkezi({ dosyaUid }: { dosyaUid: string }) {
  const [sekme, setSekme] = useState<'A' | 'B'>('A');
  const [secili, setSecili] = useState<string>('AG-1');
  const [kopya, setKopya] = useState<string>('');

  const aktif = AILE_GENEL_5.find((x) => x.id === secili) ?? AILE_GENEL_5[0];

  const yazdir = (baslik: string, icerik: string) => {
    const html = `<!doctype html><title>${baslik}</title><style>body{font-family:system-ui;padding:32px;color:#0f172a}h1{font-size:18px}pre{white-space:pre-wrap;font-size:13px;border:1px solid #e2e8f0;padding:12px;border-radius:10px}.muhur{border:2px solid #059669;color:#059669;display:inline-block;padding:4px 8px;font-weight:900;font-size:11px;border-radius:8px}.kopya{margin-top:12px;border-top:1px dashed #94a3b8;padding-top:8px;font-size:11px;color:#64748b}</style><h1>${baslik} — ${dosyaUid}</h1><div class=muhur>ONAYLI — K-02 / K-08 TASLAK — UZMAN SEÇER</div><pre>${icerik}</pre><div class=kopya>Kopya 1/2 — Aile/Veli &nbsp;|&nbsp; Kopya 2/2 — Kurum arşivi · ${new Date().toISOString().slice(0,10)} · Supporta v${typeof __SURUM__ !== 'undefined' ? __SURUM__ : '0.8.4'} · ${SHERHLER.aile}</div><script>window.print()<\/script>`;
    const w = window.open('', '_blank');
    if (w) { w.document.write(html); w.document.close(); }
  };

  return (
    <div className="space-y-4">
      <div className="flex gap-2">
        <button
          type="button"
          data-testid="aile-sekme-A"
          onClick={() => setSekme('A')}
          className={`px-3 py-1.5 rounded-xl text-sm ${sekme === 'A' ? 'bg-teal-600 text-white' : 'bg-slate-100'}`}
        >
          A — Genel (5 mini-modül)
        </button>
        <button
          type="button"
          data-testid="aile-sekme-B"
          onClick={() => setSekme('B')}
          className={`px-3 py-1.5 rounded-xl text-sm ${sekme === 'B' ? 'bg-teal-600 text-white' : 'bg-slate-100'}`}
        >
          B — Analize Göre (uzman seçer)
        </button>
      </div>

      {sekme === 'A' ? (
        <div className="grid md:grid-cols-3 gap-4">
          <div className="space-y-2">
            {AILE_GENEL_5.map((k) => (
              <button
                key={k.id}
                type="button"
                data-testid={`aile-genel-${k.id}`}
                onClick={() => setSecili(k.id)}
                className={`w-full text-left p-3 rounded-xl border text-sm ${secili === k.id ? 'border-teal-600 bg-teal-50' : 'border-slate-200 bg-white'}`}
              >
                <div className="font-semibold">{k.baslik}</div>
                <div className="text-xs text-slate-500">{k.sureDk} dk · {k.amac.slice(0, 60)}…</div>
              </button>
            ))}
          </div>
          <div className="md:col-span-2 bg-white border border-slate-200 rounded-xl p-4 space-y-3">
            <div className="font-bold">{aktif.baslik}</div>
            <div className="text-sm text-slate-600">{aktif.amac}</div>
            <ul className="list-disc pl-5 text-sm space-y-1">
              {aktif.icerik.map((m, i) => (
                <li key={i}>{m}</li>
              ))}
            </ul>
            {aktif.malzeme.length > 0 && <div className="text-xs text-slate-500">Malzeme: {aktif.malzeme.join(', ')}</div>}
            {aktif.uyari && <div className="text-xs text-amber-700 bg-amber-50 border border-amber-200 rounded-lg p-2">{aktif.uyari}</div>}
            <div className="flex gap-2">
              <button
                type="button"
                data-testid="aile-yazdir-A"
                onClick={() => yazdir(aktif.baslik, `${aktif.amac}\n\n${aktif.icerik.join('\n- ')}\n\nMalzeme: ${aktif.malzeme.join(', ') || '—'}\n${aktif.uyari ?? ''}`)}
                className="px-3 py-1.5 rounded-xl bg-teal-600 text-white text-sm"
              >
                Yazdır / PDF
              </button>
              <button
                type="button"
                data-testid="aile-kopyala-A"
                onClick={() => {
                  const t = `${aktif.baslik}\n${aktif.amac}\n${aktif.icerik.join('\n')}`;
                  navigator.clipboard?.writeText(t);
                  setKopya('Kopyalandı');
                  setTimeout(() => setKopya(''), 1500);
                }}
                className="px-3 py-1.5 rounded-xl bg-slate-100 text-sm"
              >
                Kopyala
              </button>
              {kopya && <span className="text-xs text-teal-700 py-1.5">{kopya}</span>}
            </div>
            <p className="text-[11px] text-slate-500">{SHERHLER.aile} · K-08 TASLAK — harici Turnitin/hukuk şirket sonrası.</p>
          </div>
        </div>
      ) : (
        <div className="bg-white border border-slate-200 rounded-xl p-4 space-y-3">
          <div className="font-bold">{AILE_KISISEL_SABLON.baslik}</div>
          <div className="text-sm text-slate-600">{AILE_KISISEL_SABLON.baglam}</div>
          <div className="text-xs text-slate-500">Havuzdan 1 başlık seçin — sistem otomatik seçmez, uzman seçer (K-02).</div>
          <div className="grid md:grid-cols-3 gap-2">
            {AILE_KISISEL_HAVUZ.map((h) => (
              <div key={h.id} className="p-3 rounded-xl border border-slate-200 bg-slate-50">
                <div className="font-semibold text-sm">{h.baslik}</div>
                <div className="text-xs text-slate-500">Tetik: {h.tetik}</div>
              </div>
            ))}
          </div>
          <pre className="text-xs bg-slate-50 border border-slate-200 rounded-xl p-3 whitespace-pre-wrap">{AILE_KISISEL_SABLON.uzmanNotuSablonu}</pre>
          <div className="text-sm">
            <span className="font-semibold">Aileye görev örneği:</span> {AILE_KISISEL_SABLON.aileyeGorev}
          </div>
          <div className="text-xs text-slate-500">Ölçüm: {AILE_KISISEL_SABLON.olcum}</div>
          <div className="flex gap-2">
            <button
              type="button"
              data-testid="aile-yazdir-B"
              onClick={() => yazdir(AILE_KISISEL_SABLON.baslik, `${AILE_KISISEL_SABLON.uzmanNotuSablonu}\n\nGörev: ${AILE_KISISEL_SABLON.aileyeGorev}\nÖlçüm: ${AILE_KISISEL_SABLON.olcum}`)}
              className="px-3 py-1.5 rounded-xl bg-teal-600 text-white text-sm"
            >
              Şablonu Yazdır
            </button>
          </div>
          <p className="text-[11px] text-slate-500">{SHERHLER.aile} · B’de sistem öneri üretmez, uzman yazar (K-02). Rapor/Çizelge B-4 kartıyla birlikte verilir.</p>
        </div>
      )}
    </div>
  );
}

~~~~

### `components/egitmen/EgitmenDestekPaneli.tsx`
5441 B ·SHA `d3c595bdae6baab3ab8fe291d91ec1fcb11985876591c5567067d11cfa5b7b06`

~~~~tsx
// K-651: SUPPORTA (Merkez) - Eğitmen Destek Paneli
// Dalga 2 Eğitsel Zeka: Support Fading (Desteği Geri Çekme) ve Recovery (Mola Sonrası Toparlanma)

import { useState } from 'react';

interface OgrenciProfil {
  id: string;
  ad: string;
  aktifDestek: string;
  basariSerisi: number; // Support Fading tetikleyicisi
  enIyiToparlanma: string; // Recovery profil verisi
}

const MOCK_OGRENCILER: OgrenciProfil[] = [
  { id: '1', ad: 'Can B.', aktifDestek: 'Görsel İpucu', basariSerisi: 4, enIyiToparlanma: 'Düşük Uyaranlı Görev' },
  { id: '2', ad: 'Ali Y.', aktifDestek: 'Görev Parçalama', basariSerisi: 1, enIyiToparlanma: 'Sözel Yönerge' },
  { id: '3', ad: 'Elif S.', aktifDestek: 'Zamanlayıcı', basariSerisi: 5, enIyiToparlanma: 'Hareketli Mola' },
];

export default function EgitmenDestekPaneli() {
  const [secili, setSecili] = useState<OgrenciProfil>(MOCK_OGRENCILER[0]);

  // Kural: 3 ve üzeri başarılı görevde destek azaltma önerilir
  const isFadingReady = secili.basariSerisi >= 3;

  return (
    <div className="p-6 bg-slate-50 min-h-screen">
      <h1 className="text-2xl font-bold text-slate-800 border-b border-slate-300 pb-3 mb-6">
        Eğitmen Destek Paneli (Supporta)
      </h1>

      <div className="flex gap-6">
        {/* Sol Menü: Öğrenci Seçimi */}
        <div className="w-1/3 bg-white p-4 rounded-xl shadow-sm border border-slate-200">
          <h2 className="text-sm font-semibold text-slate-500 mb-4 uppercase tracking-wider">Öğrenci Listesi</h2>
          <div className="flex flex-col gap-2">
            {MOCK_OGRENCILER.map((ogr) => (
              <button
                key={ogr.id}
                onClick={() => setSecili(ogr)}
                className={`p-3 text-left rounded-lg transition-all ${
                  secili.id === ogr.id 
                    ? 'bg-blue-600 text-white shadow-md' 
                    : 'bg-slate-100 text-slate-700 hover:bg-slate-200'
                }`}
              >
                {ogr.ad}
                {ogr.basariSerisi >= 3 && <span className="ml-2 text-yellow-300">💡</span>}
              </button>
            ))}
          </div>
        </div>

        {/* Sağ Panel: Profil ve İçgörüler */}
        <div className="w-2/3 flex flex-col gap-4">
          
          {/* Support Fading Modülü */}
          <div className="bg-white p-5 rounded-xl shadow-sm border border-slate-200">
            <h3 className="text-lg font-bold text-slate-800 mb-1">Destek Profili</h3>
            <p className="text-sm text-slate-500 mb-4">Şu an uygulanan destek stratejisi ve performansı.</p>
            
            <div className="p-4 bg-blue-50 border border-blue-100 rounded-lg">
              <div className="flex justify-between items-center">
                <div>
                  <p className="text-sm text-blue-600 font-medium">Aktif Destek (Müdahale)</p>
                  <p className="text-xl font-bold text-blue-900">{secili.aktifDestek}</p>
                </div>
                <div className="text-right">
                  <p className="text-sm text-blue-600 font-medium">İstikrarlı Başarı Serisi</p>
                  <p className="text-xl font-bold text-blue-900">{secili.basariSerisi} Görev</p>
                </div>
              </div>
            </div>

            {isFadingReady && (
              <div className="mt-4 p-4 bg-emerald-50 border border-emerald-200 rounded-lg flex items-start gap-3">
                <div className="text-2xl">💡</div>
                <div>
                  <h4 className="font-bold text-emerald-900">Desteği Geri Çekme Önerisi (Support Fading)</h4>
                  <p className="text-sm text-emerald-800 mt-1">
                    Bu öğrenci <b>{secili.aktifDestek}</b> stratejisinde uzmanlaştı. Bağımsızlığı artırmak adına, 
                    sonraki seansta desteği bir alt seviyeye indirmeyi (Fading) deneyebilirsiniz.
                  </p>
                  <button className="mt-3 px-4 py-2 bg-emerald-600 hover:bg-emerald-700 text-white text-sm font-semibold rounded-md transition-colors">
                    Desteği Azalt / Kaldır
                  </button>
                </div>
              </div>
            )}
          </div>

          {/* Recovery Profile Modülü */}
          <div className="bg-white p-5 rounded-xl shadow-sm border border-slate-200">
            <h3 className="text-lg font-bold text-slate-800 mb-1">Toparlanma (Recovery) Zekası</h3>
            <p className="text-sm text-slate-500 mb-4">Öğrencinin moladan veya kriz anından sonra en hızlı toparlandığı koşullar.</p>
            
            <div className="p-4 bg-purple-50 border border-purple-100 rounded-lg flex items-center justify-between">
              <div>
                <p className="text-sm text-purple-600 font-medium">En Verimli Dönüş (Transition) Aracı:</p>
                <p className="text-lg font-bold text-purple-900">{secili.enIyiToparlanma}</p>
              </div>
              <div className="text-purple-300 text-4xl">⏱️</div>
            </div>
            <p className="text-xs text-purple-700 mt-2">
              Öneri: Mola dönüşlerinde yüksek uyaranlı veya zor görevlerden kaçının. Başlangıçta <b>{secili.enIyiToparlanma}</b> vererek bilişsel geçişi (transition) kolaylaştırın.
            </p>
          </div>

        </div>
      </div>
    </div>
  );
}

~~~~

### `data/aile/genel.ts`
3423 B ·SHA `02aa484f6ae03c642fec3d5de84a8068c18ebdcc8b3958ba249f77d889d5e491`

~~~~tsx
/** A — Genel Davranış-Tutum Bilgilendirme (5 mini-modül, her aileye aynı — önleyici)
 *  Kaynak kavramı: MEB ÖGG Aile Rehberi Tablo 11/12 + §7 + Z-7 — cümle kopyalanmadan, kavram düzeyinde özet (K-08).
 *  K-08 pedagog onayı 04.09 kullanıcı, K-02 dili, K-14 gözlemlenebilir dil, K-15 dijital puan YOK.
 *  TASLAK — şirket sonrası Turnitin + hukuk tek pakette.
 */
export interface AileGenelKart {
  id: string;
  baslik: string;
  amac: string;
  icerik: string[]; // 3-4 madde, kavram özetleri
  sureDk: number;
  malzeme: string[];
  uyari?: string;
}

export const AILE_GENEL_5: AileGenelKart[] = [
  {
    id: 'AG-1',
    baslik: 'Nasihat ve Kıyas Yok — Gözlem Dili',
    amac: 'Eleştiri/nasihat/kıyas yerine gözlemlenebilir davranış dili kurmak.',
    icerik: [
      '“Nasihat, eleştiri, öğüt ve başkaları ile kıyaslamak hiç yardımcı olmaz” — MEB §7 ilkesi kavram özetidir.',
      '“Yaramaz” yerine “10 dk derste 3 kez ayağa kalktı” gibi sayılabilir + bağlamlı cümle kurun (K-14).',
      'Günlük 1 olumlu gözlem notu yazın (basılabilir kart, dijital puan yok).',
    ],
    sureDk: 15,
    malzeme: ['A4 gözlem kartı', 'kalem'],
    uyari: 'Yorum/değer yargısı yok — yalnızca gözlem.',
  },
  {
    id: 'AG-2',
    baslik: 'Rutin Kartı — Ne, Ne Zaman, Nerede, Ne Kadar, Sonra Ne',
    amac: 'Yazılı planla öngörülebilirlik sağlamak (Z-1).',
    icerik: [
      'Akşam rutinini 5 soruyla duvara asın: ne yapılacak · ne zaman · nerede · ne kadar · sonra ne var (Tablo 9/10 kavramı).',
      'Resimli/renkli kartta her adım tek satır, tik kutusu ekleyin.',
      'Planı çocukla birlikte hazırlayın, her gün aynı yerde tutun.',
    ],
    sureDk: 20,
    malzeme: ['rutin şablonu (A4)', 'renkli kalem'],
  },
  {
    id: 'AG-3',
    baslik: 'Görsel Ortam — Uyaran Yalıtımı',
    amac: 'Çalışma yüzeyinde çeldiriciyi azaltmak (Tablo 12 + Z-7 görsel).',
    icerik: [
      'Masada yalnızca o derste gerekli materyal kalsın, fazlası kutuya.',
      'Dersten önce yüzey toplama ritüeli: 1 dk birlikte toplayın.',
      'Duvarlarda hareketli/ışıklı uyaranı çalışma anında kaldırın.',
    ],
    sureDk: 10,
    malzeme: ['toplama kutusu'],
  },
  {
    id: 'AG-4',
    baslik: 'İşitsel Ortam — Gürültü Azaltma ve Kısa Yönerge',
    amac: 'İşitsel çeldiriciyi azaltıp yönergeyi kısaltmak (Tablo 11 + Z-7 işitsel).',
    icerik: [
      'Çalışma anında TV/arka plan sesini kapatın, kapıyı kapalı tutun.',
      'Yönergeyi göz hizasında, tek cümle, 2 adımı geçmeden söyleyin.',
      'Gerekirse söze değil, hafif dokunarak (omuz) ilgisini çekin.',
    ],
    sureDk: 10,
    malzeme: [],
  },
  {
    id: 'AG-5',
    baslik: 'Pekiştireç ve Kayıt — Hedef Davranış + İpucu',
    amac: 'Hedef davranışı küçük adımla pekiştirip kayıt tutmak (EK-12 uyumlu çerçeve, Z-2).',
    icerik: [
      'Tek hedef seçin: “ödevin ilk 10 dk’sında masada kalma”.',
      'İpucu kademesi: model → sözel hatırlatma → bağımsız; ipucunu kademeli çekin.',
      'Her gün “yaptı / yapmadı” tik kartına işleyin, haftalık uzmana getirin (dijital puan yok).',
    ],
    sureDk: 15,
    malzeme: ['hedef kartı', 'tik tablosu'],
    uyari: 'Pekiştireç maddi değil, etkinlik/övgü temelli olabilir — uzman belirler.',
  },
];

~~~~

### `data/aile/kisisel.ts`
2063 B ·SHA `5042b956dea4e9d4869d08eaff71f19c471ba1cf1f1bcb8b6ad70d087d78e758`

~~~~tsx
/** B — Çocuğun Analiz Sonuçlarına Göre Aile Eğitimi (kişiselleştirilmiş, uzmanın seçtiği 1 kart)
 *  K-02: sistem otomatik öneri ÜRETMEZ — uzman B-4/C-3 rapordan seçer, veliye iletir.
 *  K-14: gözlemlenebilir + sayılabilir + bağlamlı dil. K-15: dijital puan YOK, basılabilir.
 *  K-08: TASLAK — şirket sonrası Turnitin/hukuk.
 */

export interface AileKisiselSablon {
  id: string;
  baglam: string; // hangi analiz tetikler (ör: izleme çizelgesinde “odak kopma >X”)
  baslik: string;
  uzmanNotuSablonu: string; // boş alan, uzman doldurur — sistem doldurmaz
  aileyeGorev: string; // 1 görev, 1 ipucu formatında
  olcum: string; // nasıl kayıt tutulacak (tik, süre)
}

export const AILE_KISISEL_SABLON: AileKisiselSablon = {
  id: 'AB-1',
  baglam: 'İzleme Çizelgesi / Rapor Atölyesi’ndeki B-4 kartı + öğretmenin pasif yüklediği Gözlem Formu (K-16) → uzman yorumu',
  baslik: 'Analize Göre Aile Görevi (Uzman Seçer)',
  uzmanNotuSablonu: `[UZMAN DOLDURUR — K-02]\nGözlem/Rapor bulgusu (tarihli, sayılabilir): ...\nAileye önerilen tek görev (1 cümle, bağlamlı): ...\nİpucu kademesi (model/sözel/bağımsız): ...\nKayıt biçimi (tik/süre): ...\nSonraki izleme tarihi: ...\n`,
  aileyeGorev: 'Haftada 3 kez, “ödevin ilk 10 dk’sında masada kalma” görevini rutin kartıyla uygulayın; ipucu: sözel hatırlatma → bağımsız.',
  olcum: 'Tik tablosu: her gün “yaptı/yapmadı” + süre (dk). Haftalık seansa getirin.',
};

// Havuzdan seçim için 3 örnek başlık (uzman havuzdan 1’ini seçer, sistem seçmez)
export const AILE_KISISEL_HAVUZ = [
  { id: 'BK-1', baslik: 'Dikkat kopma sık → Görsel yalıtım + kısa yönerge (AG-3/AG-4 pekiştirme)', tetik: 'Çizelgede kopma > eşik' },
  { id: 'BK-2', baslik: 'Rutin kurulamıyor → Rutin Kartı (AG-2) + aileye 1 görev', tetik: 'Ev Çalışmaları “yapılmadı” >2' },
  { id: 'BK-3', baslik: 'Pekiştireçte tutarsızlık → Hedef+Kayıt (AG-5) sadeleştirme', tetik: 'Girdi “0/3” yoğun' },
] as const;

~~~~

### `data/bgm.ts`
16146 B ·SHA `263f592cf1c347295ab7df07beec615df9eae71b0da82a4bcea0b750fa511b17`

~~~~tsx
/**
 * Bilişsel Geliştirme Modülleri (BGM-12) — Supporta menü katmanı.
 * Kaynak: CURRICULUM v1.3 §5 · TANIM KARTLARI v1.6 KART 2 · K-267 · K-393 · K-398 · K-400.
 * (SEDUVA'daki DEHB yürütücü-işlev BGM-12 menüsü LEXIVA'da devredilmez; EQ kodlu okuma menüsü kullanılır.)
 *
 * Bu katman DEP-2026'dan AYRI durur:
 *   DEP  = BEP/RAM resmî saat-modül hizası (Program Hizalama)
 *   BGM  = okuma/fonolojik içerik menüsü (bu dosya; LEXIVA; K-700 ÖÖG uyarlama)
 * Uzman her ikisinden de seçer; sabit 12'li sıra YOKTUR (MODUL_SECIM_SERBEST).
 *
 * Dil: K-02 — tanı/tedavi/terapi iddiası yok; etki vaadi yok.
 * CURRICULUM kalıntıları (Bio-Sync, limbik, ms-beyin, "körlük") DEVRALINMAZ.
 */

export type BgmFaz = 'I' | 'II' | 'III';

export type BgmModul = {
  id: string;
  ad: string;
  kisa: string;
  faz: BgmFaz;
  okumaAlani: string;
  tanim: string;
  amac: string;
  olcum: string;
  etkinlik: string;
  odev: string;
  onlem: string;
  oneri: string;
  /** KART 2 "öncelikli çekirdek" */
  oncelikli: boolean;
  /** v0.8.0 (K-400) — etkinlik alan seti (DEP M4 ile aynı desen) */
  /** Bu BGM'nin KANIT üretebileceği DEP-2026 modülü; öneri — BEP birimi kararı değil (K-263). */
  depKoprusu: string | null;
  /** YASA-1: BGM etkinliği girdi üretir; varsayılan kodlama tipi. */
  girdiTipi: 'xArti' | 'sifirUc' | 'evetHayir';
  sureDk: string;
  malzeme: string[];
  ipucu: string;
  /** Ödev var mı (DS-10 / CM-11: yok). */
  odevVar: boolean;
  /** Dayanak = görev ailesi / kategori ATFI. Etki iddiası değil (K-04). */
  dayanak: string;
};

export const BGM_FAZ_ETIKET: Record<BgmFaz, string> = {
  I: 'Grup I — fonolojik temel (sıra değil)',
  II: 'Grup II — okuma/yazma/matematik (sıra değil)',
  III: 'Grup III — aktarım ve özerklik (sıra değil)',
};

export const BGM_MODULLER: readonly BgmModul[] = [
  {
    id: 'EQ-01', ad: 'Ses Merdiveni', kisa: 'Fonolojik eşleme',
    faz: 'I', okumaAlani: 'Fonolojik farkındalık',
    tanim: 'Merdiven ardıl sırasıyla (sözcük→uyak→hece→sesbirimi) basamak basamak ilerleme pratiği (DEP 3.2.1: önce eşleme).',
    amac: 'Başlangıç-sesi farkındalığını merdiven üstünde izlenebilir kılmak; uzman hedefi BEP satırına taşır.',
    olcum: 'Basamak isabeti (0–3) · eşleme/ayırt etme tutarlılığı. Bant/eşik ve tanı YOK (K-02).',
    etkinlik: 'Merdiven şeması üzerinde 2 örnek eşleme (model), sonra 6 sözcük bağımsız tur.',
    odev: 'Evde 5 sözcüğün başlangıç sesini eşleştirin (kavram; resmî form metni değil). Puanlanmaz.',
    onlem: 'Masada yalnız merdiven şeması ve ses kartları; ekran görüş alanında olmasın.',
    oneri: 'Uzman notu boş bırakılır; sistem kişiye özel tavsiye üretmez.',
    oncelikli: true,
    depKoprusu: 'M3', girdiTipi: 'sifirUc', sureDk: '5–7 dk',
    malzeme: ['merdiven şeması', 'ses kartları (6)', 'kum saati'],
    ipucu: 'model → sözel ("ilk sesi yakala") → bağımsız',
    odevVar: true,
    dayanak: '2021 DEP 3.1/3.2.1 ardıl sıra · MEB Ses Farkındalık Öğretmen Kılavuzu (yapı atfı; K-08)',
  },
  {
    id: 'EQ-02', ad: 'Ses Birimi Ayırt Etme', kisa: 'Harf seçiciliği',
    faz: 'I', okumaAlani: 'Fonolojik farkındalık',
    tanim: 'Karışık harf dizisinde hedef dışı uyaranı (X) seçip durma pratiği — fonolojik seçicilik.',
    amac: 'Harf düzeyinde seçiciliği (okumaya taşınan çekirdek) seans içi verilerle izlemek.',
    olcum: 'Isabet / kaçırma · erken basış adedi (SBA deseni). Yüzdelik yorumu ve tanı YOK (K-02).',
    etkinlik: 'SBA turu: X dışındaki harflerde BOŞLUK, X’te bekle (Persona ile aynı motor).',
    odev: 'Evde 3 heceli sözcükleri hecederken ilk sesi vurgulama. Puan yok.',
    onlem: 'Kısa tur (5–7 dk); ardışık zorlamada mola (çocuk kontrol çubuğu).',
    oneri: 'Seans sonu yansıma: “Hangi harfi bekledin?” — sistem yorumlamaz.',
    oncelikli: true,
    depKoprusu: 'M3', girdiTipi: 'sifirUc', sureDk: '5–7 dk',
    malzeme: ['ekran (SBA)', 'ses kartları'],
    ipucu: 'model → sözel ("X’te bekle") → bağımsız',
    odevVar: true,
    dayanak: '2021 DEP 3.2.1 ayırt etme basamağı · D-L1 merdiven (LEXIVA müfredat matrisi v0.3)',
  },
  {
    id: 'EQ-03', ad: 'Hece ve Parçalar', kisa: 'Sözcüğü bölme',
    faz: 'I', okumaAlani: 'Fonolojik parçalama',
    tanim: 'Sözcüğün hecelere/ses birimlerine bölünmesi — yönetilebilir birimlere ayırma.',
    amac: 'Parçalama-tamamlama döngüsünü görür kılmak; “büyük sözcük” direncini ilk adımla kırmak.',
    olcum: 'Hece bölme doğruluğu (x/+) · parça sayısı (betimleyici). Ölçüm yorumunu uzman yazar.',
    etkinlik: 'El çırparak heceleme: mar-tı (2), ke-le-bek (3); 8 kartlık bağımsız tur.',
    odev: 'Yarınki okuma kartındaki 3 sözcüğü heceleyin. Sistem puanlamaz.',
    onlem: 'Yönerge en fazla 2 adım; vurgulu söyleme modeli önce.',
    oneri: 'İpucu kademesi: model → sözel → bağımsız; silikleştirme notu uzmanda.',
    oncelikli: false,
    depKoprusu: 'M3', girdiTipi: 'xArti', sureDk: '6–8 dk',
    malzeme: ['hece kartları (8)', 'parçalama şeridi'],
    ipucu: 'model (uzman bölür) → sözel → bağımsız (çocuk bölür)',
    odevVar: true,
    dayanak: '2021 DEP 3.1 (hece basamağı) · MEB Ses Farkındalık (yapı atfı; K-08)',
  },
  {
    id: 'EQ-04', ad: 'Harf Tanıma ve Çizim', kisa: 'b/d-l izleme',
    faz: 'I', okumaAlani: 'Görsel-tanım / yazım',
    tanim: 'Harf şeklinin tanınması ve karışım çiftlerinde (b/d, p/q, l/g) kinestetik izleme.',
    amac: 'Harf şekli → ses eşlemesine görsel taban hazırlamak; ters çevirme gözlemi.',
    olcum: 'Çizim isabeti (x/+) · karışım çifti hata adedi (betimleyici).',
    etkinlik: 'Havada/parmakla model çizim → büyük puntolu sayfada 4× b-d-l izleme.',
    odev: 'Evde harf kartlarıyla 10 dk eşleştirme. Puan yok.',
    onlem: 'Tek harf başına kısa tur; karışım çiftinde sözel onay ("bu b, b-b-b").',
    oneri: 'Karışım çifti sıklığı yalnız gözlem; "becerememe" dili yok.',
    oncelikli: false,
    depKoprusu: 'M3', girdiTipi: 'xArti', sureDk: '5 dk',
    malzeme: ['büyük puntolu çizim sayfası', 'harf kartları'],
    ipucu: 'fiziksel izleme → model → sözel',
    odevVar: true,
    dayanak: '2021 DEP 1.4/3.2 · LEXIVA Harf Çizim görevi (müfredat matrisi v0.3)',
  },
  {
    id: 'EQ-05', ad: 'Söyleneni Yaz', kisa: 'İşitsel yazım',
    faz: 'II', okumaAlani: 'Yazma',
    tanim: 'Söylenen sözcükleri yazma + hataları sınıflandırma (atlama/ters/ekleme/karıştırma).',
    amac: 'Yazım üretimini cezasız tekrar hakkıyla destekleyip hata sınıfını verilebilir kılmak.',
    olcum: 'Sözcük isabeti (x/+) · hata sınıfı dağılımı (ÖGG Gözlem Formu Yazma deseni). Yorum uzmanda.',
    etkinlik: '6 sözcük söylene yazılır; hatalı yazımlar hata sınıfı kartına tiklenir.',
    odev: 'Kapıya asılı 3 sözcüklük "yanına al" listesi. Puan yok.',
    onlem: 'Sözcük başına 1 tekrar hakkı; düzeltme değil, işaretleme + birlikte inceleme.',
    oneri: 'Hata sınıfı trendi telemetriye işlenir; bant/eşik üretilmez (K-02).',
    oncelikli: true,
    depKoprusu: 'M3', girdiTipi: 'xArti', sureDk: '6 dk',
    malzeme: ['yazım yaprağı', 'hata sınıfı kartları (4)'],
    ipucu: 'model → sözel → bağımsız',
    odevVar: true,
    dayanak: 'MEB ÖGG Gözlem Formu Yazma m.2/5/6/7 · DEP 1.4 (yapı atfı; K-08)',
  },
  {
    id: 'EQ-06', ad: 'Akıcı Okuma', kisa: 'Tekrarlı okuma',
    faz: 'II', okumaAlani: 'Akıcılık (D-L2)',
    tanim: 'Hedef metinde tekrarlı okuma; doğru sözcük/dk kaydı + M-4 veli işaretleme köprüsü.',
    amac: 'Akıcılık turunu ev-okul ortak kaydıyla (M-4) izlenebilir kılmak.',
    olcum: 'Doğru sözcük/dk (doğru×60/sn) · tur içi kazanım. Bant/eşik YOK (K-02).',
    etkinlik: 'Tanıt (uzman okur) → 2–3 tekrarlı tur (süre tutulur) → M-4 formu hazırlanır.',
    odev: 'Günde 5–10 dk sesli okuma (AG-2); M-4 formuna işaret. Puan yok.',
    onlem: 'Metin bant düzeyi çocuğun düzeyine göre; zorlayıcı metin seçilmez.',
    oneri: 'M-4 ev kaydı ile seans verisi aynı zaman çizgisinde karşılaştırılır (yalnız uzman).',
    oncelikli: true,
    depKoprusu: 'M4', girdiTipi: 'xArti', sureDk: '8–10 dk',
    malzeme: ['hedef metin (bantlı)', 'süre sayacı', 'M-4 formu'],
    ipucu: 'eşli okuma → tek başına (süre tutulur)',
    odevVar: true,
    dayanak: 'D-L2 tekrarlı okuma · MEB akıcılık formülü (2025 kit deseni; K-08)',
  },
  {
    id: 'EQ-07', ad: 'Sözcük Çantası', kisa: 'Kelime dağarcığı',
    faz: 'II', okumaAlani: 'Sözcük dağarcığı (DEP M2.2)',
    tanim: 'Günün 5 yeni sözcüğünün anlam + üretim döngüsüyle kalıcı belleğe taşınması.',
    amac: 'Sözcüğü tanıma → üretim → tekrar üçlüsüyle izlemek.',
    olcum: 'Üretim isabeti (0–3) · tekrar turunda geri çağırma (betimleyici).',
    etkinlik: 'Çantaya ekleme → anlam kartı → "çantadan al, cümleye koy" üretimi.',
    odev: 'Yarının 5 sözcüğü akşam yemeğinde cümle içinde kullanılır. Puan yok.',
    onlem: 'Sözcük sayısı 5 ile sınırlı; aşırı yükleme yok.',
    oneri: 'Çanta içeriği veliyle paylaşılır; karşılaştırma dili yok.',
    oncelikli: false,
    depKoprusu: 'M2', girdiTipi: 'sifirUc', sureDk: '5 dk',
    malzeme: ['sözcük kartları (5)', 'çanta görseli'],
    ipucu: 'model → sözel → bağımsız',
    odevVar: true,
    dayanak: '2021 DEP M2.2 (sözcük dağarcığı) · LEXIVA kelime görevi',
  },
  {
    id: 'EQ-08', ad: 'Anlama Kartı', kisa: 'Okudunu söyle',
    faz: 'II', okumaAlani: 'Anlama',
    tanim: 'Kısa bantlı metin okuma/dinleme sonrası 3 soruda (ne/kim/nerede) anlamı ifade etme.',
    amac: 'Anlamanın sözel ayağını (ifade) kısa ve güven veren biçimde izlemek.',
    olcum: 'Anlama kartı isabeti (E/H) · cümleyle ifade (gözlem).',
    etkinlik: '4–5 cümlelik metin (2 geçiş) → 3 anlama kartı; her kart 1 cümle.',
    odev: 'Evde okunan kitap için 1 soru (aile sorusu). Puan yok.',
    onlem: 'Uzun yanıt beklenmez; 1 cümle yeterli (Z-15 dili).',
    oneri: 'Anlama zorlanmasında metin bant düzeyi gözden geçirilir (uzman).',
    oncelikli: false,
    depKoprusu: 'M4', girdiTipi: 'evetHayir', sureDk: '6 dk',
    malzeme: ['kısa metin kartı (bantlı)', 'anlama kartları (3)'],
    ipucu: 'model → sözel → bağımsız',
    odevVar: true,
    dayanak: 'D-L2 anlama alt ayağı · LEXIVA anlama görevi',
  },
  {
    id: 'EQ-09', ad: 'Sayı Blokları', kisa: 'Çokluk ve karıştırma',
    faz: 'II', okumaAlani: 'Matematik (D-L4)',
    tanim: 'Çokluk-sayı eşlemesi + karıştırma çiftleri (6/9, 1/7) ayırt etme.',
    amac: 'Somuttan soyuta köprüyü ve karıştırma seçiciliğini izlemek.',
    olcum: 'Eşleme isabeti (E/H) · karıştırma çifti hata adedi (betimleyici).',
    etkinlik: '8 blok say → sayı kartıyla eşle; "6 mı 9 mu?" karıştırma çifti kartları.',
    odev: 'Yemek masasında "kaç tabak?" sayma pratiği. Puan yok.',
    onlem: 'Karıştırım çiftinde somut blok gösterilir; sözel onay ile pekiştirme.',
    oneri: 'Sayı blokları telemetrisi MENTORIA raporuna işlenir (yalnız uzman yorumu).',
    oncelikli: false,
    depKoprusu: 'M5', girdiTipi: 'evetHayir', sureDk: '5 dk',
    malzeme: ['sayı blokları (8)', 'sayı kartları', 'karıştırma çifti kartları'],
    ipucu: 'model → isaret → bağımsız',
    odevVar: true,
    dayanak: '2021 DEP 4.3/5.1 · ÖGG Gözlem Formu Mat m.3 (yapı atfı; K-08)',
  },
  {
    id: 'EQ-10', ad: 'Süre Algısı', kisa: 'Süre tahmini',
    faz: 'II', okumaAlani: 'Süre tahmini (seans içi)',
    tanim: 'Bir işin ne kadar süreceğini tahmin etme ve gerçek süreyle karşılaştırma.',
    amac: '“Az kaldı / çok kaldı” hissini sayılabilir süreyle eşlemek (seans içi süre; takvim değil).',
    olcum: 'Tahmin − gerçek süre farkı (sn). Persona “Süre Algısı (Ritim)” ile aynı aile.',
    etkinlik: 'Kum saati tahmini: uzman 30/60/90 sn tutar, çocuk işaretler.',
    odev: 'Akşam rutininin bir adımına süre koyun (ör. çanta hazırlığı). Puan yok.',
    onlem: 'Görünür analog saat veya kum saati; "acele et" yerine süre göstergesi.',
    oneri: 'Geçiş uyarısı (Z-13) seans bitimine 5 ve 1 dk kala — utançsız dil.',
    oncelikli: false,
    depKoprusu: 'M4', girdiTipi: 'sifirUc', sureDk: '5 dk',
    malzeme: ['kum saati / analog kronometre', 'tahmin kartı'],
    ipucu: 'görsel sayaç açık → yarı kapalı → kapalı',
    odevVar: true,
    dayanak: 'süre tahmini görev ailesı · PMC 5-küme ③ rutin-zamanlama (literatür atfı)',
  },
  {
    id: 'EQ-11', ad: 'Transfer ve Serbest Okuma', kisa: 'Yeni metine taşıma',
    faz: 'III', okumaAlani: 'Aktarım (D-L7)',
    tanim: 'Kazanılan okuma becerisinin farklı metin/ortam/kişiye taşınma gözlemi (T2/T3).',
    amac: 'Kazanımın yeni metin türlerinde (serbest okuma, günlük) ortaya çıkmasını izlemek.',
    olcum: 'Yeni metinde akıcılık (doğru sözcük/dk) · Transfer Gözlem Kartı notu (uzman).',
    etkinlik: 'Bant dışı kısa metinlerle serbest okuma turları; çocuk kendi metnini seçer.',
    odev: 'Kendi seçtiği kitapla 10 dk sesli okuma (AG-2). Puan yok.',
    onlem: 'Yeni metinde zorlanma olursa bant düzeyine dönülür (yükleme artırmaz).',
    oneri: 'Transfer kartı MENTORIA rapor akışına besler (BATARYA §5).',
    oncelikli: false,
    depKoprusu: 'M4', girdiTipi: 'xArti', sureDk: '6–8 dk',
    malzeme: ['serbest okuma metinleri (bant dışı)', 'transfer gözlem kartı'],
    ipucu: 'uzman yanımda → aynı odada → ayrı (kademeli)',
    odevVar: true,
    dayanak: 'D-L7 aktarım ayağı · LEXIVA serbest okuma görevi',
  },
  {
    id: 'EQ-12', ad: 'Okuma Özerkliği', kisa: 'Dış iskeleti solma',
    faz: 'III', okumaAlani: 'Üstbiliş / otonomi',
    tanim: 'Hazır görevi çocuğun kendi planlaması; hatırlatıcı kademeli azalır (metakognisyon ONAYLI konum).',
    amac: 'Platform iskeletini solmak; günlük 10 dk sesli okuma rutinine (AG-2) yerleştirmek.',
    olcum: 'Hatırlatıcısız başlama (E/H) · planladığı okumaya dönüş. Öz-başlatma betimleyicidir.',
    etkinlik: 'Çocuk bugünkü gerçek işini (kitap/ödev) planlar; uzman yalnız izler, ipucu isterse verir.',
    odev: 'Kendi yazdığı 3 kutuluk planı odasına asmak (yazılı plan kavramı). Puan yok.',
    onlem: 'Karşılaştırma dili yok; her geribildirimde en az bir güçlü yön (Z-15).',
    oneri: 'Sistem otonomi ilan etmez; karar uzman + ailededir.',
    oncelikli: false,
    depKoprusu: 'M6', girdiTipi: 'xArti', sureDk: '8–10 dk',
    malzeme: ['3 kutulu plan kartı', 'çocuğun kendi kitabı'],
    ipucu: 'istek üzerine → yok',
    odevVar: true,
    dayanak: 'metakognisyon konumlandırma v1.0 (K-118/119) · ipucu silikleştirme deseni',
  },
] as const;
export const BGM_SAYI = BGM_MODULLER.length; // 12
export const BGM_ONCELIKLI = BGM_MODULLER.filter((m) => m.oncelikli).map((m) => m.id);
export const BGM_KATMAN_NOTU =
  'Okuma menüsü (12), DEP-2021\'in yerine geçmez. DEP = BEP/RAM saat hizası; menü = okuma/fonolojik içerik. Uzman ikisinden de seçer.';

/** LEXIVA uyarlama (K-700); ürün metinleri DÜRÜSTLUK NOTLU TASLAKTIR. */
export const BGM_TASLAK_NOTU =
  'Menü kart metinleri LEXIVA müfredat matrisi v0.3 + 2021 DEP hiza (K-08: kavram taşınır, cümle kopyalanmaz) üzerinden uyarlanmıştır. Etki iddiası içermez.';

/** BGM etkinliği kimliği — Oturum Atölyesi'nde DEP etkinlikleriyle aynı listede, ayrı etiketle (YASA-1). */
export const bgmEtkinlikId = (modulId: string) => `BGM-${modulId}`;
export const bgmEtkinlikMi = (etkinlikId: string) => etkinlikId.startsWith('BGM-');
export const bgmModulden = (etkinlikId: string) =>
  BGM_MODULLER.find((m) => bgmEtkinlikId(m.id) === etkinlikId) ?? null;

~~~~

### `data/kisitlar.ts`
6494 B ·SHA `74a82043bab369716b7ab338a9d8058bd5111e778da4314e3851dd338bc0879d`

~~~~tsx
/**
 * LEXIVA Supporta™ — KALICI KISITLAR (spec §1; K-700 ÖÖG uyarlama)
 * Bu dosya ürünün "anayasası"dır: şerhler silinemez, YASA'lar arayüzde zorlanır.
 * Kaynak: supporta-mvp-spec_v0.2.md · K-263 · K-281 · K-296 · K-331 · K-334 · K-88
 */

/** YASA-1: her performans girdisi BİR etkinliğe bağlıdır; etkinliksiz girdi sisteme girmez. */
export const YASA_1 = 'Girdi yalnızca bir etkinliğe bağlı olarak kaydedilebilir.';
/** YASA-2: çizelge motoru etkinlik motorundan doğar (bağımsız çizelge yok). */
export const YASA_2 = 'Çizelge girdilerden türetilir; elle bağımsız çizelge oluşturulamaz.';
/** YASA-3: her rapor taslaktır; uzman onayı olmadan geçerli belge değildir. */
export const YASA_3 = 'Rapor taslaktır; uzman onayı olmadan geçerli belge değildir.';

/** Ekranlarda SİLİNEMEZ sabit şerhler (spec §7). */
export const SHERHLER = {
  oturum: 'Etkinlik eşliğinde gözlemdir; bireysel izleme amaçlıdır.',
  cizelge: 'Akran karşılaştırması yoktur; çocuk yalnız kendi zaman serisiyle izlenir.',
  rapor: 'TASLAKTIR; uzman onayı olmadan geçerli belge değildir. Resmî formun yerine geçmez (K-263).',
  aile: 'Veli sistem erişimi yoktur; veli bilgilendirilen taraf ve veri kaynağıdır (K-296).',
  hizali: 'Gözlem özetidir; değerlendirme veya resmî form değildir; BEP birimi kararının yerine geçmez.',
  k02: 'LEXIVA Supporta bir yapılandırılmış özel eğitim destek ortamıdır. Tanı, tedavi veya terapi uygulamaz; uygulama içi test UYGULANMAZ (K-02); uzman kullanır.',
} as const;

/** DEP-2026 modül yapısı — giriş YALNIZ elle; hiçbir MEB sisteminden çekilmez (Y3 kırmızı çizgi). */
export const DEP_MODULLER = [
  { id: 'M1', ad: 'Öğrenmeye Destek', saat: 150, bolum: 5 },
  { id: 'M2', ad: 'Dil ve İletişim', saat: 150, bolum: 4 },
  { id: 'M3', ad: 'Okuma ve Yazma', saat: 300, bolum: 6 },
  { id: 'M4', ad: 'Erken Matematik', saat: 200, bolum: 8 },
  { id: 'M5', ad: 'Matematik', saat: 200, bolum: 4 },
  { id: 'M6', ad: 'Sosyal Etkileşim', saat: 100, bolum: 3 },
] as const;
export const DEP_TOPLAM_SAAT = DEP_MODULLER.reduce((t, m) => t + m.saat, 0); // 1100
export const DEP_SEMA_SURUM = 'DEP-2026 (ORGM 2026_01)';

/** Girdi kodlama tipleri (spec M5). */
export const KODLAMA = {
  xArti: { ad: 'x / +', aciklama: 'x: hedeflenen · +: ulaşılan (PKF deseni)' },
  sifirUc: { ad: '0-3', aciklama: 'ölçüt düzeyi (PBF deseni)' },
  evetHayir: { ad: 'Evet / Hayır', aciklama: 'gözlendi / gözlenmedi (KDF deseni)' },
} as const;

/** Oturum durumları (spec M2). */
export const OTURUM_DURUM = ['planlandı', 'tamamlandı', 'iptal', 'gelmedi'] as const;
export type OturumDurum = (typeof OTURUM_DURUM)[number];

/**
 * K-267 TERİM KURALI: birim adı **MODÜL**'dür ("hafta" değil).
 * Kapsayıcı ad: "Bilişsel Geliştirme Modülleri" (CURRICULUM §5 başlığı köklü).
 * K-393: Supporta'da modüller **sıralı değildir**.
 * K-398: kural BGM-12 menüsüne de uygulanır (KART 2). DEP-2026 ayrı katmandır.
 */
export const MODUL_SECIM_SERBEST = true;
export const MODUL_TERIM_NOTU =
  'Modüller sıralı değildir; uzman çocuğun durumuna göre seçer, atlayabilir ve sırayı kendisi belirler.';

/** ÖEK Yönetmeliği (RG 11/7/2025-32953) kaynaklı KAPSAM DIŞI çizgileri (K-330). */
export const KAPSAM_DISI = [
  { ad: 'Devam/yoklama takibi', gerekce: 'BKDS Bakanlık standardındadır (md.25/A); ödeme şartıdır (md.29/1-ı). Supporta devam takibi YAPMAZ.' },
  { ad: 'Ödeme · fatura · idari-mali işleyiş', gerekce: 'K-334 kalıcı kapsam çizgisi: eğitim desteği ürünüyüz; merkezin idari-mali işleyişine girmeyiz.' },
  { ad: 'Resmî form üretimi', gerekce: 'K-263: sistem resmî formun yerine geçmez; yalnız kanıt/taslak üretir.' },
] as const;

/** Ders saati tavanları — ÖEK Yön. md.24/4 (güncel resmî sınır; ürün bunları AŞAN plan önermez). */
export const DERS_TAVAN = {
  aylikBireysel: 12, aylikGrup: 4, haftalikBireysel: 4, haftalikGrup: 2,
  gunlukToplam: 3, telafiPenceresiAy: 24,
} as const;

/**
 * DEP-2026 resmî FORM AİLESİ (EK-1…EK-7) — kaynak: LEXIVA-BEP-FORM-ESLEMESI_v1.0 (K-370).
 * K-395: LEXIVA'da çıkarılan bu eşleme ÖZEL EĞİTİM GENELİDİR; Supporta'ya da aittir.
 * Supporta KANIT üretir · uzman KARAR verir · RAM ONAYLAR. Form doldurulmaz (K-263).
 */
export const RESMI_FORMLAR = [
  { ek: 'EK-1', ad: 'Ölçüt Bağımlı Test (ÖBT)', an: 'ilk / ara / son değ.',
    besleyen: 'Tekrar ve deneme sayısı → Ölçüt alanı', tur: 'kanıt' },
  { ek: 'EK-2', ad: 'Kontrol Listesi', an: 'ilk / ara / son değ.',
    besleyen: 'Evet/Hayır girdileri → Açıklamalar sütunu', tur: 'kanıt' },
  { ek: 'EK-3', ad: 'Dereceli Puanlama Anahtarı', an: 'değerlendirme',
    besleyen: '0-3 ölçüt girdileri → performans düzeyi (atamayı uzman yapar)', tur: 'kanıt' },
  { ek: 'EK-4', ad: 'Performans Kayıt Formu', an: 'her modülün başı ve sonu',
    besleyen: 'x/+ girdileri → Ön/Son sütununa kanıt (işareti uzman koyar)', tur: 'kanıt' },
  { ek: 'EK-5', ad: 'BEP Gelişimi İzleme Özet Formu', an: 'süreç + yıl sonu',
    besleyen: 'Hata/gözlem dağılımı → Ulaşılamama nedenleri ve Öneriler', tur: 'kanıt' },
  { ek: 'EK-6', ad: 'Portfolyo Kontrol Listesi', an: 'modül sonu / yıl sonu',
    besleyen: 'Oturum sürekliliği + dışa aktarım → portfolyo dosyası (RAM onayına gider)', tur: 'dosya' },
  { ek: 'EK-7', ad: 'Portfolyo Dereceli Puanlama Anahtarı', an: 'portfolyo değ.',
    besleyen: '—', tur: 'kapsam dışı' },
] as const;

/** Kayıt hattı ayrımı — ÖEKY md.20/2 (RG 11/7/2025-32953). İki farklı süreç. */
export const KAYIT_HATTI = [
  { id: 'a', ad: '(a) Ücreti Bakanlıkça karşılanan', ram: 'ZORUNLU (rapor + ÖEDK planı + BKDS onamı)',
    planlama: 'ÖEDK eğitim planı ekseninde' },
  { id: 'b', ad: '(b) Ücretini kendisi/velisi karşılayan', ram: 'İSTENMİYOR',
    planlama: 'Kayıttaki ölçme sonuçlarıyla BEP birimince (md.24/6 · md.26/3)' },
] as const;
export type KayitHatti = (typeof KAYIT_HATTI)[number]['id'];

/** Roller ve yetkiler (spec §3). VELİ ROLÜ YOKTUR (K-296/KC7). */
export const ROLLER = [
  { id: 'yonetici', ad: 'Yönetici', yetki: 'Tüm dosyalar · rapor onayı · dışa aktarma' },
  { id: 'uzman', ad: 'Uzman / Eğitimci', yetki: 'Kendi dosyaları · oturum · girdi · rapor taslağı' },
] as const;
export type RolId = (typeof ROLLER)[number]['id'];

~~~~

### `data/mock.ts`
13867 B ·SHA `5d29e601257751e21e4827df7a579acc59a98b2f1f365cbf2e6ff8489a4f7cbf`

~~~~tsx
/** Sentetik demo verisi — K-05: prototipte GERÇEK ÇOCUK VERİSİ YOKTUR.
 *  Maskeli UID + kurgusal ad; yaş bandı 8-10 (K-270). */
import type { Dosya, Program, Oturum, Etkinlik, Girdi, Rapor, EvOdevi, RamKaydi } from './tipler';

export const DOSYALAR: Dosya[] = [
  { uid: 'ÖĞR-4417', ad: 'Öğrenci A. (2. Sınıf)', dogum: '2018-04-12', okulSinif: 'Atatürk İlkokulu / 2-B',
    devamsizlikNotu: 'Son ayda 2 gün', gecmisBepNotu: 'RAM eğitsel değerlendirme mevcut (2025)',
    veli: { ad: 'Veli A.', tel: '05xx xxx 41 17', adres: 'İzmir / Bornova', rizaTarihi: '2026-08-20' } },
  { uid: 'ÖĞR-2903', ad: 'Öğrenci B. (3. Sınıf)', dogum: '2017-11-03', okulSinif: 'Cumhuriyet İlkokulu / 3-A',
    devamsizlikNotu: '—', gecmisBepNotu: 'BEP dosyası okuldan bekleniyor',
    veli: { ad: 'Veli B.', tel: '05xx xxx 29 03', adres: 'İzmir / Karşıyaka', rizaTarihi: '2026-09-01' } },
];

export const PROGRAMLAR: Program[] = [
  { dosyaUid: 'ÖĞR-4417', seansSayisi: 24, siklik: 'Haftada 1 (40 dk)', aileBileseni: true,
    ramRaporRef: 'RAM-2025/1184', depModul: 'M3', depSaat: 300, depSemaSurum: 'DEP-2026 (ORGM 2026_01)', kayitHatti: 'a' },
  { dosyaUid: 'ÖĞR-2903', seansSayisi: 16, siklik: 'Haftada 1 (40 dk)', aileBileseni: false,
    ramRaporRef: '—', depModul: null, depSaat: null, depSemaSurum: 'DEP-2026 (ORGM 2026_01)', kayitHatti: 'b' },
];

export const OTURUMLAR: Oturum[] = [
  { id: 'OT-101', dosyaUid: 'ÖĞR-4417', tarih: '2026-09-03', saat: '10:00', durum: 'tamamlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-102', dosyaUid: 'ÖĞR-4417', tarih: '2026-09-10', saat: '10:00', durum: 'planlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-103', dosyaUid: 'ÖĞR-2903', tarih: '2026-09-03', saat: '10:00', durum: 'planlandı', sureDk: 40, uzmanId: 'UZM-1' },
  { id: 'OT-104', dosyaUid: 'ÖĞR-2903', tarih: '2026-08-27', saat: '11:00', durum: 'gelmedi', sureDk: 40, uzmanId: 'UZM-2' },
];

export const ETKINLIKLER: Etkinlik[] = [
  { id: 'ET-1', ad: 'Hece ayırma çalışması', hedefKod: '3.1.2', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Sözel ipucu → model → bağımsız', malzeme: ['hece kartları', 'çalışma yaprağı'], katman: 'DEP' },
  { id: 'ET-2', ad: 'Sesli okuma — tekrarlı', hedefKod: '3.3.1', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Eşli okuma → bağımsız', malzeme: ['kısa metin', 'kronometre'], katman: 'DEP' },
  { id: 'ET-3', ad: 'Görsel dikkat eşleme', hedefKod: '1.1.3', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'İşaret → sözel → bağımsız', malzeme: ['eşleme kartları'], katman: 'DEP' },
  { id: 'ET-4', ad: 'İşitsel bellek dizisi', hedefKod: '1.2.1', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Model → gecikmeli model → bağımsız', malzeme: ['ses kartları'], katman: 'DEP' },
  { id: 'ET-5', ad: 'Sözcük dağarcığı — nesne adlandırma', hedefKod: '2.2.1', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Fiziksel ipucu → sözel → bağımsız', malzeme: ['nesne resimleri'], katman: 'DEP' },
  { id: 'ET-6', ad: 'Nesne niteliği ayırt etme', hedefKod: '4.1.2', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → kısmi ipucu → bağımsız', malzeme: ['blok seti'], katman: 'DEP' },
  { id: 'ET-7', ad: 'Ritmik sayma (100 içinde)', hedefKod: '5.1.4', modulAdi: 'Matematik',
    ipucuKademesi: 'Birlikte sayma → bağımsız', malzeme: ['sayı doğrusu'], katman: 'DEP' },
  { id: 'ET-8', ad: 'Sıra alma ve bekleme', hedefKod: '6.2.3', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Model → sözel hatırlatma → bağımsız', malzeme: ['sıra kartı', 'kum saati'], katman: 'DEP' },
  // — v0.8.1 genişletme: her modüle +2/3 ek (toplam 24, 4×6) —
  { id: 'ET-9', ad: 'Sürdürülebilir dikkat — nesne takibi', hedefKod: '1.3.2', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Model → sözel ipucu → bağımsız', malzeme: ['renkli toplar', 'tepsi'], katman: 'DEP' },
  { id: 'ET-10', ad: 'Yönerge izleme (2 adımlı)', hedefKod: '1.4.1', modulAdi: 'Öğrenmeye Destek',
    ipucuKademesi: 'Fiziksel rehber → sözel → bağımsız', malzeme: ['yönerge kartları'], katman: 'DEP' },
  { id: 'ET-11', ad: 'Dinlediğini anlama — kısa öykü', hedefKod: '2.1.3', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Sözel ipucu → soru-cevap → bağımsız', malzeme: ['öykü kartı', 'soru listesi'], katman: 'DEP' },
  { id: 'ET-12', ad: 'Sözel ifade — cümle kurma', hedefKod: '2.3.2', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Model cümle → tamamlama → bağımsız', malzeme: ['kelime kartları'], katman: 'DEP' },
  { id: 'ET-13', ad: 'Karşılıklı konuşma sürdürme', hedefKod: '2.4.1', modulAdi: 'Dil ve İletişim',
    ipucuKademesi: 'Sözel başlatma → sıra alma → bağımsız', malzeme: ['konu kartları', 'kum saati'], katman: 'DEP' },
  { id: 'ET-14', ad: 'Harf-ses eşleme', hedefKod: '3.2.1', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Model → eşleme → bağımsız', malzeme: ['harf kartları', 'ses kutusu'], katman: 'DEP' },
  { id: 'ET-15', ad: 'Yazma — harf dikte', hedefKod: '3.4.2', modulAdi: 'Okuma ve Yazma',
    ipucuKademesi: 'Noktalı iz → kopya → bağımsız', malzeme: ['dikte yaprağı', 'kalem'], katman: 'DEP' },
  { id: 'ET-16', ad: 'Gruplama / sınıflama', hedefKod: '4.2.3', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → sözel ipucu → bağımsız', malzeme: ['sınıflama kutuları', 'nesneler'], katman: 'DEP' },
  { id: 'ET-17', ad: 'Birebir eşleştirme', hedefKod: '4.3.1', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Fiziksel rehber → bağımsız', malzeme: ['eş kartları'], katman: 'DEP' },
  { id: 'ET-18', ad: 'Sıralama (büyük-küçük)', hedefKod: '4.4.2', modulAdi: 'Erken Matematik',
    ipucuKademesi: 'Model → deneme-yanılma → bağımsız', malzeme: ['sıralama şeridi'], katman: 'DEP' },
  { id: 'ET-19', ad: 'Sayı doğrusu ile toplama', hedefKod: '5.2.2', modulAdi: 'Matematik',
    ipucuKademesi: 'Model → rehberli → bağımsız', malzeme: ['sayı doğrusu', 'pul'], katman: 'DEP' },
  { id: 'ET-20', ad: 'Çıkarma (nesne ile)', hedefKod: '5.2.4', modulAdi: 'Matematik',
    ipucuKademesi: 'Nesne desteği → zihinden', malzeme: ['sayma pulları'], katman: 'DEP' },
  { id: 'ET-21', ad: 'Günlük yaşam problemi kurma', hedefKod: '5.3.1', modulAdi: 'Matematik',
    ipucuKademesi: 'Sözel senaryo → model → bağımsız', malzeme: ['problem kartları'], katman: 'DEP' },
  { id: 'ET-22', ad: 'Duygu tanıma', hedefKod: '6.1.2', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Görsel ipucu → eşleme → bağımsız', malzeme: ['duygu kartları'], katman: 'DEP' },
  { id: 'ET-23', ad: 'İş birliği oyunu', hedefKod: '6.3.1', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Eşli oyun → sıra alma → bağımsız', malzeme: ['kutu oyunu'], katman: 'DEP' },
  { id: 'ET-24', ad: 'Kurala uyma (oyun)', hedefKod: '6.3.3', modulAdi: 'Sosyal Etkileşim',
    ipucuKademesi: 'Model → hatırlatma → bağımsız', malzeme: ['kural kartı'], katman: 'DEP' },

  // — v0.8.3 BGM-12 etkinlikleri — katalogda ayrı filtre (DEP ile karıştırma yok; K-398 kuyruğu) —
  { id: 'ET-BGM-EQ-01', ad: 'BGM — Ses Merdiveni (Fonolojik Eşleme)', hedefKod: 'BGM-EQ-01', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['merdiven şeması', 'ses kartları', 'kum saati'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-02', ad: 'BGM — Ses Birimi Ayırt Etme (SBA Turu)', hedefKod: 'BGM-EQ-02', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['ekran (SBA)', 'ses kartları'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-03', ad: 'BGM — Hece ve Parçalar (El Çırparak Heceleme)', hedefKod: 'BGM-EQ-03', modulAdi: 'BGM-12', ipucuKademesi: 'Model (uzman bölür) → sözel → bağımsız', malzeme: ['hece kartları', 'parçalama şeridi'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-04', ad: 'BGM — Harf Tanıma ve Çizim (b/d-l İzleme)', hedefKod: 'BGM-EQ-04', modulAdi: 'BGM-12', ipucuKademesi: 'Fiziksel izleme → model → sözel', malzeme: ['büyük puntolu sayfa', 'harf kartları'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-05', ad: 'BGM — Söyleneni Yaz (Hata Sınıfı ile)', hedefKod: 'BGM-EQ-05', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['yazım yaprağı', 'hata sınıfı kartları'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-06', ad: 'BGM — Akıcı Okuma (Tekrarlı + M-4)', hedefKod: 'BGM-EQ-06', modulAdi: 'BGM-12', ipucuKademesi: 'Eşli okuma → tek başına', malzeme: ['hedef metin', 'süre sayacı', 'M-4 formu'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-07', ad: 'BGM — Sözcük Çantası (Günün 5 Sözcüğü)', hedefKod: 'BGM-EQ-07', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['sözcük kartları (5)', 'çanta görseli'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-08', ad: 'BGM — Anlama Kartı (Okudunu Söyle)', hedefKod: 'BGM-EQ-08', modulAdi: 'BGM-12', ipucuKademesi: 'Model → sözel → bağımsız', malzeme: ['kısa metin kartı', 'anlama kartları (3)'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-09', ad: 'BGM — Sayı Blokları (Çokluk + Karıştırma Çifti)', hedefKod: 'BGM-EQ-09', modulAdi: 'BGM-12', ipucuKademesi: 'Model → isaret → bağımsız', malzeme: ['sayı blokları', 'sayı kartları'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-10', ad: 'BGM — Süre Algısı (Kum Saati Tahmini)', hedefKod: 'BGM-EQ-10', modulAdi: 'BGM-12', ipucuKademesi: 'Görsel sayaç açık → yarı kapalı → kapalı', malzeme: ['kum saati', 'tahmin kartı'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-11', ad: 'BGM — Transfer ve Serbest Okuma', hedefKod: 'BGM-EQ-11', modulAdi: 'BGM-12', ipucuKademesi: 'Uzman yanımda → aynı odada → ayrı', malzeme: ['serbest okuma metinleri', 'transfer kartı'], katman: 'BGM' },
  { id: 'ET-BGM-EQ-12', ad: 'BGM — Okuma Özerkliği (Kendi Planım)', hedefKod: 'BGM-EQ-12', modulAdi: 'BGM-12', ipucuKademesi: 'İstek üzerine → yok', malzeme: ['3 kutulu plan kartı', 'çocuğun kendi kitabı'], katman: 'BGM' },
];

export const GIRDILER: Girdi[] = [
  { id: 'G-1', oturumId: 'OT-101', etkinlikId: 'ET-1', kodlamaTipi: 'xArti', deger: '+', tarih: '2026-09-03', girenRol: 'uzman' },
  { id: 'G-2', oturumId: 'OT-101', etkinlikId: 'ET-2', kodlamaTipi: 'sifirUc', deger: '2', tarih: '2026-09-03', girenRol: 'uzman' },
  { id: 'G-3', oturumId: 'OT-101', etkinlikId: 'ET-3', kodlamaTipi: 'evetHayir', deger: 'Evet', tarih: '2026-09-03', girenRol: 'uzman' },
];

export const RAPORLAR: Rapor[] = [
  { id: 'R-1', dosyaUid: 'ÖĞR-4417', tur: 'seans', baslik: 'Seans Özeti — 03.09.2026',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Hece ayırma etkinliğinde hedef davranışa ulaşıldı (+). Sesli okumada ölçüt düzeyi 2. Görsel dikkat eşlemede gözlendi.' },
  { id: 'R-2', dosyaUid: 'ÖĞR-4417', tur: 'aylik', baslik: 'Aylık Gelişim Özeti — Ağustos 2026',
    taslak: false, onayKim: 'Yönetici', onayTarih: '2026-09-01', kopyaSayisi: 2,
    icerik: 'Dört oturumun üçü tamamlandı, biri gelmedi. Okuma ekseninde hedef davranış sıklığı arttı; hece ayırmada bağımsız düzeye geçiş gözlendi.' },
  { id: 'R-3', dosyaUid: 'ÖĞR-4417', tur: 'donem', baslik: 'Dönem Sonu Değerlendirme — 2026 Güz',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Dönem boyunca 12 oturum planlandı, 10 tamamlandı. M3 Okuma ve Yazma modülünde 3.1 ve 3.3 bölümlerinde çalışıldı. Güçlü yön: tekrarlı okumada süreklilik.' },
  { id: 'R-4', dosyaUid: 'ÖĞR-4417', tur: 'bep-ilerleme', baslik: 'BEP İlerleme Taslağı — 3.1 Erken Okuryazarlık',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Hedef davranış 3.1.2 (hece ayırma): ön değerlendirmede x, son değerlendirmede +. Gözlem tarih damgalıdır; amaç/ölçüt/yöntem üretilmemiştir. GÜÇLÜ YÖN: çalışmaya istekli katılım.' },
  { id: 'R-5', dosyaUid: 'ÖĞR-4417', tur: 'ram-paketi', baslik: 'RAM İzleme Paketi Hazırlığı',
    taslak: true, onayKim: null, onayTarih: null, kopyaSayisi: 0,
    icerik: 'Portfolyo içeriği: performans kayıt formları (3 oturum), gözlem özeti, program hizalama çıktısı. Kurum kontrolü sonrası RAM\'a iletilir; iki kopya üretilir.' },
  { id: 'R-6', dosyaUid: 'ÖĞR-4417', tur: 'aile-bilgilendirme', baslik: 'Aile Bilgilendirme Çıktısı — Eylül',
    taslak: false, onayKim: 'Uzman / Eğitimci', onayTarih: '2026-09-02', kopyaSayisi: 1,
    icerik: 'Bu hafta hece çalışmalarına odaklandık. Evde: gazete başlıklarındaki kelimeleri birlikte hecelemeniz süreci destekler. Jargon kullanılmamıştır.' },
];

export const EV_ODEVLERI: EvOdevi[] = [
  { id: 'EV-1', dosyaUid: 'ÖĞR-4417', baslik: 'Mutfakta hece avı (5 nesne)', kim: 'Veli',
    neZaman: 'Hafta içi 3 gün · 10 dk', durum: 'yapıldı', not: 'Çocuk istekliydi; 4 nesne bağımsız heceledi.' },
  { id: 'EV-2', dosyaUid: 'ÖĞR-4417', baslik: 'Gazete başlığı okuma', kim: 'Veli',
    neZaman: 'Hafta sonu · 1 kez', durum: 'verildi', not: '' },
  { id: 'EV-3', dosyaUid: 'ÖĞR-2903', baslik: 'Sayı kartlarıyla eşleme', kim: 'Veli',
    neZaman: 'Hafta içi 2 gün', durum: 'yapılmadı', not: 'Aile yoğunluk bildirdi; süre kısaltıldı.' },
];

export const RAM_KAYITLARI: RamKaydi[] = [
  { dosyaUid: 'ÖĞR-4417', raporNo: 'RAM-2025/1184', tarih: '2025-10-14', gecerlilik: '2026-10-14',
    edifDurumu: 'İlk İnceleme tamamlandı (e-Rehberlik)', portfolyoHazir: true, sonrakiIzleme: '2026-09-30' },
  { dosyaUid: 'ÖĞR-2903', raporNo: '—', tarih: '—', gecerlilik: '—',
    edifDurumu: '(b) hattı — RAM raporu istenmiyor (ÖEKY md.20/2)', portfolyoHazir: false, sonrakiIzleme: '—' },
];

~~~~

### `data/tipler.ts`
2371 B ·SHA `a5a9977eb421c7071197c877c826f5926be4bdd57099bfb5618bef51b2c26d16`

~~~~tsx
/** LEXIVA Supporta™ — veri modeli (spec §5; K-700 ÖÖG uyarlama). */
import type { OturumDurum } from './kisitlar';

export interface Veli { ad: string; tel: string; adres: string; rizaTarihi: string | null; }
export interface Dosya {
  uid: string; ad: string; dogum: string; okulSinif: string;
  devamsizlikNotu: string; veli: Veli; gecmisBepNotu: string;
}
export interface EvOdevi {
  id: string; dosyaUid: string; baslik: string; kim: string;
  neZaman: string; durum: 'verildi' | 'yapıldı' | 'yapılmadı'; not: string;
}
export interface RamKaydi {
  dosyaUid: string; raporNo: string; tarih: string; gecerlilik: string;
  edifDurumu: string; portfolyoHazir: boolean; sonrakiIzleme: string;
}
export interface Program {
  dosyaUid: string; seansSayisi: number; siklik: string;
  aileBileseni: boolean; ramRaporRef: string;
  depModul: string | null; depSaat: number | null; depSemaSurum: string;
  kayitHatti: 'a' | 'b';   // ÖEKY md.20/2
}
export interface Oturum {
  id: string; dosyaUid: string; tarih: string; saat: string;
  durum: OturumDurum; sureDk: number; uzmanId: string;
}
export interface Etkinlik {
  id: string; ad: string; hedefKod: string; modulAdi: string;
  ipucuKademesi: string; malzeme: string[]; katman?: 'DEP' | 'BGM';
}
export interface Girdi {
  id: string; oturumId: string; etkinlikId: string;   // YASA-1: etkinlik ZORUNLU
  kodlamaTipi: 'xArti' | 'sifirUc' | 'evetHayir';
  deger: string; tarih: string; girenRol: string;
  ipucuGozlem?: IpucuGozlem;   // K-571/A4 (opsiyonel; eski-veri güvenli)
}
/** K-571/A4: uzmanın GÖZLEDİĞİ ipucu-kademesi (etkinlik-ipucuKademesi planlıdır; bu alan oturum-ayakta teyididir — K-02: gözlem-kaydı, ölçüm-değil). */
export type IpucuGozlem = 'model' | 'sozel' | 'bagimsiz';
/** K-571/A2: veli görüşme-randevu defteri kaydı — hatırlatma GÖNDERİLMEZ (K-334); defter yalnız yerel (K-05). */
export interface Gorusme {
  id: string; dosyaUid: string; tarih: string; konu: string;
  durum: 'planlandı' | 'gerçekleşti' | 'ertelendi' | 'iptal';
  not: string;
}
export type RaporTur = 'seans' | 'aylik' | 'donem' | 'bep-ilerleme' | 'ram-paketi' | 'aile-bilgilendirme';
export interface Rapor {
  id: string; dosyaUid: string; tur: RaporTur; baslik: string;
  taslak: boolean; onayKim: string | null; onayTarih: string | null;
  kopyaSayisi: number; icerik: string;
}

~~~~

### `lib/depo.ts`
980 B ·SHA `5a092cceee50bc329f3c55f886640b0ab96e7335a10c555bff71c4e274fc8b87`

~~~~tsx
/**
 * Yerel kalıcılık (localStorage) — KVKK yerel-önce ilkesi (K-07/K-09).
 * Buluta hiçbir şey gitmez. Sürüm anahtarı ile şema değişiminde eski veri düşer.
 */
const ONEK = 'seduva-supporta';
const SEMA = 'v1';
const K = (ad: string) => `${ONEK}:${SEMA}:${ad}`;

export function yukle<T>(ad: string, varsayilan: T): T {
  try {
    const ham = localStorage.getItem(K(ad));
    return ham ? (JSON.parse(ham) as T) : varsayilan;
  } catch { return varsayilan; }
}
export function kaydet<T>(ad: string, deger: T): void {
  try { localStorage.setItem(K(ad), JSON.stringify(deger)); } catch { /* kota/kapalı: sessiz geç */ }
}
export function temizle(): void {
  try {
    Object.keys(localStorage).filter((k) => k.startsWith(`${ONEK}:`)).forEach((k) => localStorage.removeItem(k));
  } catch { /* yoksay */ }
}
export function kayitSayisi(): number {
  try { return Object.keys(localStorage).filter((k) => k.startsWith(`${ONEK}:`)).length; } catch { return 0; }
}

~~~~

### `lib/kullan.ts`
355 B ·SHA `46810d4fa8d9838b16029e9c367bf64d1a145ef73f08edacbc99066280d5b842`

~~~~tsx
/** localStorage'a bağlı state kancası. */
import { useEffect, useState } from 'react';
import { yukle, kaydet } from './depo';

export function useKalici<T>(ad: string, varsayilan: T) {
  const [deger, setDeger] = useState<T>(() => yukle(ad, varsayilan));
  useEffect(() => { kaydet(ad, deger); }, [ad, deger]);
  return [deger, setDeger] as const;
}

~~~~

### `main.tsx`
220 B ·SHA `0841d035eaea39546619092e503383a2682334339d1384137f6f4d04c73eeafa`

~~~~tsx
import React from 'react';
import { createRoot } from 'react-dom/client';
import App from './App';
import './index.css';
createRoot(document.getElementById('root')!).render(<React.StrictMode><App /></React.StrictMode>);

~~~~

### `surum.d.ts`
181 B ·SHA `070eb2cfcd976ffdf9a06eea3da5d7186538912f8b14d446be3580645647c54c`

~~~~tsx
/** Sürüm sabiti (K-368). Tek doğruluk kaynağı: package.json → version. */
declare const __SURUM__: string;
declare const __TAM__: boolean;
declare const __PILOT__: boolean;

~~~~

## Ek D — test ve yeniden üretim

Geçici betikler ürün koduna eklenmedi. NODE_PATH ile mevcut MENTORIA araç bağımlılığı kullanıldı; SUPPORTA package/lock veya build değiştirilmedi. Playwright yeni/yalıtılmış bağlamları gerçek kullanıcı kaydı içermez. Dinamik kombinasyonların tümü denenmedi.

### supporta-hazirlik.cjs

~~~~javascript
const fs=require('fs'),path=require('path'),crypto=require('crypto');
const R='/home/user/VAMOLA';const ts=require(R+'/VAMOLA - Seduva/SEDUVA_MENTORIA/node_modules/typescript');
const roots={LEX:'VAMOLA - Lexiva/LEXIVA_SUPPORTA/SUPPORTA_TAM',SED:'VAMOLA - Seduva/SEDUVA_SUPPORTA'};
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
     let pos=sf.getLineAndCharacterOfPosition(n.getStart(sf));rows.push({id:`SUP-${key}-${String(rows.length+1).padStart(4,'0')}`,file:name,line:pos.line+1,kind:ts.SyntaxKind[n.kind],text:value.trim(),reach:name.includes('EgitmenDestekPaneli')?'Bağlı değil: kaynak rezervi':'App/import bağlamında; koşullu görünürlük ayrıca DOM’da'});
    }
   }ts.forEachChild(n,visit);
  }visit(sf);
 }
 const shell=fs.readFileSync(path.join(src,'components/Kabuk.tsx'),'utf8');
 const nav=[...shell.matchAll(/\{ id: '([^']+)', ad: '([^']+)'/g)].map(m=>({id:m[1],label:m[2]}));
 out[key]={root:rel,version:JSON.parse(fs.readFileSync(path.join(R,rel,'package.json'),'utf8')).version,files:meta,rows,nav};
}
fs.writeFileSync('/tmp/supporta-kaynak.json',JSON.stringify(out,null,2));console.log(Object.fromEntries(Object.entries(out).map(([k,v])=>[k,{files:v.files.length,rows:v.rows.length,nav:v.nav.length}])));

~~~~

### supporta-dom.cjs

~~~~javascript
const fs=require('fs'),R='/home/user/VAMOLA';const {chromium}=require(R+'/VAMOLA - Seduva/SEDUVA_MENTORIA/node_modules/playwright-core');
const jobs=[['SED','VAMOLA - Seduva/SEDUVA_SUPPORTA/SUPPORTA-TAM-v0.8.8.html'],['LEX','VAMOLA - Lexiva/LEXIVA_SUPPORTA/SUPPORTA_TAM/LEXIVA-SUPPORTA-v2.10.0.html']];
(async()=>{const b=await chromium.launch();const all={};for(const [key,file] of jobs){const result={file,states:[],errors:[],network:[],roles:[],prints:[],downloads:[]};
 for(const role of ['uzman','yonetici']){const c=await b.newContext({acceptDownloads:true});await c.addInitScript(()=>window.print=()=>{});await c.route(/^https?:/,r=>r.abort());c.on('page',p=>{p.on('pageerror',e=>result.errors.push({role,error:e.message}));p.on('request',r=>{if(/^https?:/.test(r.url()))result.network.push(r.url())})});const p=await c.newPage();p.setDefaultTimeout(7000);await p.goto('file://'+R+'/'+file);
 async function snap(name){result.states.push({role,name,text:await p.locator('body').innerText(),fields:await p.locator('textarea').evaluateAll(es=>es.map(e=>({value:e.value,disabled:e.disabled,readOnly:e.readOnly})))})}
 await snap('rol-secimi');const roles=await p.locator('[data-testid^="rol-"]').evaluateAll(es=>es.map(e=>e.dataset.testid));await p.getByTestId('rol-'+role).click();const ids=await p.locator('nav [data-testid]').evaluateAll(es=>es.map(e=>e.dataset.testid));for(const id of ids){await p.getByTestId(id).click();await snap(id)}
 await p.getByTestId('nav-rapor').click();await p.getByTestId('onayla-R-1').waitFor();result.roles.push({role,roles,nav:ids,canApproveR1:await p.getByTestId('onayla-R-1').isEnabled(),exportBeforeDisabled:await p.getByTestId('disa-R-1').isDisabled()});
 if(role==='uzman'){
 await p.getByRole('button',{name:'Kanıtı İncele ve YZ Önerisi Al',exact:true}).first().click();await snap('rapor-yz-oneri');await p.getByRole('button',{name:'Öneriyi Reddet ve Gerekçelendir',exact:true}).first().click();await snap('rapor-reddet');
 }
 await p.getByTestId('onayla-R-1').click();await p.getByTestId('disa-R-1').waitFor();await snap('rapor-onayli');result.roles[result.roles.length-1].exportAfterEnabled=await p.getByTestId('disa-R-1').isEnabled();
 if(role==='uzman'){
 const got=c.waitForEvent('page'),dl=p.waitForEvent('download');await p.getByTestId('disa-R-1').click();const pop=await got;await pop.waitForLoadState('domcontentloaded');result.prints.push({role,type:'rapor',text:await pop.locator('body').innerText()});await pop.close();const d=await dl;result.downloads.push({name:d.suggestedFilename(),content:fs.readFileSync(await d.path(),'utf8')});
 await p.getByTestId('nav-aile').click();await p.getByTestId('aile-sekme-A').click();await snap('aile-A');
 for(const tab of ['A','B']){await p.getByTestId('aile-sekme-'+tab).click();await snap('aile-sekme-'+tab);const next=c.waitForEvent('page');await p.getByTestId('aile-yazdir-'+tab).click();const pp=await next;await pp.waitForLoadState('domcontentloaded');result.prints.push({role,type:'aile-'+tab,text:await pp.locator('body').innerText()});await pp.close()}
 }
 await c.close();}
 all[key]=result;console.log(key,JSON.stringify({states:result.states.length,roles:result.roles,prints:result.prints.length,downloads:result.downloads.length,errors:result.errors,network:result.network}));}
 await b.close();fs.writeFileSync('/tmp/supporta-dom.json',JSON.stringify(all,null,2));})().catch(e=>{console.error(e);process.exit(2)});

~~~~

### SED kalıcı smoke

~~~~text

TOPLAM: 127 | BASARILI: 127 | HATALI: 0
KONSOL/SAYFA HATASI: 0

~~~~

### LEX kalıcı smoke

~~~~text

TOPLAM: 127 | BASARILI: 127 | HATALI: 0
KONSOL/SAYFA HATASI: 0

~~~~

**Koruma:** tüm manifest anahtarları üzerinden giriş farkı yalnız önceki TESLIM idi. Ürün/kanon/HTML/kalıcı test dosyaları bu hazırlıkta değiştirilmedi; son yazımlar yalnız bu yeni brief ve K-764 DEFTER/kuyruk/devir kayıtlarıdır. Mevcut ZIP/manifest aynı kalır. Dışarıya gönderim yapılmadı.
